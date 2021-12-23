---
unique-page-id: 3571809
description: 'Passaggio 3 di 3: collegare Microsoft Dynamics con Marketo (On-Premises 2011) - Documentazione di Marketo - Documentazione del prodotto'
title: 'Passaggio 3 di 3: collegare Microsoft Dynamics con Marketo (On-Premises 2011)'
exl-id: e6a5d49d-025a-4899-9e92-7a4c32086c67
source-git-commit: 2568d3414c8aaec882b79442f6312bae3b9514ab
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 0%

---

# Passaggio 3 di 3: Collegare Microsoft Dynamics con Marketo (On-Premises 2011) {#step-of-connect-microsoft-dynamics-with-marketo-on-premises}

Bene! Abbiamo installato la soluzione e configurato l&#39;utente di sincronizzazione. Successivamente, è necessario collegare Marketo e Dynamics.

>[!PREREQUISITES]
>
>* [Passaggio 1 di 3: Installare la soluzione Marketo (On-Premises 2011)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-1-of-3-install.md)
>* [Passaggio 2 di 3: Configurazione dell’utente di sincronizzazione Marketo in Dynamics (On-Premises 2011)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2011-on-premises/step-2-of-3-set-up.md)


>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

## Immetti le informazioni utente di Dynamics Sync {#enter-dynamics-sync-user-information}

1. Accedi a Marketo e fai clic su **Amministratore**.

   ![](assets/login-admin.png)

1. Fai clic su **CRM**.

   ![](assets/image2014-12-11-11-3a53-3a59.png)

1. Fai clic su **Microsoft**.

   ![](assets/image2014-12-11-11-3a54-3a10.png)

1. Fai clic su **Modifica** in **Passaggio 1: Immetti le credenziali.**

   ![](assets/image2014-12-11-11-3a54-3a19.png)

   >[!CAUTION]
   >
   >Assicurati che le tue credenziali siano corrette in quanto non è possibile ripristinare le successive modifiche dello schema dopo l’invio. Se vengono salvate le credenziali errate, sarà necessario ottenere una nuova sottoscrizione Marketo.

1. Inserisci il **Nome utente**, **Password** e CRM **URL** quindi fai clic su **Salva**.

   ![](assets/image2015-4-2-14-3a50-3a7.png)

   >[!NOTE]
   >
   >* Il nome utente in Marketo deve corrispondere al nome utente per l&#39;utente di sincronizzazione in CRM. Il formato può essere `user@domain.com` o DOMINIO\utente.
   >* Se non conosci l’URL, [scopri come trovarlo qui](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md).


## Seleziona campi da sincronizzare {#select-fields-to-sync}

Ora è necessario selezionare i campi su cui si desidera eseguire la sincronizzazione.

1. Fai clic su **Modifica** in **Passaggio 2: Selezionare Campi da sincronizzare.**

   ![](assets/image2015-3-16-9-51-28a.png)

1. Sono presenti campi preselezionati che verranno sincronizzati. Aggiungi altro, se lo desideri, e fai clic su **Salva**.

   ![](assets/image2016-8-25-13-3a26-3a14.png)

   >[!NOTE]
   >
   >Marketo memorizza un riferimento ai campi da sincronizzare. Se elimini un campo in Dynamics, è consigliabile eseguire questa operazione con la [sincronizzazione disabilitata](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md). Quindi aggiorna lo schema in Marketo modificando e salvando il [Seleziona campi da sincronizzare](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md).

## Campi di sincronizzazione per un filtro personalizzato {#sync-fields-for-a-custom-filter}

Se hai creato un filtro personalizzato, assicurati di entrare e selezionare i nuovi campi da sincronizzare con Marketo.

1. Vai ad Amministratore e seleziona **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Fai clic su **Modifica** in Dettagli sincronizzazione campo.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Scorri verso il basso fino al campo e controllalo. Il nome effettivo deve essere new_synctomkto ma il nome visualizzato può essere qualsiasi cosa. Fai clic su **Salva**.

   ![](assets/image2016-8-25-14-3a14-3a57.png)

## Abilita sincronizzazione {#enable-sync}

1. Fai clic su **Modifica** in **Passaggio 3: Abilita sincronizzazione**.

   ![](assets/image2015-3-16-9-52-2b.png)

   >[!CAUTION]
   >
   >Marketo non eseguirà automaticamente il deduplicazione rispetto a una sincronizzazione di Microsoft Dynamics o quando immetti manualmente persone o lead.

1. Leggi tutto nella finestra a comparsa, inserisci il tuo messaggio e-mail e fai clic su **Avvia sincronizzazione**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. La prima sincronizzazione potrebbe richiedere alcune ore. Al termine riceverai una notifica e-mail.

   ![](assets/image2014-12-11-11-3a55-3a15.png)

   Ottimo lavoro!
