---
unique-page-id: 2360421
description: Sostituire il comportamento di Analytics a livello di programma - Documentazione di Marketo - Documentazione del prodotto
title: Sostituire il comportamento di analisi a livello di programma
exl-id: 2fd86279-99ae-494d-a6f8-2572b7dcd892
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 10%

---

# Sostituire il comportamento di analisi a livello di programma {#override-analytics-behavior-at-the-program-level}

È possibile impostare il comportamento di [analisi a livello di amministratore sui canali](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/make-a-program-without-a-period-cost-available-in-revenue-explorer-and-analyzers.md), ma è anche possibile ignorarlo a livello di programma. Ecco come:

1. Passa alla schermata **[!UICONTROL Marketing Activities]**.

   ![](assets/image2014-9-24-11-3a40-3a46.png)

1. Individuare e selezionare il programma.

   ![](assets/image2014-9-24-11-3a40-3a57.png)

1. Nella scheda **[!UICONTROL Setup]**, trascina [!UICONTROL Analytics Behavior] nell&#39;area di lavoro.

   ![](assets/image2014-9-24-11-3a41-3a2.png)

1. Selezionare [!UICONTROL Analytics Behavior] desiderato.

   >[!NOTE]
   >
   >**Definizione**
   >
   >* **Inclusivo** - Questa opzione garantisce che il programma sia disponibile per la generazione di rapporti in Esplora ricavi e analizzatori, indipendentemente dal fatto che sia stato incluso o meno un costo del periodo.
   >* **Operativo** - Con questa opzione il programma non viene visualizzato in Esplora ricavi o negli analizzatori.

   >[!NOTE]
   >
   >Il comportamento predefinito (se questa impostazione non viene applicata) è che il programma verrà incluso in Analytics **SOLO se è presente almeno un costo periodo**, anche uno a cui sono assegnati zero dollari.

   ![](assets/image2014-9-24-11-3a42-3a0.png)

1. Fai clic su **[!UICONTROL Save]**.

   ![](assets/image2014-9-24-11-3a42-3a6.png)

Ben fatto! Ora sai come ignorare il comportamento di analisi a livello di programma.

>[!NOTE]
>
>Le modifiche avranno effetto il giorno successivo e saranno rese disponibili o estratte dagli analizzatori ed esploratori di ricavi.
