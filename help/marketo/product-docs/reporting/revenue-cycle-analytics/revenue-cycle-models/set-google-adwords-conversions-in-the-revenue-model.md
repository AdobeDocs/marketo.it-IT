---
unique-page-id: 6095029
description: Impostare le conversioni di Google AdWords nel modello di ricavo - Documenti Marketo - Documentazione del prodotto
title: Impostare le conversioni di Google AdWords nel modello dei ricavi
exl-id: dd1259fc-d3f2-44ec-8055-f75d55263b36
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 0%

---

# Impostare le conversioni di Google AdWords nel modello dei ricavi {#set-google-adwords-conversions-in-the-revenue-model}

Collega il tuo account Google AdWords a Marketo per caricare automaticamente i dati di conversione offline da Marketo a Google AdWords. Quindi, dall’interfaccia utente di AdWords, potrai vedere facilmente quali clic hanno generato lead qualificati, opportunità e nuovi clienti (o qualsiasi fase dei ricavi desideri monitorare) dopo di te [aggiungere colonne personalizzate](https://support.google.com/adwords/answer/3073556) in AdWords.

>[!NOTE]
>
>Si tratta di un’integrazione push da Marketo a Google AdWords. Verranno visualizzati i dati di conversione _solo_ nel portale Google AdWords, _non nell’interfaccia utente di Marketo_.

Ulteriori informazioni su [Funzione di importazione della conversione offline di Google](https://support.google.com/adwords/answer/2998031?hl=en). Mappa le conversioni offline di AdWords in uno o più stadi in un modello Revenue (Entrate). Esistono tre modi per eseguire la mappatura:

* Conversione AdWords
* Azione fase
* Mappatura AdWords

Puoi creare una nuova conversione offline di AdWords da Marketo se utilizzi Azione stage.

>[!PREREQUISITES]
>
>[Aggiungere Google AdWords come servizio LaunchPoint](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service.md)

## Usa conversione AdWords {#use-adwords-conversion}

1. Vai a **Analytics** area.

   ![](assets/image2015-2-23-18-3a9-3a34.png)

1. Seleziona un modello.

   ![](assets/image2015-2-23-18-3a3-3a12.png)

1. Clic **Modifica bozza**.

   ![](assets/image2015-3-10-15-3a3-3a20.png)

1. Seleziona la fase dei ricavi da mappare a una conversione AdWords.

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. Seleziona la **Conversione AdWords** si desidera eseguire la mappatura sulla fase Marketo.

   ![](assets/image2015-2-26-16-3a46-3a15.png)

   Bello! I dati di conversione di AdWords verranno caricati sul tuo Google AdWords alla cadenza selezionata.

## Usa azione fase {#use-stage-action}

Puoi anche mappare una conversione AdWords in Azioni stage.

1. Seleziona il passaggio da mappare a una conversione AdWords.

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. Sotto **Azioni fase** a discesa, seleziona **Imposta conversione AdWords**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Seleziona un **Conversione AdWords**.

   ![](assets/image2015-2-26-16-3a54-3a47.png)

   **Suggerimento**: se non hai conversioni AdWords, creane una facendo clic su **+Nuova conversione**.

   ![](assets/image2015-2-26-21-3a22-3a10.png)

1. Clic **Salva**.

   ![](assets/image2015-2-26-16-3a56-3a2.png)

1. Dopo aver completato la mappatura di tutte le conversioni AdWords nelle fasi dei ricavi, torna alla pagina di riepilogo. Seleziona **Azioni modello** e scegli **Approva fasi**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

## Suggerimento pro: aggiungi una nuova conversione {#pro-tip-add-a-new-conversion}

Suggerimento pro! È possibile creare una nuova conversione offline AdWords da Marketo.

>[!CAUTION]
>
>Per le nuove conversioni create da Marketo, l’impostazione &quot;ottimizzazione&quot; è abilitata. Ciò significa che le strategie di offerta di AdWords possono ottimizzare le offerte per tali conversioni. Puoi modificare questa impostazione dal tuo account AdWords.

1. Sotto **Azioni fase** a discesa, seleziona **Imposta conversione AdWords**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Seleziona **Nuova conversione**.

   ![](assets/image2015-2-26-21-3a22-3a10.png)

1. Immetti un **Nome conversione**. Clic **Salva**.

   ![](assets/image2015-2-26-21-3a24-3a7.png)

   Eccellente! Questa nuova conversione verrà visualizzata nel tuo account AdWords.

## Usa mappatura AdWords {#use-adwords-mapping}

È possibile associare tutte le fasi del modello alla conversione AdWords in un&#39;unica posizione utilizzando le mappature AdWords.

1. Seleziona **Modifica mappature AdWords**.

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. Seleziona il **Conversione AdWords** per ogni fase che si desidera monitorare.

   ![](assets/image2015-2-26-17-3a6-3a15.png)

1. Dopo aver mappato le fasi, fai clic su **Salva**.

   ![](assets/image2015-2-26-17-3a7-3a48.png)

1. Dopo aver completato la mappatura di tutte le conversioni AdWords nelle fasi dei ricavi, torna alla pagina di riepilogo. Seleziona **Azioni modello** e scegli **Approva fasi**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

Per visualizzare i dati di conversione offline, dovrai accedere al tuo account AdWords. Si consiglia di utilizzare i [Funzione Colonne personalizzate](https://support.google.com/adwords/answer/3073556) per creare colonne di conteggio delle conversioni per ogni conversione offline importata da Marketo.
