---
unique-page-id: 2359418
description: Importa un elenco di persone - Documenti Marketo - Documentazione prodotto
title: Importa un elenco di persone
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 0%

---


# Importa un elenco di persone {#import-a-list-of-people}

## Missione: Importare un elenco di fogli di calcolo dei partecipanti alle presentazioni nel database {#mission-import-a-spreadsheet-list-of-trade-show-attendees-into-your-database}

>[!PREREQUISITES]
>
>[Configurazione e aggiunta di una persona](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md)

Questa esercitazione spiega come importare le persone da un file di foglio di calcolo in Marketo.

## Passaggio 1: Download e modifica di un foglio di calcolo {#step-download-and-edit-a-spreadsheet}

1. Per iniziare, scaricate il file del foglio di calcolo di esercitazione ([**fideiussore-partecipanti.csv**](https://docs.marketo.com/display/docs/assets/tradeshow-attendees.csv)) nel computer.

   ![](assets/image2014-9-24-12-3a5-3a0.png)

   >[!NOTE]
   >
   >Durante l’importazione di una data, usa il seguente formato: **21/9/20** (mese/giorno/anno).

   >[!NOTE]
   >
   >Tutti i campi data/ora importati vengono considerati come Ora centrale. Se i campi data/ora si trovano in un fuso orario diverso, è possibile utilizzare una formula Excel per trasformarla in Ora centrale (America/Chicago).

1. Aggiungete il vostro nome, cognome, indirizzo e-mail e titolo del processo, quindi salvate il file sul computer.

   ![](assets/image2014-9-24-12-3a5-3a30.png)

>[!NOTE]
>
>Immettete il vostro indirizzo e-mail reale nel file CSV in modo da poter ricevere i messaggi e-mail di incoraggiamento che invierete alla prossima missione.

## Passaggio 2: Creare un programma {#step-create-a-program}

1. Andate all&#39;area **Attività di marketing**.

   ![](assets/ma-2.png)

1. Selezionare la cartella **Learning**, quindi in **New** fare clic su **New Program** (Nuovo programma).

   ![](assets/image2014-9-24-12-3a21-3a13.png)

1. **Assegnare** un nome al programma &quot;My Tradeshow Program&quot; e selezionare &quot;Event&quot; per il tipo **di** programma.

   ![](assets/image2014-9-24-12-3a21-3a25.png)

1. Selezionare **Tradeshow** per il **Canale** e fare clic su **Crea**.

   ![](assets/image2014-9-24-12-3a21-3a39.png)

>[!NOTE]
>
>I programmi evento si verificano in date specifiche. Ulteriori informazioni su [**Eventi**](/help/marketo/product-docs/demand-generation/events/understanding-events/understanding-event-programs.md).

## Passaggio 3: Importa il foglio di calcolo in Marketo {#step-import-your-spreadsheet-into-marketo}

1. In **My Tradeshow Program**, fare clic su **New** e selezionare **New Local Asset** (Nuova risorsa locale).

   ![](assets/seven-3.png)

1. Fare clic su **List**.

   ![](assets/image2014-9-24-12-3a22-3a56.png)

1. **Denominate** l&#39;elenco &quot;Partecipanti alla presentazione&quot; e fate clic su  **Crea**.

   ![](assets/image2014-9-24-12-3a23-3a9.png)

1. Nell&#39;elenco **Partecipanti alla presentazione**, fare clic su **Azioni elenco** e selezionare **Importa elenco**.

   ![](assets/ten-2.png)

   >[!CAUTION]
   >
   >Se usate un file CSV personalizzato, accertatevi che sia codificato UTF-8, UTF-16, Shift-JIS o EUC-JP.

   >[!NOTE]
   >
   >Il limite di dimensione per i file CSV è di 100 MB.

1. **Andate** al file  **del foglio di calcolo fidelizzato-partecipanti.** csveli sul computer e fate clic su  **Avanti**.

   ![](assets/eleven-2.png)

   >[!NOTE]
   >
   >In modalità di importazione elenco, se si sceglie **Ignora nuove persone e aggiornamenti**, non si avranno effetti sui record di persone esistenti o si registreranno attività. Utilizzate questa modalità se desiderate un elenco rapido e pre-filtrato di persone esistenti da utilizzare nelle attività di marketing. Selezionando questa modalità:
   >
   > * Consente di saltare la creazione di nuove persone
   > * Ignora aggiornamenti campo persona
   > * Ignora registrazione attività


1. Mappare i campi Colonna elenco nel rispettivo Campo Marketo e fare clic su **Avanti**.

   ![](assets/image2014-9-24-12-3a24-3a49.png)

   >[!TIP]
   >
   >Le intestazioni delle colonne devono sempre corrispondere al campo esattamente (con distinzione tra maiuscole e minuscole) per ottenere i migliori risultati di mappatura automatica. Se si utilizzano campi personalizzati e non li si visualizza nell&#39;elenco a discesa, tornare indietro e [crearli](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md) in modo che possano diventare opzioni.

   >[!NOTE]
   >
   >Se non si desidera importare alcun campo, selezionare **Ignora** nel menu a discesa Campo marketing.

1. Selezionare **My Tradeshow Program** per **Acquisition Program**, quindi fare clic su **Import**.

   ![](assets/image2014-9-24-12-3a25-3a1.png)

1. Attendete che la gente importi, quindi chiudete la finestra a comparsa di avanzamento dell’importazione.

   ![](assets/image2014-9-24-12-3a25-3a13.png)

1. Di nuovo in **My Tradeshow Program**, fare clic sulla scheda **Members**. Vedrete tutte le persone che avete appena importato.

   ![](assets/fifteen-1.png)

>[!NOTE]
>
>È possibile analizzare il successo del programma monitorando l&#39;iscrizione al programma. Ulteriori informazioni su [**Programmi**](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md).

## Missione completata {#mission-complete}

I partecipanti alle tue fiere ora sono membri del tuo programma Marketo!

<br> 

[◄ Missione 4: Risposta automatica e-mail](/help/marketo/getting-started/quick-wins/email-auto-response.md)

[Missione 6: Drip, Drip, Cura ►](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)
