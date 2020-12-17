---
unique-page-id: 7513680
description: Automatizzare un avviso per possibili duplicati di persone - Documenti Marketo - Documentazione prodotto
title: Automatizzare un avviso per eventuali persone duplicate
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 0%

---


# Automatizzare un avviso per le possibili persone duplicate {#automate-an-alert-for-possible-duplicate-people}

Vuoi un avviso ogni volta che è possibile creare una persona duplicata? Ecco come impostare una Smart Campaign per farlo.

1. [Create una nuova campagna](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md) intelligente. Definire il seguente elenco di smart:

* Trigger: **La persona viene creata**
* Filtro: **Campi duplicati.** Nome campo  **completo**

   ![](assets/image2017-3-27-8-3a22-3a4.png)

   >[!TIP]
   >
   >Siate creativi. Sperimentate con campi diversi per ottenere risultati di filtraggio migliori.

1. Nella fase di flusso, scegliere l&#39;azione di flusso [Invia avviso](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md).

   ![](assets/image2017-3-27-8-3a24-3a8.png)

   >[!TIP]
   >
   >Utilizzo del [token di invio delle informazioni di avviso](/help/marketo/product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md) per includere un collegamento alla persona nel CRM.

   >[!CAUTION]
   >
   >Se importate un elenco di grandi dimensioni, potreste ricevere una serie di avvisi contemporaneamente!
   >
   >Inoltre, due persone con lo stesso nome non significa automaticamente che sono la stessa persona.

1. Attivare la campagna nella scheda **Schedule**.

   ![](assets/image2017-3-27-8-3a24-3a37.png)

È tutto! Questa campagna intelligente verrà attivata ogni volta che viene creata una nuova persona con un nome completo esistente in Marketo.

>[!MORELIKETHIS]
>
>[Trova e unisci persone duplicate](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md)
