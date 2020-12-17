---
unique-page-id: 2359414
description: Punteggio semplice - Marketo Docs - Documentazione del prodotto
title: Punteggio semplice
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 0%

---


# Punteggio semplice {#simple-scoring}

>[!PREREQUISITES]
>
>* [Configurazione e aggiunta di una persona](get-set-up-and-add-a-person.md)
>* [Pagina di destinazione con un modulo](landing-page-with-a-form.md)


## Passaggio 1: Creazione di una campagna di punteggio {#step-create-a-scoring-campaign}

1. Andate all&#39;area **Attività di marketing**.

   ![](assets/ma-1.png)

1. Fare clic con il pulsante destro del mouse sulla cartella **Learning** e scegliere **Nuova cartella campagna**.

   ![](assets/two-2.png)

1. Denominate la cartella della campagna &quot;Scoring&quot;.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >Se disponete già di una cartella Punteggio, denominatela come qualcosa di diverso, ad esempio Punteggio 1. I nomi delle cartelle devono essere univoci.

1. Fate clic con il pulsante destro del mouse sulla nuova cartella **Scoring** e selezionate **New Smart Campaign**.

   ![](assets/four.png)

1. **Denominate** la campagna &quot;Change Score&quot; e fate clic su  **Create (Crea)**.

   ![](assets/five-1.png)

1. Fare clic sulla scheda **Smart List**.

   ![](assets/six-1.png)

   Vogliamo che questa campagna venga eseguita ogni volta che una persona compila il **modulo di richiesta di prova**.

1. Individuare e trascinare il trigger **Riempie il modulo** sul quadro sinistro.

   ![](assets/image2014-9-24-11-3a43-3a35.png)

1. Selezionare **My Form**.

   >[!NOTE]
   >
   >Se hai completato la [pagina di destinazione con una vittoria rapida di Form](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md), dovresti avere il modulo. Se per il modulo è stato utilizzato un nome diverso, selezionarlo.

   ![](assets/image2014-9-24-11-3a44-3a16.png)

1. Fare clic sulla scheda **Flusso**.

   ![](assets/image2014-9-24-11-3a44-3a33.png)

1. Trascinare l&#39;azione di flusso **Modifica punteggio** sul quadro sinistro.

   ![](assets/image2014-9-24-11-3a44-3a45.png)

1. È possibile digitare qualsiasi valore da aggiungere al punteggio della persona. Immettete &quot;+5&quot; nel campo **Change**.

   ![](assets/eleven-1.png)

   >[!TIP]
   >
   >Buone campagne di assegnazione dei punteggi sono fondamentali per la distribuzione di personale di alta qualità alle vendite. Leggi [**La guida definitiva al punteggio lead**](https://www.marketo.com/definitive-guides/lead-scoring/).

1. Fare clic sulla scheda **Schedule** e sul pulsante **Activate**.

   ![](assets/twelve-1.png)

1. Fare clic su **Attiva** nella schermata di conferma.

   ![](assets/thirteen-1.png)

>[!NOTE]
>
>Una volta attivata, questa campagna viene eseguita ogni volta che una persona compila il modulo. La campagna continuerà a essere attiva finché non verrà disattivata.

## Passaggio 2: Compilare il modulo {#step-fill-out-the-form}

1. Selezionare la pagina di destinazione creata nella [pagina di destinazione con una vittoria rapida di Form](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md).

   ![](assets/fourteen-1.png)

1. Fare clic su **Visualizza pagina approvata**. La pagina di destinazione verrà aperta in una nuova scheda.

   ![](assets/image2014-9-24-11-3a47-3a51.png)

1. Compila il modulo con il tuo nome, cognome e indirizzo e-mail, quindi fai clic su **Invia**.

   ![](assets/image2014-9-24-11-3a47-3a59.png)

   >[!NOTE]
   >
   >Utilizzate lo stesso nome e indirizzo e-mail usato la prima volta che vi siete inseriti come persona per applicare l&#39;aumento di punteggio &quot;+5&quot;.

## Passaggio 3: Visualizza informazioni persona {#step-view-the-person-info}

1. Passare all&#39;area Database.

   ![](assets/db-2.png)

1. Cercare l&#39;indirizzo e-mail utilizzato durante la compilazione del modulo.

   ![](assets/eighteen.png)

1. Fate doppio clic sulla persona.

   ![](assets/nineteen.png)

I dettagli della persona verranno aperti in una nuova scheda o in una nuova finestra. Vedere come il punteggio è aumentato di 5 punti per compilare il modulo?!

![](assets/twenty.png)

**Congratulazioni!** È stata creata una campagna di valutazione.
[◄ Missione 2: Pagina di destinazione con un modulo](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md)

[Missione 4: Risposta automatica e-mail ►](/help/marketo/getting-started/quick-wins/email-auto-response.md)
