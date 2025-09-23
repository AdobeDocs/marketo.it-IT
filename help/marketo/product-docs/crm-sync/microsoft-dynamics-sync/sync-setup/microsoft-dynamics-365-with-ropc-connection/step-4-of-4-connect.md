---
description: Passaggio 4 di 4 - Collegare la soluzione Marketo con la connessione di controllo della password del proprietario della risorsa - Documentazione Marketo - Documentazione del prodotto
title: Passaggio 4 di 4 - Connessione della soluzione Marketo con la connessione del controllo della password del proprietario della risorsa
exl-id: 71a52a3e-f31e-45ee-8196-d536528e42ca
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 0%

---

# Passaggio 4 di 4: connettere la soluzione Marketo con la connessione di controllo della password del proprietario della risorsa {#step-4-of-4-connect-the-marketo-solution-ropc}

Ultimo passaggio della sincronizzazione. Ci sei quasi!

>[!PREREQUISITES]
>
>* [Passaggio 1 di 4: installare la soluzione Marketo con la connessione di controllo password del proprietario della risorsa](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md)
>* [Passaggio 2 di 4: configurare la soluzione Marketo con la connessione di controllo password del proprietario della risorsa](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md)
>* [Passaggio 3 di 4: configurare l&#39;app client in MS [!DNL Dynamics]](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-3-of-4-set-up.md)

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

>[!NOTE]
>
>Se si esegue l&#39;aggiornamento da Autenticazione di base a [!DNL OAuth], è possibile utilizzare [questo articolo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/reconfigure-dynamics-authentication-method.md) per riconfigurare l&#39;autenticazione.

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

   >[!NOTE]
   >
   >Prima di immettere nuove credenziali, puoi [convalidarle qui](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md){target="_blank"}.

1. Immettere **[!UICONTROL Username]**, **[!UICONTROL Password]**, [!DNL Microsoft Dynamics] **[!UICONTROL URL]**, **[!UICONTROL Client ID]** e **[!UICONTROL Client Secret]**. Al termine, fai clic su **[!UICONTROL Save]**.

   ![](assets/step-4-of-4-connect-ropc-5.png)

   >[!NOTE]
   >
   >Il nome utente in Marketo deve corrispondere al nome utente per l&#39;utente di sincronizzazione in CRM. Il formato può essere `user@domain.com` o DOMINIO\utente.

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
   >Marketo non eseguirà la deduplicazione automatica in base a una sincronizzazione [!UICONTROL Microsoft Dynamics] o quando si immettono manualmente persone o lead.

1. Leggi tutto il contenuto del popup, immetti il tuo indirizzo e-mail e fai clic su **[!UICONTROL Start Sync]**.

   ![](assets/image2015-3-16-9-3a55-3a10.png)

1. A seconda del numero di record, la sincronizzazione iniziale può richiedere da alcune ore a pochi giorni. Al termine riceverai una notifica e-mail.

   ![](assets/image2015-3-16-9-3a59-3a51.png)

>[!MORELIKETHIS]
>
>[Riconfigura [!DNL Dynamics] Metodo di autenticazione](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/reconfigure-dynamics-authentication-method.md)
