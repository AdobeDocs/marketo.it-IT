---
unique-page-id: 1146997
description: Utilizzare un token di data in un passaggio del flusso di attesa - Documentazione di Marketo - Documentazione del prodotto
title: Utilizzare un token di data in un passaggio del flusso di attesa
exl-id: d161922b-ce90-4e65-9282-d3bb866c1d94
feature: Smart Campaigns
source-git-commit: 2eeb7ea7fd43ba75a3c802a91ce07c90dc8abd91
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---

# Utilizzare un token di data in un passaggio del flusso di attesa {#use-a-date-token-in-a-wait-flow-step}

Puoi utilizzare il passaggio del flusso di attesa per mettere in pausa il percorso di una persona tramite una campagna avanzata fino a una data particolare che utilizza un token di data. Puoi anche modificare la data di fine di un certo numero di giorni.

>[!NOTE]
>
>Questo si applica solo alle campagne Trigger. Non è possibile utilizzare questa funzione nelle campagne batch.

1. Nella tua Smart Campaign **[!UICONTROL Flusso]** , trascina sulla scheda **[!UICONTROL Wait]** passaggio di flusso.

   ![](assets/image2014-9-22-14-3a8-3a22.png)

1. Fai clic sull’icona a forma di ingranaggio.

   ![](assets/image2014-9-22-14-3a8-3a37.png)

1. Dalla sezione **[!UICONTROL Tipo]** a discesa, seleziona **[!UICONTROL Token data]**.

   ![](assets/image2014-9-22-14-3a8-3a41.png)

1. Scegli un token di data per specificare quando deve terminare il passaggio Attendi:

   * `{{my._____}}`
   * `{{lead.______}}`
   * `{{company.______}}`
   * `{{system._______}}`

   ![](assets/image2014-9-22-14-3a9-3a33.png)

1. Per attendere fino al prossimo anniversario della data che si verifica nell&#39;anno di calendario corrente o successivo, seleziona la casella.

   ![](assets/image2014-9-22-14-3a9-3a37.png)

   >[!TIP]
   >
   >Utilizza questa opzione sui token di data che fanno riferimento a date precedenti, ad esempio un compleanno o una data di inizio contratto.

1. Facoltativamente, è possibile modificare la data di fine di un numero specificato di giorni.

   ![](assets/image2014-9-22-14-3a9-3a57.png)

   >[!NOTE]
   >
   >È inoltre possibile specificare il numero di giorni utilizzando una `{{lead.` o `{{company.` token che rappresenta un campo intero o un `{{my.` token di tipo numero.

1. Fai clic su **[!UICONTROL Salva]**.

   ![](assets/image2014-9-22-14-3a11-3a3.png)

   >[!MORELIKETHIS]
   >
   >* [Utilizzare una durata in un passaggio del flusso di attesa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-duration-in-a-wait-flow-step.md){target="_blank"}
   >* [Utilizzare una data specifica in un passaggio del flusso di attesa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md){target="_blank"}
