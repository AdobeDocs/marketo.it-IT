---
description: Abilitare/Disabilitare la sincronizzazione oggetti personalizzati - Documentazione di Marketo - Documentazione del prodotto
title: Abilitare/disabilitare la sincronizzazione oggetti personalizzati
exl-id: 01417fb6-70f5-449b-ad56-42e1c0b2ff68
feature: Veeva CRM
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 5%

---

# Abilitare/disabilitare la sincronizzazione oggetti personalizzati {#enable-disable-custom-object-sync}

Anche gli oggetti personalizzati creati nell&#39;istanza di CRM [!DNL Veeva] possono far parte di Marketo Engage. Ecco come configurarlo.

## Attivare o disattivare la sincronizzazione oggetti personalizzati {#enable-or-disable-the-custom-object-sync}

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

1. In Marketo, fai clic su **[!UICONTROL Admin]**, quindi su **[!UICONTROL Veeva Objects Sync]**.

   ![](assets/enable-disable-custom-object-sync-1.png)

1. Se si tratta del primo oggetto personalizzato, fare clic su **[!UICONTROL Sync Schema]**. In caso contrario, fare clic su **[!UICONTROL Refresh Schema]** per verificare di disporre dell&#39;ultima versione.

   ![](assets/enable-disable-custom-object-sync-2.png)

1. Se la sincronizzazione globale è in esecuzione, disabilitarla facendo clic su **[!UICONTROL Disable Global Sync]**.

   ![](assets/enable-disable-custom-object-sync-3.png)

   >[!NOTE]
   >
   >La sincronizzazione dello schema di oggetti personalizzato [!DNL Veeva] potrebbe richiedere alcuni minuti.

1. Fai clic su **[!UICONTROL Refresh Schema]**.

   ![](assets/enable-disable-custom-object-sync-4.png)

Selezionare l&#39;oggetto da sincronizzare e fare clic su **[!UICONTROL Enable Sync]**.

![](assets/enable-disable-custom-object-sync-5.png)

>[!TIP]
>
>Marketo può sincronizzare un oggetto personalizzato solo se ha una relazione diretta con l&#39;oggetto Contatto o Account in [!DNL Veeva] CRM.

1. Fare di nuovo clic su **[!UICONTROL Enable Sync]**.

   ![](assets/enable-disable-custom-object-sync-6.png)

1. Tornare alla scheda [!UICONTROL Veeva] e fare clic su **[!UICONTROL Enable Sync]**.

   ![](assets/enable-disable-custom-object-sync-7.png)

## Utilizzo degli oggetti personalizzati {#using-your-custom-objects}

>[!NOTE]
>
>Non è possibile utilizzare oggetti personalizzati nelle campagne intelligenti con trigger.

1. In [!UICONTROL Smart List], trascina il filtro &quot;**[!UICONTROL Has Opportunity]**&quot; e imposta su **[!UICONTROL True]**.

   ![](assets/enable-disable-custom-object-sync-8.png)

1. Facoltativamente, utilizza i vincoli di filtro per restringere lo stato attivo.

   ![](assets/enable-disable-custom-object-sync-9.png)

Eccellente! È ora possibile utilizzare i dati di questo oggetto personalizzato in [!UICONTROL Smart Campaigns] e [!UICONTROL Smart Lists].

>[!MORELIKETHIS]
>
>[Aggiungi/Rimuovi campo oggetto personalizzato come elenco avanzato/vincoli trigger](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target="_blank"}
