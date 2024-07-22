---
unique-page-id: 2360421
description: Sostituire il comportamento di Analytics a livello di programma - Documentazione di Marketo - Documentazione del prodotto
title: Sostituire il comportamento di Analytics a livello di programma
exl-id: 2fd86279-99ae-494d-a6f8-2572b7dcd892
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '192'
ht-degree: 1%

---

# Sostituire il comportamento di Analytics a livello di programma {#override-analytics-behavior-at-the-program-level}

È possibile impostare il comportamento di [analisi a livello di amministratore sui canali](/help/marketo/product-docs/reporting/revenue-cycle-analytics/program-analytics/make-a-program-without-a-period-cost-available-in-revenue-explorer-and-analyzers.md), ma è anche possibile ignorarlo a livello di programma. Ecco come:

1. Vai all&#39;area **Attività di marketing**.

   ![](assets/image2014-9-24-11-3a40-3a46.png)

1. Individuare e selezionare il programma.

   ![](assets/image2014-9-24-11-3a40-3a57.png)

1. Nella scheda **Configurazione**, trascina Comportamento di Analytics nell&#39;area di lavoro.

   ![](assets/image2014-9-24-11-3a41-3a2.png)

1. Seleziona il comportamento di Analytics desiderato.

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

1. Fai clic su **Salva**.

   ![](assets/image2014-9-24-11-3a42-3a6.png)

Ben fatto! Ora sai come ignorare il comportamento di analisi a livello di programma.

>[!NOTE]
>
>Le modifiche avranno effetto il giorno successivo e saranno rese disponibili o estratte dagli analizzatori ed esploratori di ricavi.
