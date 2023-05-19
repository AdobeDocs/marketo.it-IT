---
unique-page-id: 2359418
description: Importare un elenco di persone - Documentazione di Marketo - Documentazione del prodotto
title: Importa un elenco di persone
exl-id: a85ec787-7b22-4666-84fd-d7bf23d32cd4
source-git-commit: 80512816eaf0a70a3f10a50c34aeea14edd9046b
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 0%

---

# Importa un elenco di persone {#import-a-list-of-people}

## Missione: importare nel database un elenco di fogli di calcolo dei partecipanti alle fiere {#mission-import-a-spreadsheet-list-of-trade-show-attendees-into-your-database}

>[!PREREQUISITES]
>
>[Configurazione e aggiunta di una persona](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target="_blank"}

Questa esercitazione illustra come importare le persone da un file del foglio di calcolo in Marketo.

## Passaggio 1: Scaricare e modificare un foglio di calcolo {#step-download-and-edit-a-spreadsheet}

1. Per iniziare, scaricare il file del foglio di calcolo dell&#39;esercitazione ([**tradeshow-attendees.csv**](/help/marketo/getting-started/assets/tradeshow-attendees.csv){target="_blank"}) al computer.

   ![](assets/import-a-list-of-people-1.png)

   >[!NOTE]
   >
   >Quando importi una data, utilizza questo formato: **9/21/20** (mese/giorno/anno).

   >[!NOTE]
   >
   >Tutti i campi data/ora importati vengono trattati come ora centrale. Se sono presenti campi data/ora in un fuso orario diverso, è possibile utilizzare una formula di Excel per trasformarla in Ora centrale (America/Chicago).

1. Aggiungi nome, cognome, indirizzo e-mail effettivo (in modo da poter ricevere le e-mail di formazione che invierai nella prossima missione) e qualifica. Salva il file sul computer.

   ![](assets/import-a-list-of-people-2.png)

   >[!CAUTION]
   >
   >Marketo sì **non** supporta gli indirizzi e-mail che contengono emoji.

## Passaggio 2: creare un programma {#step-create-a-program}

1. Vai a **[!UICONTROL Attività di marketing]** area.

   ![](assets/import-a-list-of-people-3.png)

1. Seleziona il **Apprendimento** cartella, quindi in **[!UICONTROL Nuovo]** click **[!UICONTROL Nuovo programma]**.

   ![](assets/import-a-list-of-people-4.png)

1. **Nome** il programma &quot;My Tradeshow Program&quot; e selezionare &quot;Event&quot; per il **[!UICONTROL Tipo di programma]**.

   ![](assets/import-a-list-of-people-5.png)

1. Seleziona **[!UICONTROL Tradeshow]** per **[!UICONTROL Canale]** e fai clic su **[!UICONTROL Crea]**.

   ![](assets/import-a-list-of-people-6.png)

>[!NOTE]
>
>I programmi di eventi si verificano in date specifiche. Ulteriori informazioni su [**Eventi**](/help/marketo/product-docs/demand-generation/events/understanding-events/understanding-event-programs.md){target="_blank"}.

## Passaggio 3: importare il foglio di calcolo in Marketo {#step-import-your-spreadsheet-into-marketo}

1. In entrata **Il mio programma di fiere**, fai clic su **[!UICONTROL Nuovo]** e seleziona **[!UICONTROL Nuova risorsa locale]**.

   ![](assets/import-a-list-of-people-7.png)

1. Seleziona **[!UICONTROL Elenco]**.

   ![](assets/import-a-list-of-people-8.png)

1. **Nome** nell&#39;elenco Partecipanti alla fiera e fare clic su **[!UICONTROL Crea]**.

   ![](assets/import-a-list-of-people-9.png)

1. Nel tuo **[!UICONTROL Partecipanti a fiere]** , fare clic su **[!UICONTROL Azioni elenco]** e seleziona **[!UICONTROL Importa elenco]**.

   ![](assets/import-a-list-of-people-10.png)

   >[!CAUTION]
   >
   >Se utilizzi un file CSV, accertati che sia codificato in UTF-8, UTF-16, Shift-JIS o EUC-JP.

   >[!NOTE]
   >
   >Il limite di dimensione per i file CSV è di 100 MB.

1. **[!UICONTROL Sfoglia]** al **tradeshow-attendees.csv** file di foglio di calcolo sul computer e fare clic su **[!UICONTROL Successivo]**.

   ![](assets/import-a-list-of-people-11.png)

   >[!NOTE]
   >
   >In modalità di importazione elenco, scegliere **[!UICONTROL Ignora nuove persone e aggiornamenti]** significa che non influirai sui record persona esistenti o non registrerai alcuna attività. Utilizza questa modalità se desideri un elenco statico rapido e prefiltrato di persone esistenti da utilizzare nelle attività di marketing. Selezionando questa modalità:
   >
   > * Ignora creazione nuova persona
   > * Ignora aggiornamenti campo persona
   > * Ignora registrazione attività


1. Mappa il tuo [!UICONTROL Colonna elenco] ai rispettivi campi Marketo e fai clic su **[!UICONTROL Successivo]**.

   ![](assets/import-a-list-of-people-12.png)

   >[!TIP]
   >
   >Per ottenere i migliori risultati di mappatura automatica, le intestazioni di colonna devono sempre corrispondere esattamente al campo (distinzione maiuscole/minuscole). Se utilizzi campi personalizzati e non li vedi nel menu a discesa, torna indietro e [crearle](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md){target="_blank"} quindi possono diventare delle opzioni.

   >[!NOTE]
   >
   >Se sono presenti campi che non si desidera importare, selezionare **Ignora** nel menu a discesa Campo Marketo.

1. Seleziona **Il mio programma di fiere** per **[!UICONTROL Programma di acquisizione]**, quindi fai clic su **[!UICONTROL Importa]**.

   ![](assets/import-a-list-of-people-13.png)

1. Attendi che le persone effettuino l&#39;importazione, quindi chiudi la finestra a comparsa di avanzamento dell&#39;importazione.

   ![](assets/import-a-list-of-people-14.png)

1. Torna in **Il mio programma di fiere**, fare clic su **[!UICONTROL Membri]** scheda. Vedrai tutte le persone appena importate.

   ![](assets/import-a-list-of-people-15.png)

>[!NOTE]
>
>Puoi analizzare il successo del programma tenendo traccia dell’iscrizione al programma. Ulteriori informazioni su [**Programmi**](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md){target="_blank"}.

## Missione completata {#mission-complete}

I partecipanti alle fiere sono ora membri del programma Marketo.

<br> 

[◄ Mission 4: risposta automatica e-mail](/help/marketo/getting-started/quick-wins/email-auto-response.md)

[Missione 6: gocciolamento, gocciolamento, ► di sviluppo](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)
