---
unique-page-id: 3571830
description: 'Passaggio 3 di 3: collegare Microsoft Dynamics con Marketo (Online) - Documenti Marketo - Documentazione del prodotto'
title: 'Passaggio 3 di 3: collegare Microsoft Dynamics con Marketo (Online)'
translation-type: tm+mt
source-git-commit: ed9399396c82a3b2fb93c83ffdaa1dc7b0827306
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---


# Passaggio 3 di 3: Collegare Microsoft Dynamics con Marketo (Online) {#step-of-connect-microsoft-dynamics-with-marketo-online}

Questo è l&#39;ultimo passaggio della sincronizzazione. Ci siamo quasi!

>[!PREREQUISITES]
>
>* [Passaggio 1 di 3: Installare la soluzione Marketo (online)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-1-of-3-install.md)
>* [Passaggio 2 di 3: Configurare l’utente di sincronizzazione di Marketo in Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-2-of-3-set-up.md)


>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

## Immetti le informazioni utente di Dynamics Sync {#enter-dynamics-sync-user-information}

1. Accedi a Marketo e fai clic su **Amministratore**.

   ![](assets/login-admin.png)

1. Fai clic su **CRM**.

   ![](assets/image2015-3-16-9-3a47-3a34.png)

1. Selezionare **Microsoft**.

   ![](assets/image2015-3-16-9-3a50-3a6.png)

1. Fare clic su **Modifica** in **Passaggio 1: Immettere Credentials**.

   ![](assets/image2015-3-16-9-3a48-3a43.png)

   >[!CAUTION]
   >
   >Assicurati che le tue credenziali siano corrette in quanto non è possibile ripristinare le successive modifiche dello schema dopo l’invio. Se vengono salvate le credenziali errate, dovrai ottenere una nuova sottoscrizione Marketo.

1. Inserisci **Nome utente**, **Password** e Microsoft Dynamics **URL**. Al termine, fai clic su **Salva**.

   ![](assets/five-1.png)

   >[!NOTE]
   >
   >* Se il provisioning di Marketo è stato eseguito prima di ottobre 2020, l’ID client e il segreto sono campi facoltativi. Altrimenti, sono obbligatori. L&#39;ottenimento di queste informazioni dipenderà dalla versione di MSD in uso.
   >* Il nome utente in Marketo deve corrispondere al nome utente per l&#39;utente di sincronizzazione in CRM. Il formato può essere `user@domain.com` o DOMAIN\user.
   >* Se non conosci l&#39;URL, [scopri come trovarlo qui](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md).


## Seleziona campi da sincronizzare {#select-fields-to-sync}

1. Fare clic su **Modifica** in **Passaggio 2: Selezionare Campi da sincronizzare**.

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. Seleziona i campi da sincronizzare con Marketo in modo che vengano preselezionati. Fare clic su **Salva**.

   ![](assets/image2016-8-25-15-3a6-3a11.png)

>[!NOTE]
>
>Marketo memorizza un riferimento ai campi da sincronizzare. Se elimini un campo in Dynamics, è consigliabile eseguire questa operazione con la funzione [sincronizzazione disabilitata](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md). Quindi aggiorna lo schema in Marketo modificando e salvando [Seleziona campi da sincronizzare](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md).

## Campi di sincronizzazione per un filtro personalizzato {#sync-fields-for-a-custom-filter}

Se hai creato un filtro personalizzato, assicurati di entrare e selezionare i nuovi campi da sincronizzare con Marketo.

1. Vai ad Amministratore e seleziona **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Fare clic su **Modifica** in Dettagli sincronizzazione campi.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Scorri verso il basso fino al campo e controllalo. Il nome effettivo deve essere new_synctomkto ma il nome visualizzato può essere qualsiasi cosa. Fare clic su **Salva**.

   ![](assets/image2016-8-25-15-3a7-3a35.png)

## Abilita sincronizzazione {#enable-sync}

1. Fare clic su **Modifica** in **Passaggio 3: Abilita Sync**.

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketo non eseguirà automaticamente la deduplicazione rispetto a una sincronizzazione di Microsoft Dynamics o quando si immettono manualmente persone o lead.

1. Leggi tutto nella finestra a comparsa, inserisci il tuo indirizzo e-mail e fai clic su **Avvia sincronizzazione**.

   ![](assets/image2015-3-16-9-3a55-3a10.png)

1. La prima sincronizzazione potrebbe richiedere alcune ore. Al termine riceverai una notifica e-mail.

   ![](assets/image2015-3-16-9-3a59-3a51.png)

Ottimo lavoro!
