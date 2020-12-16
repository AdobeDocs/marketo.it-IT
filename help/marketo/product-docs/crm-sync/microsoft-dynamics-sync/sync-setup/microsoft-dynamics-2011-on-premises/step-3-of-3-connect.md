---
unique-page-id: 3571809
description: Passaggio 3 di 3 - Connetti Microsoft Dynamics con Marketo (On-Premises 2011) - Marketo Docs - Documentazione prodotto
title: Passaggio 3 di 3 - Connetti Microsoft Dynamics con Marketo (On-Premises 2011)
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 0%

---


# Passaggio 3 di 3: Connect Microsoft Dynamics con Marketo (On-Premises 2011) {#step-of-connect-microsoft-dynamics-with-marketo-on-premises}

Bene! Abbiamo installato la soluzione e configurato l&#39;utente di sincronizzazione. Quindi, dobbiamo collegare Marketo e Dynamics.

>[!PREREQUISITES]
>
>* [Passaggio 1 di 3: Installare la soluzione Marketo (On-Premises 2011)](step-1-of-3-install.md)
>* [Passaggio 2 di 3: Impostazione della sincronizzazione degli utenti di Marketing in Dynamics (On-Premises 2011)](step-2-of-3-set-up.md)


>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

## Immettere le informazioni utente di Dynamics Sync {#enter-dynamics-sync-user-information}

1. Accedete a Marketo e fate clic su **Admin**.

   ![](assets/login-admin.png)

1. Fate clic su **CRM**.

   ![](assets/image2014-12-11-11-3a53-3a59.png)

1. Fate clic su **Microsoft**.

   ![](assets/image2014-12-11-11-3a54-3a10.png)

1. Fate clic su **Modifica** nel **passaggio 1: Immettere le credenziali.**

   ![](assets/image2014-12-11-11-3a54-3a19.png)

   >[!CAUTION]
   >
   >Verificate che le credenziali siano corrette in quanto non sarà possibile ripristinare le modifiche successive dello schema dopo l&#39;invio. Se vengono salvate credenziali errate, dovrete ottenere una nuova iscrizione a Marketo.

1. Immettete il **nome** utente, la **password** e l&#39; **URL** CRM, quindi fate clic su **Salva**.

   ![](assets/image2015-4-2-14-3a50-3a7.png)

   >[!NOTE]
   >
   >Il nome utente in Marketo deve corrispondere al nome utente per l&#39;utente di sincronizzazione in CRM. Il formato può essere [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#a0d5d3c5d2e0c4cfcdc1c9ce8ec3cfcd) o DOMINIO\utente.

   >[!TIP]
   >
   >Non conosci l&#39;URL? Verrà mostrato come trovare l&#39;URL [del servizio](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md) Dynamics Organization.

## Seleziona campi da sincronizzare {#select-fields-to-sync}

Ora è necessario selezionare i campi sui quali eseguire la sincronizzazione.

1. Fate clic su **Modifica** nel **passaggio 2: Selezionare Campi da sincronizzare.**

   ![](assets/image2015-3-16-9-51-28a.png)

1. Sono presenti campi preselezionati che verranno sincronizzati. Aggiungete altro se lo desiderate e fate clic su **Salva**.

   ![](assets/image2016-8-25-13-3a26-3a14.png)

## Campi di sincronizzazione per un filtro personalizzato {#sync-fields-for-a-custom-filter}

Se avete creato un filtro personalizzato, accertatevi di entrare e selezionare i nuovi campi da sincronizzare con Marketo.

1. Vai ad Admin e seleziona **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Fate clic su **Modifica** in Dettagli sincronizzazione campo.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Scorri verso il basso fino al campo e controllalo. Il nome effettivo deve essere new_synctomkto, ma il nome visualizzato può essere qualsiasi cosa. Fate clic su **Salva**.

   ![](assets/image2016-8-25-14-3a14-3a57.png)

## Abilita sincronizzazione {#enable-sync}

1. Fate clic su **Modifica** nel **passaggio 3: Abilita sincronizzazione**.

   ![](assets/image2015-3-16-9-52-2b.png)

   >[!CAUTION]
   >
   >Marketo non eseguirà automaticamente la deduplicazione rispetto a una sincronizzazione di Microsoft Dynamics, o quando immetti manualmente persone o lead.

1. Leggete tutto nella finestra a comparsa, inserite il messaggio e-mail e fate clic su **Avvia sincronizzazione**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. La prima sincronizzazione potrebbe richiedere alcune ore. Al termine, riceverete una notifica e-mail.

   ![](assets/image2014-12-11-11-3a55-3a15.png)

   Ottimo lavoro!
