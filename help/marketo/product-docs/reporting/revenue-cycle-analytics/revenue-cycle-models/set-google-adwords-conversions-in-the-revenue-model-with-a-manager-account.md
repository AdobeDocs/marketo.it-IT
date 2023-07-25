---
unique-page-id: 7504923
description: Impostare le conversioni di Google AdWords nel modello dei ricavi con un account Manager - Documenti Marketo - Documentazione del prodotto
title: Impostare le conversioni di Google AdWords nel modello dei ricavi con un account Manager
exl-id: 8c9f50cf-0a8b-4f9a-a0bd-bb57eeac24cf
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 0%

---

# Impostare le conversioni di Google AdWords nel modello dei ricavi con un account Manager {#set-google-adwords-conversions-in-the-revenue-model-with-a-manager-account}

Collega il tuo account Google AdWords a Marketo per caricare automaticamente i dati di conversione offline da Marketo a Google AdWords. Quindi, dall’interfaccia utente di AdWords, potrai vedere facilmente quali clic hanno generato lead qualificati, opportunità e nuovi clienti (o qualsiasi fase dei ricavi desideri monitorare) dopo di te [aggiungere colonne personalizzate](https://support.google.com/adwords/answer/3073556) in AdWords.

Se si dispone di più account Google Adwords, è possibile utilizzare un [Account Google AdWords Manager](https://www.google.com/adwords/manager-accounts/) (precedentemente noto come My Client Center) per integrarli con Marketo.

Puoi mappare le conversioni offline di AdWords in uno o più stadi in un modello Revenue. Esistono due modi:

* Azione fase
* Mappatura AdWords

>[!PREREQUISITES]
>
>[Aggiungere Google AdWords as a Launchpoint Service con un account Manager](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service-with-a-manager-account.md)

## Usa azione fase {#use-stage-action}

Mappa una conversione AdWords nelle azioni stage.

1. Seleziona il passaggio da mappare a una conversione AdWords.

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. Sotto **Azioni fase** a discesa, seleziona **Imposta conversione AdWords**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Imposta un **Conversione AdWords**.

   >[!NOTE]
   >
   >È possibile selezionare una conversione AdWords diversa per ogni account secondario.

   ![](assets/image2015-3-27-17-3a16-3a37.png)

   Suggerimento: se non hai conversioni AdWords, creane una facendo clic su **+Nuova conversione**.

   ![](assets/image2015-3-27-17-3a18-3a58.png)

1. Clic **Salva**.

   ![](assets/image2015-3-27-17-3a21-3a15.png)

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

   ![](assets/image2015-3-27-17-3a23-3a13.png)

1. Immetti un **Nome conversione**. Clic **Salva**.

   ![](assets/image2015-3-27-17-3a24-3a49.png)

   Eccellente! Questa nuova conversione verrà visualizzata nel tuo account AdWords.

## Usa mappatura AdWords {#use-adwords-mapping}

È possibile associare tutte le fasi del modello alla conversione AdWords in un&#39;unica posizione utilizzando le mappature AdWords.

1. Seleziona **Modifica mappature AdWords**.

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. Seleziona il **Account AdWords** e desiderato **Conversione AdWords** per ogni fase che si desidera monitorare.

   ![](assets/image2015-3-27-17-3a30-3a15.png)

1. Dopo aver mappato le fasi, fai clic su **Salva**.

   ![](assets/image2015-3-27-17-3a30-3a48.png)

1. Dopo aver completato la mappatura di tutte le conversioni AdWords nelle fasi dei ricavi, torna alla pagina di riepilogo. Seleziona **Azioni modello** e scegli **Approva fasi**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

Per visualizzare i dati di conversione offline, dovrai accedere al tuo account AdWords. Si consiglia di utilizzare i [Funzione Colonne personalizzate](https://support.google.com/adwords/answer/3073556) per creare colonne di conteggio delle conversioni per ogni conversione offline importata da Marketo.
