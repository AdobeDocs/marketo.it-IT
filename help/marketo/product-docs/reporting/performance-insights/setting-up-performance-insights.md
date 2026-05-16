---
unique-page-id: 12981145
description: Scopri come impostare Performance Insights configurando la configurazione delle opportunità, i costi del programma, il comportamento delle analisi e i criteri di successo. Assicurati che l’attribuzione e il flusso di dati siano corretti per una generazione di rapporti accurata.
title: Impostazione di approfondimenti prestazioni
exl-id: f87bbaba-c2c1-4b83-9e07-f8a5d1f1738b
feature: Reporting
TQID: https://experienceleague.adobe.com/xH9HG3hKoUFG3428IngBYFG6n4W3k1Bd-baVI7WTMrE
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: c5f60233-d5ea-4453-a799-0ad258b4d399id: e64968b2-4ee5-47f9-8cae-0588f184b9ebid: ea90ebee-5c84-42d9-8b21-006bdabc95a3
subfeature_v2: id: b9f06cb0-cdf7-4b83-a9d1-a701d132779b
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: e1e0219c-f879-479f-8427-888ed2a6e9c2
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 298
ht-degree: 4%

---

# Configurazione di [!UICONTROL Performance Insights] {#setting-up-performance-insights}

Segui i passaggi seguenti per impostare MPI.

## Configurazione dell’opportunità {#opportunity-setup}

1. Fai clic su **[!UICONTROL Admin]**.

   ![](assets/admin.png)

1. Fai clic su **[!UICONTROL Revenue Cycle Analytics]**.

   ![](assets/two-2.png)

   >[!NOTE]
   >
   >Se non si dispone di RCA, è necessario selezionare **[!UICONTROL Program Analysis]** per il passaggio 2.

1. In Attribution, fare clic su **[!UICONTROL Edit]**.

   ![](assets/three-1.png)

1. Vengono visualizzate le impostazioni di attribuzione.

   ![](assets/four-2.png)

   Se l’attribuzione è esplicita, assicurati che il ruolo di contatto dell’opportunità sia stato popolato (tramite l’endpoint &quot;Opportunity Role&quot; o tramite l’integrazione CRM).

   Se l’attribuzione è implicita, assicurati che il campo aziendale sul lead/contatto corrisponda al Nome account dell’opportunità.

   >[!NOTE]
   >
   >Assicurati che tutte le opportunità siano compilate nei campi appropriati:
   >
   >* [!UICONTROL Opportunity Amount]
   >* [!UICONTROL Is Closed]
   >* [!UICONTROL Is Won]
   >* [!UICONTROL Creation Date] (potrebbe non essere impostato nel tuo caso)
   >* [!UICONTROL Closed Date] (potrebbe non essere impostato nel tuo caso)
   >* [!UICONTROL Opportunity Type]

## Configurazione del programma {#program-setup}

Aggiornare i costi del programma per almeno 12 mesi. Puoi farlo manualmente o utilizzando l’API del programma. In questo esempio lo facciamo manualmente.

1. Fai clic su **[!UICONTROL Marketing Activities]**.

   ![](assets/ma.png)

1. Individuare e selezionare il programma.

   ![](assets/select-program.png)

1. Fai clic sulla scheda **[!UICONTROL Setup]**.

   ![](assets/setup-tab.png)

1. Trascina **[!UICONTROL Period Cost]** nell&#39;area di lavoro.

   ![](assets/period-cost.png)

1. Impostare il mese del programma per almeno 12 mesi fa e fare clic su **[!UICONTROL Ok]**.

   ![](assets/set-period.png)

1. Impostare il costo del periodo e fare clic su **[!UICONTROL Save]**.

   ![](assets/set-cost.png)

Quindi, rivedi il comportamento di analisi per indicare se un particolare canale deve essere incluso nell’analisi. Imposta il comportamento di Analytics (Normale, Inclusivo, Operativo).

1. Fai clic su **[!UICONTROL Admin]**.

   ![](assets/admin.png)

1. Fai clic su **[!UICONTROL Tags]**.

   ![](assets/tags.png)

1. Fare clic su **+** per espandere l&#39;elenco dei canali.

   ![](assets/channel.png)

1. Fare doppio clic sul canale desiderato.

   ![](assets/channel-click.png)

1. Fare clic sul menu a discesa **[!UICONTROL Analytics Behavior]** e selezionare il comportamento desiderato.

   ![](assets/edit-channel.png)

1. Imposta i criteri di successo.

   ![](assets/success.png)

1. Fai clic su **[!UICONTROL Save]**.

   ![](assets/save.png)

## Collega il programma alla persona {#tie-the-program-to-the-person}

1. Assicurati che il programma di acquisizione e la data di acquisizione siano stati impostati per ogni persona nel database affinché l’attribuzione del primo contatto funzioni.
1. Assicurati che i tuoi programmi impostino gli stati di successo per le tue persone.

>[!NOTE]
>
>Le modifiche apportate non sono istantanee. È necessario un periodo overnight prima che le modifiche diventino effettive.
