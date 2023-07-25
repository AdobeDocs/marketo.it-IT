---
unique-page-id: 10094404
description: Creare gruppi di campi personalizzati utilizzando la Libreria campi - Documenti Marketo - Documentazione del prodotto
title: Creare gruppi di campi personalizzati utilizzando l’Organizer campi
exl-id: 0425a446-2c92-4a2a-85c4-e05c22118035
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '992'
ht-degree: 2%

---

# Creare gruppi di campi personalizzati utilizzando l’Organizer campi {#create-custom-field-groups-using-the-field-organizer}

Prima di poter abilitare i gruppi di campi personalizzati per la generazione di rapporti nell&#39;area Analisi delle prestazioni del modello (lead) di Gestione ciclo ricavi, è necessario categorizzare i campi standard o personalizzati in gruppi per la generazione di rapporti tramite l&#39;Organizer campi in Gestione lead di Marketo. Questo vale solo per gli attributi del lead e della società.
Quando si seleziona un campo standard o personalizzato dall&#39;elenco a discesa Campo della finestra di dialogo Nuovo organizzatore campi, il tipo di dati Gestione lead di Marketo associato al campo che si desidera raggruppare viene mappato su uno dei tre editor disponibili nell&#39;organizzatore campi: stringa, numero intero o data.

| Tipo di dati Gestione lead Marketo | Tipo di dati editor organizzatore campi |
|---|---|
| Stringa | Stringa |
| E-mail | Stringa |
| Intero | Intero |
| Testo | Stringa |
| URL | Stringa |
| Riferimento | Non supportato |
| Valuta | Intero |
| Data e ora | Data |
| Booleano | Non supportato |
| Telefono | Stringa |
| Data | Data |
| Mobile | Intero |
| Calcolato | Non supportato |

Nelle tre sezioni successive viene descritto come creare un gruppo di campi personalizzato per una stringa, un numero intero o un tipo di data.

## Crea gruppo di campi personalizzato - Editor di stringhe {#create-custom-field-group-string-editor}

1. Clic **Database lead**.

   ![](assets/one.png)

1. Clic **Nuovo**, e seleziona **Crea Organizzatore Campi**.

   ![](assets/two.png)

1. Clic **Campo** e seleziona un campo standard o personalizzato con un tipo di dati mappato all’editor di stringhe (vedi tabella nella sezione precedente). Il paese è utilizzato qui.

   ![](assets/three.png)

1. Fai clic su **Crea**.

   ![](assets/four.png)

   Il nuovo gruppo personalizzato viene visualizzato nella struttura del database lead rappresentata da Nome campo > Gruppo nome campo (ad esempio: Paese > Gruppo paese).

   ![](assets/4.5.png)

1. Fai clic sull’icona della matita per personalizzare il nome. Ad esempio, è possibile rinominare &quot;Gruppo di paesi&quot; in &quot;Continente&quot;. Digita il nuovo nome desiderato e fai clic lontano dalla casella per salvare automaticamente.

   ![](assets/five.png)

1. Per impostazione predefinita, tutti i valori dei dati sono inseriti nel sottogruppo &quot;Altro&quot;. Per categorizzare i valori dei dati, fai clic su **Aggiungi gruppo** per creare un sottogruppo e assegnargli un nome.

   >[!NOTE]
   >
   >Puoi aggiungere fino a dieci sottogruppi per categorizzare i valori dei dati. A ogni sottogruppo creato viene assegnato un numero ID.

   In questo esempio, sono stati creati gruppi per la maggior parte dei continenti.

   ![](assets/six.png)

   >[!NOTE]
   >
   >Per eliminare un sottogruppo, fai clic sulla X rossa accanto al nome del sottogruppo. Se nel gruppo sono presenti valori di dati, questi verranno spostati nel gruppo predefinito Altro.

1. Evidenzia uno o più valori di dati nell’area di lavoro e trascina i valori di dati nel sottogruppo appropriato.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >Per rimuovere un valore di dati da un sottogruppo, riassegnare il valore di dati al gruppo predefinito Altro.

1. Utilizza l’opzione filtro nell’angolo in alto a sinistra direttamente sopra l’area di lavoro per selezionare e visualizzare i valori dei dati in uno o più sottogruppi. I valori dei dati basati sulla selezione dei filtri vengono visualizzati nell’area di lavoro.

   ![](assets/eight.png)

   >[!NOTE]
   >
   >Una volta definiti i gruppi, è possibile abilitare il gruppo di campi personalizzato per la generazione di rapporti in Analisi delle prestazioni del modello (lead) tramite la scheda Analisi del ciclo dei ricavi in Gestione lead di Marketo.

## Crea gruppo di campi personalizzato - Editor numeri interi {#create-custom-field-group-integer-editor}

1. Clic **Database lead**.

   ![](assets/one.png)

1. Clic **Nuovo**, e seleziona **Crea Organizzatore Campi**.

   ![](assets/two.png)

