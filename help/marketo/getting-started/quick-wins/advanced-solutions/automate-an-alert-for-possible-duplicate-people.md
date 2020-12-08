---
unique-page-id: 7513680
description: Automatizzare un avviso per possibili duplicati di persone - Documenti Marketo - Documentazione prodotto
title: Automatizzare un avviso per eventuali persone duplicate
translation-type: tm+mt
source-git-commit: 3c24395e55c756184615941327e15e050fa7d0ac
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---


# Automatizzare un avviso per eventuali persone duplicate {#automate-an-alert-for-possible-duplicate-people}

Vuoi un avviso ogni volta che è possibile creare una persona duplicata? Ecco come impostare una Smart Campaign per farlo.

>[!NOTE]
>
>**FYI**
>
>Marketo sta standardizzando la lingua tra tutte le iscrizioni, pertanto è possibile che nell&#39;abbonamento siano presenti lead/lead e persone in docs.marketo.com. Questi termini significano la stessa cosa; non influisce sulle istruzioni dell&#39;articolo. Ci sono anche altri cambiamenti. [Ulteriori](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)informazioni.

1. [Create una nuova campagna](../../../product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md)intelligente. Definire il seguente elenco di smart:

   * Trigger: **Persona creata**
   * Filtro: **Duplica campi. **Il nome del campo **è** **Nome** completo.

   ![](assets/image2017-3-27-8-3a22-3a4.png)

   >[!TIP]
   >
   >Siate creativi. Sperimentate con campi diversi per ottenere risultati di filtraggio migliori.

1. Nel passaggio del flusso, scegliete [Invia azione flusso avvisi](../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md) .

   ![](assets/image2017-3-27-8-3a24-3a8.png)

   >[!TIP]
   >
   >Utilizzo del token [](../../../product-docs/email-marketing/general/using-tokens/use-the-send-alert-info-token.md) Invia informazioni avviso per includere un collegamento alla persona in CRM.

   >[!CAUTION]
   >
   >Se importate un elenco di grandi dimensioni, potreste ricevere una serie di avvisi contemporaneamente!
   >
   >
   >Inoltre, due persone con lo stesso nome non significa automaticamente che sono la stessa persona.

1. Attivate la campagna nella scheda **Pianificazione** .

   ![](assets/image2017-3-27-8-3a24-3a37.png)

È tutto! Questa campagna intelligente verrà attivata ogni volta che viene creata una nuova persona con un nome completo esistente in Marketo.

>[!MORELIKETHIS]
>
>* [Trova e unisci persone duplicate](../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md)

