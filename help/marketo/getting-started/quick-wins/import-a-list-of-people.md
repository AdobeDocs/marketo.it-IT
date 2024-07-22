---
unique-page-id: 2359418
description: Importare un elenco di persone - Documentazione di Marketo - Documentazione del prodotto
title: Importa un elenco di persone
exl-id: a85ec787-7b22-4666-84fd-d7bf23d32cd4
feature: Getting Started
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '500'
ht-degree: 0%

---

# Importa un elenco di persone {#import-a-list-of-people}

## Missione: importare nel database un elenco di fogli di calcolo dei partecipanti alle fiere {#mission-import-a-spreadsheet-list-of-trade-show-attendees-into-your-database}

>[!PREREQUISITES]
>
>[Configurazione e aggiunta di una persona](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target="_blank"}

Questa esercitazione illustra come importare le persone da un file del foglio di calcolo in Marketo.

## Passaggio 1: Scaricare e modificare un foglio di calcolo {#step-download-and-edit-a-spreadsheet}

1. Per iniziare, scarica il file del foglio di calcolo dell&#39;esercitazione ([**tradeshow-attendees.csv**](/help/marketo/getting-started/assets/tradeshow-attendees.csv){target="_blank"}) nel computer.

   ![](assets/import-a-list-of-people-1.png)

   >[!NOTE]
   >
   >Durante l&#39;importazione di una data, utilizzare questo formato: **9/21/20** (mese/giorno/anno).

   >[!NOTE]
   >
   >Tutti i campi data/ora importati vengono trattati come ora centrale. Se sono presenti campi data/ora in un fuso orario diverso, è possibile utilizzare una formula di Excel per trasformarla in Ora centrale (America/Chicago).

1. Aggiungi nome, cognome, indirizzo e-mail effettivo (in modo da poter ricevere le e-mail di formazione che invierai nella prossima missione) e qualifica. Salva il file sul computer.

   ![](assets/import-a-list-of-people-2.png)

   >[!CAUTION]
   >
   >Marketo **non** supporta gli indirizzi e-mail che contengono emoticon.

## Passaggio 2: creare un programma {#step-create-a-program}

1. Vai all&#39;area **[!UICONTROL Attività di marketing]**.

   ![](assets/import-a-list-of-people-3.png)

1. Seleziona la cartella **Apprendimento**, quindi in **[!UICONTROL Nuovo]** fai clic su **[!UICONTROL Nuovo programma]**.

   ![](assets/import-a-list-of-people-4.png)

1. **Denomina** il programma &quot;Il mio programma di fiere&quot; e seleziona &quot;Evento&quot; per il **[!UICONTROL tipo di programma]**.

   ![](assets/import-a-list-of-people-5.png)

1. Seleziona **[!UICONTROL Presentazione]** per il **[!UICONTROL Canale]** e fai clic su **[!UICONTROL Crea]**.

   ![](assets/import-a-list-of-people-6.png)

>[!NOTE]
>
>I programmi di eventi si verificano in date specifiche. Ulteriori informazioni su [**Eventi**](/help/marketo/product-docs/demand-generation/events/understanding-events/understanding-event-programs.md){target="_blank"}.

## Passaggio 3: importare il foglio di calcolo in Marketo {#step-import-your-spreadsheet-into-marketo}

1. In **Programma di fiere**, fai clic su **[!UICONTROL Nuovo]** e seleziona **[!UICONTROL Nuova risorsa locale]**.

   ![](assets/import-a-list-of-people-7.png)

1. Seleziona **[!UICONTROL Elenco]**.

   ![](assets/import-a-list-of-people-8.png)

1. **Denomina** l&#39;elenco &quot;Partecipanti alla fiera&quot; e fai clic su **[!UICONTROL Crea]**.

   ![](assets/import-a-list-of-people-9.png)

1. Nell&#39;elenco **[!UICONTROL Partecipanti a fiere]** fare clic su **[!UICONTROL Azioni elenco]** e selezionare **[!UICONTROL Importa elenco]**.

   ![](assets/import-a-list-of-people-10.png)

   >[!CAUTION]
   >
   >Se utilizzi un file CSV, accertati che sia codificato in UTF-8, UTF-16, Shift-JIS o EUC-JP.

   >[!NOTE]
   >
   >Il limite di dimensione per i file CSV è di 100 MB.

1. **[!UICONTROL Individua]** il file del foglio di calcolo **tradeshow-attendees.csv** nel computer e fai clic su **[!UICONTROL Avanti]**.

   ![](assets/import-a-list-of-people-11.png)

   >[!NOTE]
   >
   >In modalità di importazione elenchi, se si sceglie **[!UICONTROL Ignora nuove persone e aggiornamenti]**, non verranno registrati record persona esistenti né attività. Utilizza questa modalità se desideri un elenco statico rapido e prefiltrato di persone esistenti da utilizzare nelle attività di marketing. Selezionando questa modalità:
   >
   > * Ignora creazione nuova persona
   > * Ignora aggiornamenti campo persona
   > * Ignora registrazione attività

1. Mappa i campi [!UICONTROL Colonna elenco] ai rispettivi campi Marketo e fai clic su **[!UICONTROL Avanti]**.

   ![](assets/import-a-list-of-people-12.png)

   >[!TIP]
   >
   >Per ottenere i migliori risultati di mappatura automatica, le intestazioni di colonna devono sempre corrispondere esattamente al campo (distinzione maiuscole/minuscole). Se stai utilizzando campi personalizzati e non li vedi nel menu a discesa, torna indietro e [creali](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md){target="_blank"} in modo che possano diventare opzioni.

   >[!NOTE]
   >
   >Se sono presenti campi che non si desidera importare, selezionare **Ignora** nel menu a discesa Campo Marketo.

1. Seleziona **Il mio programma di fiere** per il **[!UICONTROL programma di acquisizione]**, quindi fai clic su **[!UICONTROL Importa]**.

   ![](assets/import-a-list-of-people-13.png)

1. Attendi che le persone effettuino l&#39;importazione, quindi chiudi la finestra a comparsa di avanzamento dell&#39;importazione.

   ![](assets/import-a-list-of-people-14.png)

1. Tornando al **Programma di fiere**, fare clic sulla scheda **[!UICONTROL Membri]**. Vedrai tutte le persone appena importate.

   ![](assets/import-a-list-of-people-15.png)

>[!NOTE]
>
>Puoi analizzare il successo del programma tenendo traccia dell’iscrizione al programma. Ulteriori informazioni su [**Programmi**](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md){target="_blank"}.

## Missione completata {#mission-complete}

I partecipanti alle fiere sono ora membri del programma Marketo.

<br> 

[◄ Mission 4: risposta automatica e-mail](/help/marketo/getting-started/quick-wins/email-auto-response.md)

[Missione 6: gocciolamento, gocciolamento, ► di sviluppo](/help/marketo/getting-started/quick-wins/drip-drip-nurture.md)