1. Clic **Campo** e seleziona un campo standard o personalizzato con un tipo di dati mappato all’editor di stringhe (vedi tabella nella sezione precedente). Il reddito annuale è utilizzato qui.

   ![](assets/nine.png)

1. Fai clic su **Crea**.

   ![](assets/9.5.png)

   Il nuovo gruppo personalizzato viene visualizzato nella struttura del database dei lead rappresentata da Nome campo > Gruppo nome campo (ad esempio Ricavo annuale > Gruppo ricavi annuale).

   ![](assets/9.6.png)

1. Fare clic sul nome del gruppo personalizzato predefinito sopra l&#39;editor di numeri interi per personalizzare il nome. Ad esempio, è possibile rinominare &quot;Gruppo di ricavi annuale&quot; in &quot;Ricavo annuale per dimensione&quot;. Clic **Salva**.

   ![](assets/eleven.png)

   L’editor di numeri interi consente di creare più sottogruppi per definire ciascun sottogruppo in base alla dimensione. In questo esempio verranno creati tre gruppi per le piccole, medie e imprese.

1. Per aggiungere il primo gruppo, immettere un nome nel campo **Nome gruppo** (ad esempio: piccolo) e immettere un valore massimo nel campo **Intervallo gruppo** (esempio: 200000). Clic **Aggiungi gruppo**.

   ![](assets/twelve.png)

   Sotto il gruppo appena inserito viene visualizzata una voce di gruppo vuota. L’esempio seguente mostra una voce per piccole, medie e imprese.

   >[!NOTE]
   >
   >Puoi aggiungere fino a dieci sottogruppi per categorizzare i valori dei dati. Ogni voce di Intervallo gruppi si basa sulla voce precedente. Se si lascia vuota l&#39;ultima voce Intervallo gruppi per l&#39;ultimo sottogruppo personalizzato creato, non viene impostato alcun valore massimo per i dati.

1. Fare clic sulla scheda Riepilogo per salvare e rivedere le impostazioni.

   ![](assets/thirteen.png)

   >[!NOTE]
   >
   >Per eliminare un sottogruppo, fai clic sulla X rossa accanto al nome del sottogruppo.

1. Nella pagina Riepilogo controllare le impostazioni.

   ![](assets/13.5.png)

   >[!NOTE]
   >
   >Una volta definiti i gruppi, è possibile abilitare il gruppo di campi personalizzato per la generazione di rapporti in Analisi delle prestazioni del modello (lead) tramite la scheda Analisi del ciclo dei ricavi in Gestione lead di Marketo.

## Crea gruppo di campi personalizzato - Editor date {#create-custom-field-group-date-editor}

1. Clic **Database lead**.

   ![](assets/one.png)

1. Clic **Nuovo**, e seleziona **Crea Organizzatore Campi**.

   ![](assets/two.png)

1. Clic **Campo** e seleziona un campo standard o personalizzato con un tipo di dati mappato all’editor di stringhe (vedi tabella nella sezione precedente). Qui viene utilizzata la data di acquisizione.

   ![](assets/fourteen.png)

1. Fai clic su **Crea**.

   ![](assets/14.5.png)

   Il nuovo gruppo personalizzato viene visualizzato nella struttura del database lead rappresentata da Nome campo > Gruppo nome campo (ad esempio: Data acquisizione > Gruppo data acquisizione).

   ![](assets/14.6.png)

1. Fai clic sul nome del gruppo personalizzato predefinito sopra l’editor di date per personalizzarlo. Ad esempio, puoi rinominare &quot;Gruppo di date di acquisizione&quot; in &quot;Categorie di date di acquisizione&quot;. Clic **Salva**.

   ![](assets/fifteen.png)

   L’editor di date consente di creare più sottogruppi e definire ciascun sottogruppo per data. In questo esempio verranno creati tre gruppi: Lead Q1-15, Lead Q2-15 e Lead Q3-15.

1. Per aggiungere il primo gruppo, immettere un nome nel campo **Nome gruppo** (ad esempio, Lead T1-15) e immettere una data nel campo data che rappresenta la data in cui il lead è stato acquisito o prima (ad esempio: 3/31/2015 per l&#39;ultimo giorno del T1-15). Clic **Aggiungi gruppo**.

   ![](assets/sixteen.png)

   >[!NOTE]
   >
   >Puoi aggiungere fino a dieci sottogruppi per categorizzare i valori dei dati. Ogni voce di Intervallo gruppi si basa sulla voce precedente. Se si lascia vuota l&#39;ultima voce Intervallo gruppi per l&#39;ultimo sottogruppo personalizzato creato, non viene impostato alcun valore per la data di fine.

   L’esempio seguente mostra una voce per i lead del primo trimestre 2015 che passano al terzo trimestre.

   ![](assets/16.5.png)

   Ed è tutto! Ottimo lavoro.
