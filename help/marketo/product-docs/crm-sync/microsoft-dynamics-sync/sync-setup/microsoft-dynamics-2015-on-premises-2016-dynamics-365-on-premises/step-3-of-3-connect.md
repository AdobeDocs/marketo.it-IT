---
unique-page-id: 7504744
description: Installazione di Marketo per Dynamics 2015 On-Prem e 2016 365 On-Prem Step 3 di 3 - Marketo Docs - Documentazione prodotto
title: Installazione di Marketo per Dynamics 2015 On-Prem e 2016 365 On-Prem Step 3 di 3
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 0%

---


# Installazione di Marketo per Dynamics 2015 On-Prem e 2016 365 On-Prem Step 3 di 3 {#install-marketo-for-dynamics-on-prem-and-on-prem-step-of}

>[!PREREQUISITES]
>
>* [Installazione di Marketo per Dynamics 2015 On-Prem e 2016 365 On-Prem Step 1 di 3](step-1-of-3-install.md)
>* [Installazione di Marketo per Dynamics 2015 On-Prem e 2016 365 On-Prem Step 2 di 3](step-2-of-3-set-up.md)

>



>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

## Immettere le informazioni utente di Dynamics Sync {#enter-dynamics-sync-user-information}

1. Accedi a Marketo e fai clic su **Admin**.

   ![](assets/login-admin.png)

1. Fate clic su **CRM**.

   ![](assets/image2015-3-16-9-47-34.png)

1. Selezionare **Microsoft**.

   ![](assets/image2015-3-16-9-50-6.png)

1. Fate clic su **Modifica** nel **passaggio 1: Immettere le credenziali**.

   ![](assets/image2015-3-16-9-48-43.png)

   >[!CAUTION]
   >
   >Verificate che le credenziali siano corrette in quanto non sarà possibile ripristinare le modifiche successive dello schema dopo l&#39;invio. Se vengono salvate credenziali errate, dovrete ottenere una nuova iscrizione a Marketo.

1. Immettete il **nome** utente, la **password** un **URL** di Microsoft Dynamics e un ID **** client facoltativo. Al termine, fate clic su **Salva** .

   ![](assets/client-id.png)

   >[!NOTE]
   >
   >Il nome utente in Marketo deve corrispondere al nome utente per l&#39;utente di sincronizzazione in CRM. Il formato può essere [`[email protected]`](http://docs.marketo.com/cdn-cgi/l/email-protection#8cf9ffe9fecce8e3e1ede5e2a2efe3e1) o DOMINIO\utente.

   >[!TIP]
   >
   >Non conosci l&#39;URL? Verrà illustrato come trovare l&#39;URL [del servizio](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md) Dynamics Organization.

## Seleziona campi da sincronizzare {#select-fields-to-sync}

1. Fate clic su **Modifica** nel **passaggio 2: Selezionare Campi da sincronizzare**.

   ![](assets/image2015-3-16-9-51-28.png)

1. Selezionate i campi che desiderate sincronizzare con Marketo, in modo che siano preselezionati. Fate clic su **Salva**.

   ![](assets/image2016-8-25-15-3a14-3a28.png)

## Campi di sincronizzazione per un filtro personalizzato {#sync-fields-for-a-custom-filter}

Se avete creato un filtro personalizzato, accertatevi di entrare e selezionare i nuovi campi da sincronizzare con Marketo.

1. Vai ad Admin e seleziona **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Fate clic su **Modifica** in Dettagli sincronizzazione campo.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Scorri verso il basso fino al campo e controllalo. Il nome effettivo deve essere new_synctomkto, ma il nome visualizzato può essere qualsiasi cosa. Fate clic su **Salva**.

   ![](assets/image2016-8-25-15-3a15-3a35.png)

## Abilita sincronizzazione {#enable-sync}

1. Fate clic su **Modifica** nel **passaggio 3: Abilita sincronizzazione**.

   ![](assets/image2015-3-16-9-52-2.png)

   >[!CAUTION]
   >
   >Marketo non eseguirà automaticamente la deduplicazione rispetto a una sincronizzazione di Microsoft Dynamics o quando immetti manualmente le persone.

1. Leggete tutto nella finestra a comparsa, inserite il messaggio e-mail e fate clic su **Avvia sincronizzazione**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. La prima sincronizzazione potrebbe richiedere alcune ore. Al termine, riceverete una notifica e-mail.

   ![](assets/image2015-3-16-9-59-51.png)

Ottimo lavoro!
