---
unique-page-id: 6095029
description: Imposta le conversioni di Google AdWords nel modello delle entrate - Documenti Marketo - Documentazione del prodotto
title: Imposta conversioni Google AdWords nel modello Revenue
translation-type: tm+mt
source-git-commit: cb7df3dd38275837f8ab05ce846c2c68ab78462f
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 0%

---


# Imposta conversioni Google AdWords nel modello Revenue {#set-google-adwords-conversions-in-the-revenue-model}

Collega il tuo account Google AdWords a Marketo per caricare automaticamente i dati di conversione offline da Marketo a Google AdWords. Quindi, dall&#39;interfaccia utente di AdWords, potrai vedere facilmente quali clic hanno portato a lead qualificati, opportunità e nuovi clienti (o qualsiasi fase di fatturato desideri monitorare) dopo che hai [aggiunto colonne personalizzate](https://support.google.com/adwords/answer/3073556) in AdWords.

>[!NOTE]
>
>Questa è un&#39;integrazione push da Marketo a Google AdWords. I dati di conversione verranno visualizzati _solo_ nel portale Google AdWords, _non nell&#39;interfaccia di Marketing_.

Ulteriori informazioni sulla [funzionalità di importazione delle conversioni offline di Google](https://support.google.com/adwords/answer/2998031?hl=en). Mappatura conversioni offline di AdWords in uno o più stadi di un modello Revenue. Esistono tre modi per eseguire la mappatura:

* Conversione AdWords
* Azione fase
* Mappatura AdWords

Puoi creare una nuova conversione offline AdWords da Marketo se utilizzi Action stage.

>[!PREREQUISITES]
>
>[Aggiungi Google AdWords come servizio LaunchPoint](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service.md)

## Usa conversione AdWords {#use-adwords-conversion}

1. Andate all&#39;area **Analytics**.

   ![](assets/image2015-2-23-18-3a9-3a34.png)

1. Selezionare un modello.

   ![](assets/image2015-2-23-18-3a3-3a12.png)

1. Fare clic su **Modifica bozza**.

   ![](assets/image2015-3-10-15-3a3-3a20.png)

1. Seleziona la fase ricavi da mappare su una conversione AdWords.

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. Selezionare la **Conversione AdWords** da mappare sul passaggio Marketo.

   ![](assets/image2015-2-26-16-3a46-3a15.png)

   Bello! I dati di conversione AdWords verranno caricati su Google AdWords alla cadenza selezionata.

## Usa azione fase {#use-stage-action}

È inoltre possibile mappare una conversione AdWords in Azioni fase.

1. Seleziona il passaggio da mappare a una conversione AdWords.

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. Nel menu a discesa **Azioni fase**, selezionare **Imposta conversione AdWords**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Selezionare una **Conversione AdWords**.

   ![](assets/image2015-2-26-16-3a54-3a47.png)

   **Suggerimento**: Se non hai conversioni AdWords, creane una facendo clic su  **+Nuova conversione**.

   ![](assets/image2015-2-26-21-3a22-3a10.png)

1. Fare clic su **Salva**.

   ![](assets/image2015-2-26-16-3a56-3a2.png)

1. Dopo aver mappato tutte le conversioni AdWords alle fasi ricavo, torna alla pagina di riepilogo. Selezionare **Azioni modello** e scegliere **Approva fasi**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

## Suggerimento Pro: Aggiungere una nuova conversione {#pro-tip-add-a-new-conversion}

Suggerimento Pro! Da Marketo è possibile creare una nuova conversione offline AdWords.

>[!CAUTION]
>
>Nuove conversioni create da Marketo con l&#39;impostazione &quot;ottimizzazione&quot; abilitata. Ciò significa che le strategie di offerta AdWords possono ottimizzare le offerte per tali conversioni. Puoi modificare questa impostazione dal tuo account AdWords.

1. Nel menu a discesa **Azioni fase**, selezionare **Imposta conversione AdWords**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Selezionare **Nuova conversione**.

   ![](assets/image2015-2-26-21-3a22-3a10.png)

1. Immettere un **Nome conversione**. Fare clic su **Salva**.

   ![](assets/image2015-2-26-21-3a24-3a7.png)

   Eccellente! Questa nuova conversione verrà visualizzata nel tuo account AdWords.

## Usa mappatura AdWords {#use-adwords-mapping}

Puoi associare tutte le fasi del modello alla conversione AdWords in un&#39;unica posizione utilizzando le mappature AdWords.

1. Selezionare **Modifica mappature AdWords**.

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. Selezionare la **Conversione AdWords** desiderata per ogni fase da monitorare.

   ![](assets/image2015-2-26-17-3a6-3a15.png)

1. Dopo aver mappato le fasi, fare clic su **Salva**.

   ![](assets/image2015-2-26-17-3a7-3a48.png)

1. Dopo aver mappato tutte le conversioni AdWords alle fasi ricavo, torna alla pagina di riepilogo. Selezionare **Azioni modello** e scegliere **Approva fasi**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

Per visualizzare i dati di conversione offline, dovrai accedere al tuo account AdWords. È consigliabile utilizzare la funzione [Colonne personalizzate](https://support.google.com/adwords/answer/3073556) per creare le colonne del conteggio di conversione per ogni conversione offline importata da Marketo.
