---
unique-page-id: 7504744
description: Installazione di Marketo per Microsoft Dynamics 2015 on-premises Passaggio 3 di 3 - Documentazione di Marketo - Documentazione del prodotto
title: Installazione di Marketo per Microsoft Dynamics 2015 on-premise - Passaggio 3 di 3
exl-id: 054bf725-7a80-4114-8360-2d86e2e33dd7
feature: Microsoft Dynamics
source-git-commit: 2d3264ab75d2327f9226373aad383e7a51508589
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 1%

---

# Passaggio 3 di 3: Connessione a Marketo Dynamics (on-prem 2015) {#step-of-connect-marketo-dynamics-on-premises-2015}

>[!PREREQUISITES]
>
>* [Installa Marketo per Microsoft Dynamics 2015 locale Passaggio 1 di 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-1-of-3-install-2015.md){target="_blank"}
>* [Installa Marketo per Microsoft Dynamics 2015 on-premise passaggio 2 di 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-set-up-2015.md){target="_blank"}

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

## Immetti le informazioni utente di Dynamics Sync {#enter-dynamics-sync-user-information}

1. Accedere a Marketo e fare clic su **[!UICONTROL Admin]**.

   ![](assets/login-admin.png)

1. Fai clic su **[!UICONTROL CRM]**.

   ![](assets/image2015-3-16-9-47-34.png)

1. Seleziona **[!UICONTROL Microsoft]**.

   ![](assets/image2015-3-16-9-50-6.png)

1. Fare clic su **[!UICONTROL Edit]** in **[!UICONTROL Enter Credentials]**.

   ![](assets/image2015-3-16-9-48-43.png)

   >[!CAUTION]
   >
   >Assicurati che le credenziali siano corrette in quanto non è possibile ripristinare le modifiche allo schema successive dopo l’invio. Se vengono salvate credenziali non corrette, dovrai ottenere una nuova sottoscrizione Marketo.

1. Immetti **[!UICONTROL Username]**, **[!UICONTROL Password]** un Microsoft Dynamics **[!UICONTROL URL]** e un **ID/segreto client**. Al termine, fai clic su **[!UICONTROL Save]**.

   ![](assets/step-3-of-3-5.png)

   >[!NOTE]
   >
   >* Se il provisioning del tuo Marketo è stato eseguito prima di ottobre 2020, ID client e Segreto sono campi facoltativi. Altrimenti sono obbligatori. L’ottenimento di queste informazioni dipende dalla versione di MSD in uso.
   >* Il nome utente in Marketo deve corrispondere al nome utente per l&#39;utente di sincronizzazione in CRM. Il formato può essere `user@domain.com` o DOMINIO\utente.
   >* Se non conosci l&#39;URL, [scopri come trovarlo qui](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md){target="_blank"}.

   >[!TIP]
   >
   >Non conosci l’URL? Qui verrà illustrato come trovare l&#39;[URL del servizio Dynamics Organization](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/view-the-organization-service-url.md){target="_blank"}.

## Seleziona campi da sincronizzare {#select-fields-to-sync}

1. Fare clic su **[!UICONTROL Edit]** in **[!UICONTROL Select Fields to Sync]**.

   ![](assets/image2015-3-16-9-51-28.png)

1. Seleziona i campi da sincronizzare con Marketo in modo che siano preselezionati. Fai clic su **[!UICONTROL Save]**.

   ![](assets/image2016-8-25-15-3a14-3a28.png)

>[!NOTE]
>
>Marketo memorizza un riferimento ai campi da sincronizzare. Se elimini un campo in Dynamics, è consigliabile eliminare [sync disabilitato](/help/marketo/product-docs/crm-sync/salesforce-sync/enable-disable-the-salesforce-sync.md){target="_blank"}. Quindi aggiorna lo schema in Marketo modificando e salvando [Seleziona campi da sincronizzare](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-field-sync/editing-fields-to-sync-before-deleting-them-in-dynamics.md){target="_blank"}.

## Sincronizza campi per un filtro personalizzato {#sync-fields-for-a-custom-filter}

Se hai creato un filtro personalizzato, accertati di entrare e selezionare i nuovi campi da sincronizzare con Marketo.

1. Vai all&#39;amministratore e seleziona **[!UICONTROL Microsoft Dynamics]**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Fare clic su **[!UICONTROL Edit]** in Dettagli sincronizzazione campi.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. Scorri verso il basso fino al campo e selezionalo. Il nome effettivo deve essere new_synctomkto, ma il nome visualizzato può essere qualsiasi cosa. Fai clic su **[!UICONTROL Save]**.

   ![](assets/image2016-8-25-15-3a15-3a35.png)

## Abilita sincronizzazione {#enable-sync}

1. Fare clic su **[!UICONTROL Edit]** in **[!UICONTROL Enable Sync]**.

   ![](assets/image2015-3-16-9-52-2.png)

   >[!CAUTION]
   >
   >Marketo non esegue automaticamente la deduplicazione su una sincronizzazione Microsoft Dynamics o quando si immettono manualmente persone.

1. Leggi tutto il contenuto del popup, immetti il tuo indirizzo e-mail e fai clic su **[!UICONTROL Start Sync]**.

   ![](assets/image2015-3-30-14-3a23-3a13.png)

1. A seconda del numero di record, la sincronizzazione iniziale può richiedere da alcune ore a pochi giorni. Al termine riceverai una notifica e-mail.

   ![](assets/image2015-3-16-9-59-51.png)
