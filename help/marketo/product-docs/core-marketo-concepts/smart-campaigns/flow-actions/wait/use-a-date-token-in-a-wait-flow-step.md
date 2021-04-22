---
unique-page-id: 1146997
description: Utilizzare un token di data in un passaggio del flusso di attesa - Documenti Marketo - Documentazione del prodotto
title: Utilizzare un token di data in un passaggio del flusso di attesa
exl-id: d161922b-ce90-4e65-9282-d3bb866c1d94
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---

# Utilizzare un token di data in un passaggio del flusso di attesa {#use-a-date-token-in-a-wait-flow-step}

Puoi utilizzare il passaggio Flusso di attesa per mettere in pausa il percorso di una persona attraverso una campagna intelligente fino a una data specifica che utilizza un token di data. Puoi anche modificare la data di fine di un certo numero di giorni.

>[!NOTE]
>
>Questo vale solo per attivare le campagne. Non è possibile utilizzare questa funzione nelle campagne batch.

1. Nella scheda **Flusso** della campagna intelligente, trascina il passaggio del passaggio di flusso **Attendi**.

   ![](assets/image2014-9-22-14-3a8-3a22.png)

1. Fai clic sull’icona a forma di ingranaggio a destra.

   ![](assets/image2014-9-22-14-3a8-3a37.png)

1. Dal menu a discesa **Tipo**, seleziona **Token di data**.

   ![](assets/image2014-9-22-14-3a8-3a41.png)

1. Scegli un token di data per specificare quando deve terminare il passaggio Attendi :

   * `{{my._____}}`
   * `{{lead.______}}`
   * `{{company.______}}`
   * `{{system._______}}`

   ![](assets/image2014-9-22-14-3a9-3a33.png)

1. Per attendere il prossimo anniversario della data che si verifica nell&#39;anno solare corrente o successivo, seleziona la casella .

   ![](assets/image2014-9-22-14-3a9-3a37.png)

   >[!TIP]
   >
   >Utilizza questa opzione nei token data che fanno riferimento a date passate, ad esempio una data di compleanno o di inizio del contratto.

1. Facoltativamente, puoi modificare la data di fine di un numero specifico di giorni.

   ![](assets/image2014-9-22-14-3a9-3a57.png)

   >[!NOTE]
   >
   >È inoltre possibile specificare il numero di giorni utilizzando un token `{{lead.` o `{{company.` che rappresenta un campo intero o un token `{{my.` di tipo numerico.

1. Fare clic su **Salva**.

   ![](assets/image2014-9-22-14-3a11-3a3.png)

   >[!MORELIKETHIS]
   >
   >* [Utilizzare una durata in un passaggio del flusso di attesa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-duration-in-a-wait-flow-step.md)
   >* [Utilizzare una data specifica in un passaggio del flusso di attesa](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/wait/use-a-specific-date-in-a-wait-flow-step.md)

