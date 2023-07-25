---
unique-page-id: 1146978
description: Utilizzare una durata in un passaggio del flusso di attesa - Documentazione di Marketo - Documentazione del prodotto
title: Utilizzare una durata in un passaggio del flusso di attesa
exl-id: 7b13d225-78ba-4ef1-9ff5-0f6acde6e5ff
feature: Smart Campaigns
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 0%

---

# Utilizzare una durata in un passaggio del flusso di attesa {#use-a-duration-in-a-wait-flow-step}

Puoi utilizzare il passaggio Flusso di attesa per mettere in pausa il percorso di una persona in una campagna intelligente per un certo periodo di tempo. Puoi anche specificare i criteri per il giorno della settimana e l’ora in cui termina.

1. Nella tua campagna intelligente **Flusso** , trascina sulla scheda **Wait** passaggio di flusso.

   ![](assets/image2014-9-22-11-3a53-3a57.png)

1. Immetti per quanto tempo desideri sospendere l’operazione.

   ![](assets/image2014-9-22-11-3a54-3a0.png)

1. Tutto qui! Il flusso verrà messo in pausa per la durata specificata. Per opzioni avanzate, fai clic sull’icona a forma di ingranaggio a destra.

   ![](assets/image2014-9-22-11-3a54-3a7.png)

1. Specifica il giorno della settimana in cui deve terminare il passaggio di attesa.

   ![](assets/image2014-9-22-11-3a54-3a10.png)

1. Facoltativamente, specifica l’ora. Clic **Salva**.

   ![](assets/image2014-9-22-11-3a54-3a35.png)

   >[!NOTE]
   >
   >**Esempio**
   >
   >Una persona attiva una campagna intelligente venerdì alle 17. Il passaggio di attesa è avanzato: 48 ore e deve terminare il lunedì-venerdì alle 9.
   >
   >Il risultato sarebbe che la persona avrebbe continuato nel flusso su **Lunedì, ore 9**. Questa è la prima data M-F dopo 48 ore.

   >[!NOTE]
   >
   >La durata, le date, le ore e i giorni utilizzati dipendono dal fuso orario dell’abbonamento.

   >[!MORELIKETHIS]
   >
   >* [Utilizzare una data specifica in un passaggio del flusso di attesa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md)
   >* [Utilizzare un token di data in un passaggio del flusso di attesa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-date-token-in-a-wait-flow-step.md)
