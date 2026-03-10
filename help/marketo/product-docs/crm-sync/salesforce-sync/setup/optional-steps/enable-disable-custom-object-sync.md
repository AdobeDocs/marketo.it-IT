---
unique-page-id: 4719297
description: Scopri come abilitare o disabilitare la sincronizzazione di oggetti personalizzati di Salesforce in Marketo Engage. Utilizza Admin e Salesforce Objects Sync per selezionare gli oggetti e aggiornare lo schema.
title: Abilitare/disabilitare la sincronizzazione oggetti personalizzati
exl-id: f17d9135-b33e-48c0-9220-131fb437e9e5
feature: Salesforce Integration
source-git-commit: 2b29f05a27f847184e0968442012d443e9e0597d
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 9%

---

# Abilitare/disabilitare la sincronizzazione oggetti personalizzati {#enable-disable-custom-object-sync}

Anche gli oggetti personalizzati creati nell’istanza Salesforce possono far parte di Marketo Engage. Ecco come configurarlo.

## Abilitare/disabilitare la sincronizzazione oggetti personalizzati {#enable-disable-custom-object-sync-1}

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

1. Passa alla schermata **[!UICONTROL Admin]**.

   ![](assets/enable-disable-custom-object-sync-1.png)

1. Scegliere **[!UICONTROL Salesforce Objects Sync]** dal menu Gestione database.

   ![](assets/enable-disable-custom-object-sync-2.png)

1. Se si tratta del primo oggetto personalizzato, fare clic su **[!UICONTROL Sync schema]**. In caso contrario, fai clic su **[!UICONTROL Refresh Schema]** per assicurarti di disporre dell&#39;ultima versione.

   ![](assets/enable-disable-custom-object-sync-3.png)

1. Se la sincronizzazione globale è in esecuzione, sarà necessario disattivarla facendo clic su **[!UICONTROL Disable Global Sync]**.

   ![](assets/image2014-12-10-10-3a14-3a54.png)

   >[!NOTE]
   >
   >La sincronizzazione dello schema di oggetti personalizzato [!DNL Salesforce] potrebbe richiedere alcuni minuti.

1. Fai clic su **[!UICONTROL Refresh Schema]**.

   ![](assets/image2014-12-10-10-3a15-3a7.png)

1. Selezionare l&#39;oggetto da sincronizzare e fare clic su **[!UICONTROL Enable Sync]**.

   >[!TIP]
   >
   >Marketo può sincronizzare un oggetto personalizzato solo se ha una relazione diretta con l&#39;oggetto Lead, Contact o Account in [!DNL Salesforce].

   ![](assets/image2014-12-10-10-3a15-3a30.png)

1. Fare di nuovo clic su **[!UICONTROL Enable Sync]**.

   ![](assets/image2014-12-10-10-3a15-3a40.png)

1. Tornare alla scheda **[!DNL Salesforce]** e fare clic su **[!UICONTROL Enable Sync]**.

   ![](assets/image2014-12-10-10-3a15-3a49.png)

## Utilizzo degli oggetti personalizzati {#using-your-custom-objects}

>[!NOTE]
>
>Non è possibile utilizzare oggetti personalizzati in Smart Campaigns con trigger.

1. Nell&#39;elenco avanzato, trascinare il mouse sul filtro **[!UICONTROL Has Opportunity]** e impostare su **[!UICONTROL true]**.

   ![](assets/image2015-8-26-9-3a39-3a28.png)

1. Quindi, utilizzate i vincoli di filtro per restringere lo stato attivo.

   ![](assets/image2015-8-24-14-3a18-3a53.png)

   Eccellente! È ora possibile utilizzare i dati di questo oggetto personalizzato nelle campagne avanzate e negli elenchi avanzati.

>[!MORELIKETHIS]
>
>[Aggiungi/Rimuovi campo oggetto personalizzato come elenco avanzato/vincoli trigger](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target="_blank"}
