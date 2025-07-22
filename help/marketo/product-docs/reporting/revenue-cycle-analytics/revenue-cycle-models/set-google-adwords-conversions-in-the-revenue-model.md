---
unique-page-id: 6095029
description: Imposta [!DNL Google AdWords] conversioni nel modello di ricavi - Documenti Marketo - Documentazione del prodotto
title: Imposta [!DNL Google AdWords] conversioni nel modello di ricavi
exl-id: dd1259fc-d3f2-44ec-8055-f75d55263b36
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 1%

---

# Imposta conversioni [!DNL Google AdWords] nel modello di ricavi {#set-google-adwords-conversions-in-the-revenue-model}

Collega l&#39;account [!DNL Google AdWords] a Marketo per caricare automaticamente i dati di conversione offline da Marketo a [!DNL Google AdWords]. Quindi, dall&#39;interfaccia utente di [!DNL AdWords], potrai vedere facilmente quali clic hanno generato lead qualificati, opportunità e nuovi clienti (o qualsiasi fase dei ricavi desideri monitorare) dopo [aver aggiunto colonne personalizzate](https://support.google.com/adwords/answer/3073556) in [!DNL AdWords].

>[!NOTE]
>
>Questa è un&#39;integrazione push da Marketo a [!DNL Google AdWords]. I dati di conversione verranno visualizzati _only_ nel portale [!DNL Google AdWords], _not nell&#39;interfaccia utente di Marketo_.

Ulteriori informazioni sulla funzione di importazione della conversione offline di [Google](https://support.google.com/adwords/answer/2998031?hl=en). Mappare [!DNL AdWords] conversioni offline in uno o più stadi in un modello dei ricavi. Esistono tre modi per eseguire la mappatura:

* Conversione [!DNL AdWords]
* Azione fase
* Mappatura di [!DNL AdWords]

È possibile creare una nuova conversione offline di [!DNL AdWords] da Marketo se si utilizza Azione stage.

>[!PREREQUISITES]
>
>[Aggiungi [!DNL Google AdWords] come servizio LaunchPoint](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service.md)

## Usa conversione [!DNL AdWords] {#use-adwords-conversion}

1. Passare all&#39;area **[!UICONTROL Analytics]**.

   ![](assets/image2015-2-23-18-3a9-3a34.png)

1. Seleziona un modello.

   ![](assets/image2015-2-23-18-3a3-3a12.png)

1. Fai clic su **[!UICONTROL Edit Draft]**.

   ![](assets/image2015-3-10-15-3a3-3a20.png)

1. Selezionare la fase dei ricavi da mappare a una conversione [!DNL AdWords].

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. Seleziona **[!UICONTROL AdWords Conversion]** da mappare alla tua fase di Marketo.

   ![](assets/image2015-2-26-16-3a46-3a15.png)

   Bello! I dati di conversione di [!DNL AdWords] verranno caricati in [!DNL Google AdWords] alla cadenza selezionata.

## Usa azione fase {#use-stage-action}

È inoltre possibile mappare un [!UICONTROL AdWords Conversion] in **[!UICONTROL Stage Actions]**.

1. Selezionare il passaggio da mappare a una conversione [!DNL AdWords].

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. Nel menu a discesa **[!UICONTROL Stage Actions]**, seleziona **[!UICONTROL Set AdWords Conversion]**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Selezionare un **[!UICONTROL AdWords Conversion]**.

   ![](assets/image2015-2-26-16-3a54-3a47.png)

   **Suggerimento**: se non hai conversioni [!DNL AdWords], creane una facendo clic su **[!UICONTROL +New Conversion]**.

   ![](assets/image2015-2-26-21-3a22-3a10.png)

1. Fai clic su **[!UICONTROL Save]**.

   ![](assets/image2015-2-26-16-3a56-3a2.png)

1. Dopo aver completato la mappatura di tutte le conversioni di [!DNL AdWords] in fasi di ricavi, torna alla pagina di riepilogo. Selezionare **[!UICONTROL Model Actions]** e scegliere **[!UICONTROL Approve Stages]**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

## Suggerimento pro: aggiungi una nuova conversione {#pro-tip-add-a-new-conversion}

Suggerimento pro! È possibile creare una nuova conversione offline di [!DNL AdWords] da Marketo.

>[!CAUTION]
>
>Per le nuove conversioni create da Marketo, l’impostazione &quot;ottimizzazione&quot; è abilitata. Ciò significa che le strategie di offerta di [!DNL AdWords] possono ottimizzare le offerte per tali conversioni. È possibile modificare questa impostazione dall&#39;account [!DNL AdWords].

1. Nel menu a discesa **[!UICONTROL Stage Actions]**, seleziona **[!UICONTROL Set AdWords Conversion]**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Seleziona **[!UICONTROL New Conversion]**.

   ![](assets/image2015-2-26-21-3a22-3a10.png)

1. Immetti **[!UICONTROL Conversion Name]**. Fai clic su **[!UICONTROL Save]**.

   ![](assets/image2015-2-26-21-3a24-3a7.png)

   Eccellente! Questa nuova conversione verrà visualizzata nel tuo account [!DNL AdWords].

## Usa mappatura [!DNL AdWords] {#use-adwords-mapping}

È possibile associare tutte le fasi del modello a [!UICONTROL AdWords Conversion] in un&#39;unica posizione utilizzando [!DNL AdWords] Mapping.

1. Seleziona **[!UICONTROL Edit AdWords Mappings]**.

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. Selezionare il **[!UICONTROL AdWords Conversion]** desiderato per ogni fase che si desidera monitorare.

   ![](assets/image2015-2-26-17-3a6-3a15.png)

1. Dopo aver mappato le fasi, fare clic su **[!UICONTROL Save]**.

   ![](assets/image2015-2-26-17-3a7-3a48.png)

1. Dopo aver completato la mappatura di tutte le conversioni di [!DNL AdWords] in fasi di ricavi, torna alla pagina di riepilogo. Selezionare **[!UICONTROL Model Actions]** e scegliere **[!UICONTROL Approve Stages]**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

Per visualizzare i dati di conversione offline, dovrai accedere al tuo account [!DNL AdWords]. È consigliabile utilizzare la funzionalità [Colonne personalizzate](https://support.google.com/adwords/answer/3073556) per creare colonne di conteggio delle conversioni per ogni conversione offline importata da Marketo.
