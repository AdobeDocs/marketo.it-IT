---
unique-page-id: 3571830
description: Passaggio 3 di 3 - Connessione della soluzione Marketo con la connessione server-to-server - Documentazione di Marketo - Documentazione del prodotto
title: Passaggio 3 di 3 - Connessione della soluzione Marketo con la connessione server-to-server
exl-id: e3ede749-f787-45d3-adb4-f71ef1221208
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '420'
ht-degree: 0%

---

# Passaggio 3 di 3: connettere la soluzione Marketo con la connessione server-server {#step-3-of-3-connect-microsoft-dynamics-with-marketo-solution-s2s}

Ultimo passaggio della sincronizzazione. Ci siamo quasi!

>[!PREREQUISITES]
>
>* [Passaggio 1 di 3: installare la soluzione Marketo con connessione server-server](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-1-of-3-install.md){target="_blank"}
>* [Passaggio 2 di 3: configurare la soluzione Marketo con connessione server-server](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-s2s-connection/step-2-of-3-set-up.md){target="_blank"}

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

>[!IMPORTANT]
>
>Se si esegue l&#39;aggiornamento da Autenticazione di base a [!DNL OAuth], è necessario contattare il [Supporto Marketo](https://nation.marketo.com/t5/support/ct-p/Support) per ricevere assistenza nell&#39;aggiornamento dei parametri aggiuntivi. Se si abilita questa funzionalità, la sincronizzazione verrà temporaneamente interrotta finché non verranno immesse nuove credenziali e la sincronizzazione non verrà riabilitata. Se desideri ripristinare la modalità di autenticazione precedente, la funzione può essere disabilitata (fino ad aprile 2022).

>[!NOTE]
>
>Prima di immettere nuove credenziali, puoi [convalidarle qui](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md){target="_blank"}.

## Immetti le informazioni utente di sincronizzazione di [!DNL Dynamics] {#enter-dynamics-sync-user-information}

1. Accedere a Marketo e fare clic su **[!UICONTROL Admin]**.

   ![](assets/login-admin.png)

1. Fai clic su **[!UICONTROL CRM]**.

   ![](assets/image2015-3-16-9-3a47-3a34.png)

1. Seleziona **[!UICONTROL Microsoft]**.

   ![](assets/image2015-3-16-9-3a50-3a6.png)

1. Fare clic su **[!UICONTROL Edit]** in **[!UICONTROL Step 1: Enter Credentials]**.

   ![](assets/image2015-3-16-9-3a48-3a43.png)

   >[!CAUTION]
   >
   >Assicurati che l’URL dell’organizzazione sia corretto, poiché non è possibile ripristinare le modifiche allo schema successive dopo l’invio. Se viene utilizzato un URL organizzazione errato, dovrai ottenere una nuova sottoscrizione Marketo. Se non conosci l&#39;URL, [scopri come trovarlo qui](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md){target="_blank"}.

1. Immettere le informazioni utente di sincronizzazione di [!DNL Dynamics] e al termine fare clic su **[!UICONTROL Save]**.

   ![](assets/step-3-of-3-connect-s2s-5.png)

   >[!NOTE]
   >
   >Il nome utente in Marketo deve corrispondere all&#39;[indirizzo e-mail](https://docs.microsoft.com/en-us/power-platform/admin/manage-application-users#view-or-edit-the-details-of-an-application-user){target="_blank"} dell&#39;utente dell&#39;applicazione nel CRM. Il formato può essere `user@domain.com` o DOMINIO\utente.

## Seleziona campi da sincronizzare {#select-fields-to-sync}

1. Fare clic su **[!UICONTROL Edit]** in **[!UICONTROL Step 2: Select Fields to Sync]**.

   ![](assets/image2015-3-16-9-3a51-3a28.png)

1. Seleziona i campi da sincronizzare con Marketo in modo che siano preselezionati. Fai clic su **[!UICONTROL Save]**.

   ![](assets/image2016-8-25-15-3a6-3a11.png)

>[!NOTE]
>
>Marketo memorizza un riferimento ai campi da sincronizzare. Se elimini un campo in [!DNL Dynamics], è consigliabile eliminare [sync disabilitato](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md). Quindi aggiorna lo schema in Marketo modificando e salvando [Seleziona campi da sincronizzare](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md).

## Sincronizza campi per un filtro personalizzato {#sync-fields-for-a-custom-filter}

Se hai creato un filtro personalizzato, accertati di entrare e selezionare i nuovi campi da sincronizzare con Marketo.

1. Vai a [!UICONTROL Admin] e seleziona **[!UICONTROL Microsoft Dynamics]**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Fare clic su **[!UICONTROL Edit]** il [!UICONTROL Field Sync Details].

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Scorri verso il basso fino al campo e selezionalo. Il nome effettivo deve essere new_synctomkto, ma il nome visualizzato può essere qualsiasi cosa. Fai clic su **[!UICONTROL Save]**.

   ![](assets/image2016-8-25-15-3a7-3a35.png)

## Abilita sincronizzazione {#enable-sync}

1. Fare clic su **[!UICONTROL Edit]** in **[!UICONTROL Step 3: Enable Sync]**.

   ![](assets/image2015-3-16-9-3a52-3a2.png)

   >[!CAUTION]
   >
   >Marketo non eseguirà la deduplicazione automatica in base a una sincronizzazione [!DNL Microsoft Dynamics] o quando si immettono manualmente persone o lead.

1. Leggi tutto il contenuto del popup, immetti il tuo indirizzo e-mail e fai clic su **[!UICONTROL Start Sync]**.

   ![](assets/image2015-3-16-9-3a55-3a10.png)

1. A seconda del numero di record, la sincronizzazione iniziale può richiedere da alcune ore a pochi giorni. Al termine riceverai una notifica e-mail.

   ![](assets/image2015-3-16-9-3a59-3a51.png)
