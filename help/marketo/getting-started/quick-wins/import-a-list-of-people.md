---
unique-page-id: 2359418
description: Importare un elenco di persone - Marketo Docs - Documentazione del prodotto
title: Importare un elenco di persone
exl-id: a85ec787-7b22-4666-84fd-d7bf23d32cd4
source-git-commit: 0da33dfa840dd1e5a5618fcd762b482f7a2e0789
workflow-type: tm+mt
source-wordcount: '500'
ht-degree: 0%

---

# Importare un elenco di persone {#import-a-list-of-people}

## Missione: Importa nel database un elenco di fogli di calcolo dei partecipanti alle fiere di commercio {#mission-import-a-spreadsheet-list-of-trade-show-attendees-into-your-database}

>[!PREREQUISITES]
>
>[Configurazione e aggiunta di una persona](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target=&quot;_blank&quot;}

Questa esercitazione spiega come importare in Marketo le persone da un file di foglio di calcolo.

## Passaggio 1: Scaricare e modificare un foglio di calcolo {#step-download-and-edit-a-spreadsheet}

1. Per iniziare, scarica il file del foglio di calcolo della pratica ([**fidelizzazione.csv**](/help/marketo/getting-started/assets/tradeshow-attendees.csv){target=&quot;_blank&quot;}) al computer.

   ![](assets/image2014-9-24-12-3a5-3a0.png)

   >[!NOTE]
   >
   >Quando importi una data, utilizza questo formato: **21/09/20** (Mese/Giorno/Anno).

   >[!NOTE]
   >
   >Tutti i campi data/ora da importare vengono trattati come Ora centrale. Se si dispone di campi data/ora in un fuso orario diverso, è possibile utilizzare una formula Excel per trasformarla in Ora centrale (America/Chicago).

1. Aggiungi il tuo nome, cognome, indirizzo e-mail effettivo (in modo da poter ricevere le e-mail di promozione che invierai nella prossima missione) e il titolo del lavoro. Salvare il file sul computer.

   ![](assets/image2014-9-24-12-3a5-3a30.png)

   >[!CAUTION]
   >
   >Marketo **not** supportano gli indirizzi e-mail che contengono emoticon.

## Passaggio 2: Creare un programma {#step-create-a-program}

1. Vai a **Attività di marketing** area.

   ![](assets/ma-2.png)

1. Seleziona la tua **Apprendimento** cartella, quindi sotto **Nuovo** click **Nuovo programma**.

   ![](assets/image2014-9-24-12-3a21-3a13.png)

1. **Nome** il programma &quot;My Tradeshow Program&quot; e selezionare &quot;Event&quot; per **Tipo di programma**.

   ![](assets/image2014-9-24-12-3a21-3a25.png)

1. Seleziona **Presentazione** per **Canale** e fai clic su **Crea**.

   ![](assets/image2014-9-24-12-3a21-3a39.png)

>[!NOTE]
>
>I programmi evento si verificano in date specifiche. Ulteriori informazioni [**Eventi**](/help/marketo/product-docs/demand-generation/events/understanding-events/understanding-event-programs.md){target=&quot;_blank&quot;}.

## Passaggio 3: Importare il foglio di calcolo in Marketo {#step-import-your-spreadsheet-into-marketo}

1. In **Il mio programma**, fai clic su **Nuovo** e seleziona **Nuova risorsa locale**.

   ![](assets/seven-3.png)

1. Fai clic su **Elenco**.

   ![](assets/image2014-9-24-12-3a22-3a56.png)

1. **Nome** l&#39;elenco &quot;Partecipanti alla fiera&quot; e fai clic su **Crea**.

   ![](assets/image2014-9-24-12-3a23-3a9.png)

1. Nel tuo **Partecipanti alla fiera** elenco, fai clic su **Azioni elenco** e seleziona **Importa elenco**.

   ![](assets/ten-2.png)

   >[!CAUTION]
   >
   >Se utilizzi un tuo file CSV, accertati che sia codificato UTF-8, UTF-16, Shift-JIS o EUC-JP.

   >[!NOTE]
   >
   >Il limite di dimensione per i file CSV è di 100 MB.

1. **Sfoglia** al **fidelizzazione.csv** foglio di calcolo sul computer e fai clic su **Successivo**.

   ![](assets/eleven-2.png)

   >[!NOTE]
   >
   >In modalità di importazione elenco, scegliere **Ignora nuove persone e aggiornamenti** significa che non influirai sui record di persone esistenti o non registrerai alcuna attività. Utilizza questa modalità se desideri un elenco rapido e pre-filtrato statico delle persone esistenti da utilizzare nelle attività di marketing. Selezionando questa modalità:
   >
   > * Ignora la creazione di nuove persone
   > * Ignora aggiornamenti campo persona
   > * Ignora registrazione attività


1. Mappa i campi della colonna dell’elenco nel rispettivo campo Marketo e fai clic su **Successivo**.

   ![](assets/image2014-9-24-12-3a24-3a49.png)

   >[!TIP]
   >
   >Per ottenere i migliori risultati di mappatura automatica, le intestazioni di colonna devono sempre corrispondere esattamente al campo (con distinzione tra maiuscole e minuscole). Se utilizzi campi personalizzati e non li visualizzi nell’elenco a discesa, torna indietro e [crearle](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md){target=&quot;_blank&quot;} in modo che possano diventare opzioni.

   >[!NOTE]
   >
   >Se sono presenti campi che non si desidera importare, selezionare **Ignora** nel menu a discesa Campo Marketo .

1. Seleziona **Il mio programma** per **Programma di acquisizione**, quindi fai clic su **Importa**.

   ![](assets/image2014-9-24-12-3a25-3a1.png)

1. Attendi l’importazione delle persone, quindi chiudi la finestra a comparsa di avanzamento dell’importazione.

   ![](assets/image2014-9-24-12-3a25-3a13.png)

1. Indietro **Il mio programma**, fai clic su **Membri** scheda . Vedrete tutte le persone appena importate.

   ![](assets/fifteen-1.png)

>[!NOTE]
>
>Puoi analizzare il successo del tuo programma monitorando l&#39;iscrizione al programma. Ulteriori informazioni [**Programmi**](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md){target=&quot;_blank&quot;}.

## Missione completata {#mission-complete}

I partecipanti al vostro programma sono ora membri del vostro programma Marketo!

<br> 

[◄ Missione 4: Risposta automatica e-mail](/help/marketo/getting-started/quick-wins/email-auto-response.md)

[Missione 6 Goccia, Asciugatura, Alimentazione ►](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)
