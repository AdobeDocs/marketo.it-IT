---
unique-page-id: 7504923
description: Impostare le conversioni Google AdWords nel modello dei ricavi con un account manager - Marketo Docs - Documentazione del prodotto
title: Impostare le conversioni Google AdWords nel modello dei ricavi con un account manager
exl-id: 8c9f50cf-0a8b-4f9a-a0bd-bb57eeac24cf
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 0%

---

# Impostare le conversioni Google AdWords nel modello dei ricavi con un account manager {#set-google-adwords-conversions-in-the-revenue-model-with-a-manager-account}

Collega il tuo account Google AdWords a Marketo per caricare automaticamente i dati di conversione offline da Marketo a Google AdWords. Quindi, dall’interfaccia utente di AdWords, potrai vedere facilmente quali clic hanno portato a lead qualificati, opportunità e nuovi clienti (o qualsiasi fase di ricavo desideri monitorare) dopo aver [aggiungere colonne personalizzate](https://support.google.com/adwords/answer/3073556) in AdWords.

Se disponi di più account Google Adwords, puoi utilizzare un [Account Google AdWords Manager](https://www.google.com/adwords/manager-accounts/) (precedentemente noto come Centro client personale) per integrarli con Marketo.

Puoi mappare le conversioni offline di AdWords su uno o più stadi in un modello Revenue. Esistono due modi:

* Azione fase
* Mappatura di AdWords

>[!PREREQUISITES]
>
>[Aggiungere Google AdWords as a Launchpoint Service con un account Manager](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service-with-a-manager-account.md)

## Usa azione fase {#use-stage-action}

Mappare una conversione AdWords in Azioni stage .

1. Seleziona il passaggio da mappare a una conversione AdWords.

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. Sotto la **Azioni stage** a discesa, seleziona **Imposta conversione AdWords**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Imposta un **Conversione AdWords**.

   >[!NOTE]
   >
   >Per ogni account figlio è possibile selezionare una conversione AdWords diversa.

   ![](assets/image2015-3-27-17-3a16-3a37.png)

   Suggerimento: Se non hai conversioni AdWords, creane una facendo clic su **+Nuova conversione**.

   ![](assets/image2015-3-27-17-3a18-3a58.png)

1. Fai clic su **Salva**.

   ![](assets/image2015-3-27-17-3a21-3a15.png)

1. Dopo aver mappato tutte le conversioni di AdWords nelle fasi di ricavo, torna alla pagina di riepilogo. Seleziona **Azioni modello** e scegli **Approva fasi**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

## Consiglio Pro: Aggiungi una nuova conversione {#pro-tip-add-a-new-conversion}

Consiglio! Da Marketo è possibile creare una nuova conversione offline AdWords.

>[!CAUTION]
>
>Le nuove conversioni create da Marketo dispongono dell’impostazione &quot;ottimizzazione&quot; abilitata. Ciò significa che le strategie di offerta AdWords sono autorizzate a ottimizzare le offerte per tali conversioni. Puoi modificare questa impostazione dal tuo account AdWords.

1. Sotto la **Azioni stage** a discesa, seleziona **Imposta conversione AdWords**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Seleziona **Nuova conversione**.

   ![](assets/image2015-3-27-17-3a23-3a13.png)

1. Inserisci un **Nome conversione**. Fai clic su **Salva**.

   ![](assets/image2015-3-27-17-3a24-3a49.png)

   Eccellente! Questa nuova conversione verrà visualizzata nel tuo account AdWords.

## Usa mappatura AdWords {#use-adwords-mapping}

Puoi associare tutte le fasi del modello alla conversione AdWords in un&#39;unica posizione utilizzando le mappature AdWords.

1. Seleziona **Modifica mappature AdWords**.

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. Seleziona il **Account AdWords** e desiderato **Conversione AdWords** per ogni fase da monitorare.

   ![](assets/image2015-3-27-17-3a30-3a15.png)

1. Dopo aver mappato gli stadi, fai clic su **Salva**.

   ![](assets/image2015-3-27-17-3a30-3a48.png)

1. Dopo aver mappato tutte le conversioni di AdWords nelle fasi di ricavo, torna alla pagina di riepilogo. Seleziona **Azioni modello** e scegli **Approva fasi**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

Per visualizzare i dati di conversione offline, dovrai accedere al tuo account AdWords. Si consiglia di utilizzare le [Funzione Colonne personalizzate](https://support.google.com/adwords/answer/3073556) per creare colonne del conteggio di conversione per ogni conversione offline importata da Marketo.
