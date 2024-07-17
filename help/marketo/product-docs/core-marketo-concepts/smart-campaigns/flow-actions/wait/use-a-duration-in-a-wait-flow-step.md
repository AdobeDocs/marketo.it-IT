---
unique-page-id: 1146978
description: Utilizzare una durata in un passaggio del flusso di attesa - Documentazione di Marketo - Documentazione del prodotto
title: Utilizzare una durata in un passaggio del flusso di attesa
exl-id: 7b13d225-78ba-4ef1-9ff5-0f6acde6e5ff
feature: Smart Campaigns
source-git-commit: 12f2399859c784095cc2c1df772c66c649106ba3
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 0%

---

# Utilizzare una durata in un passaggio del flusso di attesa {#use-a-duration-in-a-wait-flow-step}

Puoi utilizzare il passaggio Flusso di attesa per mettere in pausa il percorso di una persona in una campagna avanzata per un certo periodo di tempo. Puoi anche specificare i criteri per il giorno della settimana e l’ora in cui termina.

1. Nella scheda **[!UICONTROL Flusso]** della campagna avanzata, trascina il passaggio del flusso **[!UICONTROL Attendi]**.

   ![](assets/use-a-duration-in-a-wait-flow-step-1.png)

1. Immetti per quanto tempo desideri sospendere l’operazione.

   ![](assets/use-a-duration-in-a-wait-flow-step-2.png)

1. Tutto qui! Il flusso verrà messo in pausa per la durata specificata. Per opzioni avanzate, fai clic sull’icona a forma di ingranaggio a destra.

   ![](assets/use-a-duration-in-a-wait-flow-step-3.png)

1. Specifica il giorno della settimana in cui deve terminare il passaggio di attesa.

   ![](assets/use-a-duration-in-a-wait-flow-step-4.png)

1. Facoltativamente, specifica l’ora. Fai clic su **[!UICONTROL Salva]**.

   ![](assets/use-a-duration-in-a-wait-flow-step-5.png)

   >[!NOTE]
   >
   >**Esempio**
   >
   >Una persona attiva una campagna intelligente venerdì alle 17. Il passaggio di attesa è avanzato: 48 ore e deve terminare il lunedì-venerdì alle 9.
   >
   >Il risultato è che la persona continuerà nel flusso il **lunedì, 9**. Questa è la prima data M-F dopo 48 ore.

   >[!NOTE]
   >
   >La durata, le date, le ore e i giorni utilizzati dipendono dal fuso orario dell’abbonamento.

   >[!MORELIKETHIS]
   >
   >* [Utilizzare una data specifica in un passaggio del flusso di attesa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md){target="_blank"}
   >* [Utilizzare un token di data in un passaggio del flusso di attesa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-date-token-in-a-wait-flow-step.md){target="_blank"}
