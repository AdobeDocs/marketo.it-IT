---
unique-page-id: 2359414
description: Punteggio semplice - Documentazione di Marketo - Documentazione del prodotto
title: Punteggio semplice
exl-id: 6129d46a-e6d2-4819-9b6c-ccbf37060712
feature: Getting Started
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---

# Punteggio semplice {#simple-scoring}

>[!PREREQUISITES]
>
>* [Configurazione e aggiunta di una persona](/help/marketo/getting-started/quick-wins/get-set-up-and-add-a-person.md){target="_blank"}
>* [Pagina di destinazione con modulo](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}

## Passaggio 1: creare una campagna punteggio {#step-create-a-scoring-campaign}

1. Vai all&#39;area **[!UICONTROL Attività di marketing]**.

   ![](assets/simple-scoring-1.png)

1. Fai clic con il pulsante destro del mouse sulla cartella **Apprendimento** e fai clic su **[!UICONTROL Nuova cartella campagne]**.

   ![](assets/simple-scoring-2.png)

1. Denomina la cartella della campagna &quot;Punteggio&quot; e fai clic su **[!UICONTROL Crea]**.

   ![](assets/simple-scoring-3.png)

   >[!NOTE]
   >
   >Se disponi già di una cartella Punteggio, assegna a questa un nome diverso, ad esempio Punteggio 1. I nomi delle cartelle devono essere univoci.

1. Fai clic con il pulsante destro del mouse sulla cartella **Punteggio** e seleziona **[!UICONTROL Nuova campagna avanzata]**.

   ![](assets/simple-scoring-4.png)

1. Denomina la campagna &quot;Punteggio di modifica&quot; e fai clic su **[!UICONTROL Crea]**.

   ![](assets/simple-scoring-5.png)

1. Fare clic sulla scheda **[!UICONTROL Elenco avanzato]**.

   ![](assets/simple-scoring-6.png)

   Vogliamo che questa campagna venga eseguita ogni volta che una persona compila il **modulo di richiesta di prova**.

1. Trova e trascina il trigger **[!UICONTROL Compila modulo]** nell&#39;area di lavoro a sinistra.

   ![](assets/simple-scoring-7.png)

1. Seleziona **Modulo personale**.

   ![](assets/simple-scoring-8.png)

   >[!NOTE]
   >
   >Se hai completato la [pagina di destinazione con un modulo](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"} vinto rapidamente, dovresti disporre del modulo. Se per il modulo è stato utilizzato un nome diverso, selezionarlo.

1. Fare clic sulla scheda **[!UICONTROL Flusso]**.

   ![](assets/simple-scoring-9.png)

1. Trascina l&#39;azione di flusso **Change Score** nell&#39;area di lavoro a sinistra.

   ![](assets/simple-scoring-10.png)

1. Puoi digitare qualsiasi valore da aggiungere al punteggio della persona. Immettiamo &quot;+5&quot; nel campo **[!UICONTROL Modifica]**.

   ![](assets/simple-scoring-11.png)

   >[!TIP]
   >
   >Le campagne con un buon punteggio sono fondamentali per offrire alle vendite personale di alta qualità. Leggi [**La guida definitiva al punteggio lead**](https://www.marketo.com/definitive-guides/lead-scoring/){target="_blank"}.

1. Fai clic sulla scheda **[!UICONTROL Pianifica]** e sul pulsante **[!UICONTROL Attiva]**.

   ![](assets/simple-scoring-12.png)

1. Fai clic su **[!UICONTROL Attiva]** nella schermata di conferma.

   ![](assets/simple-scoring-13.png)

>[!NOTE]
>
>Una volta attivata, questa campagna verrà eseguita ogni volta che una persona compila il modulo. La campagna continuerà a essere in esecuzione fino a quando non verrà disattivata.

## Passaggio 2: compilare il modulo {#step-fill-out-the-form}

1. Seleziona la pagina di destinazione creata nella [pagina di destinazione con una vincita rapida modulo](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md){target="_blank"}.

   ![](assets/simple-scoring-14.png)

1. Fare clic su **[!UICONTROL Anteprima]**. La pagina di destinazione si aprirà in una nuova scheda.

   ![](assets/simple-scoring-15.png)

1. Compila il modulo con il tuo nome, cognome e indirizzo e-mail, quindi fai clic su **[!UICONTROL Invia]**.

   ![](assets/simple-scoring-16.png)

   >[!NOTE]
   >
   >Utilizza lo stesso nome e indirizzo e-mail utilizzati al momento del tuo primo ingresso come persona per applicare l’aumento di punteggio &quot;+5&quot;.

## Passaggio 3: visualizzare le informazioni sulla persona {#step-view-the-person-info}

1. Passare all&#39;area **[!UICONTROL Database]**.

   ![](assets/simple-scoring-17.png)

1. Cerca l’indirizzo e-mail utilizzato durante la compilazione del modulo.

   ![](assets/simple-scoring-18.png)

1. Fai doppio clic sulla persona.

   ![](assets/simple-scoring-19.png)

I dettagli della persona verranno aperti in una nuova scheda o finestra. Vedi come il tuo punteggio è aumentato di 5 punti per la compilazione del modulo?

![](assets/simple-scoring-20.png)

## Missione completata! {#mission-complete}

<br> 

[◄ Mission 2: Pagina di destinazione con un modulo](/help/marketo/getting-started/quick-wins/landing-page-with-a-form.md)

[Missione 4: ► di risposta automatica e-mail](/help/marketo/getting-started/quick-wins/email-auto-response.md)
