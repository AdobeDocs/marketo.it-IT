---
unique-page-id: 1146997
description: Utilizzare un token di data in un passaggio del flusso di attesa - Documentazione di Marketo - Documentazione del prodotto
title: Utilizzare un token di data in un passaggio del flusso di attesa
exl-id: d161922b-ce90-4e65-9282-d3bb866c1d94
feature: Smart Campaigns
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 0%

---

# Utilizzare un token di data in un passaggio del flusso di attesa {#use-a-date-token-in-a-wait-flow-step}

Puoi utilizzare il passaggio del flusso di attesa per mettere in pausa il percorso di una persona tramite una campagna avanzata fino a una data particolare che utilizza un token di data. Puoi anche modificare la data di fine di un certo numero di giorni.

>[!NOTE]
>
>Questo si applica solo alle campagne Trigger. Non è possibile utilizzare questa funzione nelle campagne batch.

1. Nella scheda **[!UICONTROL Flow]** di Smart Campaign, trascina sul passaggio di flusso **[!UICONTROL Wait]**.

   ![](assets/use-a-date-token-in-a-wait-flow-step-1.png)

1. Fai clic sull’icona a forma di ingranaggio.

   ![](assets/use-a-date-token-in-a-wait-flow-step-2.png)

1. Dall&#39;elenco a discesa **[!UICONTROL Type]**, selezionare **[!UICONTROL Date Token]**.

   ![](assets/use-a-date-token-in-a-wait-flow-step-3.png)

1. Scegli un [!UICONTROL Date token] per specificare quando deve terminare il passaggio Attendi:

   * `{{my._____}}`
   * `{{lead.______}}`
   * `{{company.______}}`
   * `{{system._______}}`

   ![](assets/use-a-date-token-in-a-wait-flow-step-4.png)

1. Per attendere fino al prossimo anniversario della data che si verifica nell&#39;anno di calendario corrente o successivo, seleziona la casella.

   ![](assets/use-a-date-token-in-a-wait-flow-step-5.png)

   >[!TIP]
   >
   >Utilizza questa opzione sui token di data che fanno riferimento a date precedenti, ad esempio un compleanno o una data di inizio contratto.

1. Facoltativamente, è possibile modificare la data di fine di un numero specificato di giorni.

   ![](assets/use-a-date-token-in-a-wait-flow-step-6.png)

   >[!NOTE]
   >
   >È inoltre possibile specificare il numero di giorni utilizzando un token `{{lead.` o `{{company.` che rappresenta un campo intero o un token `{{my.` di tipo numero.

1. Fai clic su **[!UICONTROL Save]**.

   ![](assets/use-a-date-token-in-a-wait-flow-step-7.png)

   >[!MORELIKETHIS]
   >
   >* [Utilizzare una durata in un passaggio del flusso di attesa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-duration-in-a-wait-flow-step.md){target="_blank"}
   >* [Utilizzare una data specifica in un passaggio del flusso di attesa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md){target="_blank"}
