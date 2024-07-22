---
unique-page-id: 4719297
description: Abilitare/Disabilitare la sincronizzazione oggetti personalizzati - Documentazione di Marketo - Documentazione del prodotto
title: Abilita/Disabilita sincronizzazione oggetti personalizzati
exl-id: f17d9135-b33e-48c0-9220-131fb437e9e5
feature: Salesforce Integration
source-git-commit: 756a38ba87dd5af9ee783e9709056d444d4f415b
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---

# Abilita/Disabilita sincronizzazione oggetti personalizzati {#enable-disable-custom-object-sync}

Anche gli oggetti personalizzati creati nell’istanza Salesforce possono far parte del Marketo Engage. Ecco come configurarlo.

## Abilita/Disabilita sincronizzazione oggetti personalizzati {#enable-disable-custom-object-sync-1}

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

1. Fai clic su **[!UICONTROL Amministratore]**.

   ![](assets/one.png)

1. Scegliere **[!UICONTROL Sincronizzazione oggetti Salesforce]** dal menu Gestione database.

   ![](assets/two-2.png)

1. Se si tratta del primo oggetto personalizzato, fare clic su **[!UICONTROL Sincronizza schema]**. In caso contrario, fare clic su **[!UICONTROL Aggiorna schema]** per verificare di disporre dell&#39;ultima versione.

   ![](assets/image2014-12-10-10-3a14-3a44.png)

1. Se la sincronizzazione globale è in esecuzione, è necessario disattivarla facendo clic su **[!UICONTROL Disattiva sincronizzazione globale]**.

   ![](assets/image2014-12-10-10-3a14-3a54.png)

   >[!NOTE]
   >
   >La sincronizzazione dello schema di oggetti personalizzato di Salesforce potrebbe richiedere alcuni minuti.

1. Fare clic su **[!UICONTROL Aggiorna schema]**.

   ![](assets/image2014-12-10-10-3a15-3a7.png)

1. Selezionare l&#39;oggetto da sincronizzare e fare clic su **[!UICONTROL Abilita sincronizzazione]**.

   >[!TIP]
   >
   >Marketo può sincronizzare un oggetto personalizzato solo se ha una relazione diretta con l’oggetto Lead, Contact o Account in Salesforce.

   ![](assets/image2014-12-10-10-3a15-3a30.png)

1. Fai di nuovo clic su **[!UICONTROL Abilita sincronizzazione]**.

   ![](assets/image2014-12-10-10-3a15-3a40.png)

1. Torna alla scheda **[!DNL Salesforce]** e fai clic su **[!UICONTROL Abilita sincronizzazione]**.

   ![](assets/image2014-12-10-10-3a15-3a49.png)

## Utilizzo degli oggetti personalizzati {#using-your-custom-objects}

>[!NOTE]
>
>Non è possibile utilizzare oggetti personalizzati in Smart Campaigns con trigger.

1. Nell&#39;elenco avanzato, trascina il filtro **[!UICONTROL Ha opportunità]** e imposta su **[!UICONTROL true]**.

   ![](assets/image2015-8-26-9-3a39-3a28.png)

1. Quindi, utilizzate i vincoli di filtro per restringere lo stato attivo.

   ![](assets/image2015-8-24-14-3a18-3a53.png)

   Eccellente! È ora possibile utilizzare i dati di questo oggetto personalizzato nelle campagne avanzate e negli elenchi avanzati.

>[!MORELIKETHIS]
>
>[Aggiungi/Rimuovi campo oggetto personalizzato come elenco avanzato/vincoli trigger](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target="_blank"}
