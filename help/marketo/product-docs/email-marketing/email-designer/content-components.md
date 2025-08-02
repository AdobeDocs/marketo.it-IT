---
solution: Marketo Engage
product: marketo
title: Componenti contenuto
description: DESCRIZIONE.
level: Beginner, Intermediate
feature: Email Designer
hide: true
hidefromtoc: true
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '1154'
ht-degree: 0%

---

# Componenti contenuto {#content-components}

Durante la creazione del contenuto dell&#39;e-mail, **[!UICONTROL Content components]** ti consente di personalizzare ulteriormente l&#39;e-mail con componenti non elaborati che puoi modificare una volta inseriti in un messaggio e-mail.

Puoi aggiungere tutti i componenti di contenuto necessari all’interno di uno o più componenti struttura, che definiscono il layout dell’e-mail.

## Aggiungere componenti per contenuti {#add-content-components}

Per aggiungere componenti di contenuto all’e-mail e adattarli alle tue esigenze, segui i passaggi indicati di seguito.

1. In E-mail Designer, usa un contenuto esistente o trascina **[!UICONTROL Structure components]** nel contenuto vuoto per definire il layout dell&#39;e-mail. `[Learn how](content-from-scratch.md)`

1. Per accedere alla sezione **[!UICONTROL Content components]**, selezionare il pulsante corrispondente nel riquadro sinistro di E-mail Designer.

   SCHERMATA

1. Trascina i componenti di contenuto selezionati all’interno dei componenti struttura rilevanti.

   SCHERMATA

   >[!NOTE]
   >
   >Puoi aggiungere più componenti in un singolo componente struttura e in ogni colonna di un componente struttura.

1. Regolare gli attributi e lo stile di ogni componente utilizzando le schede **[!UICONTROL Settings]** e **[!UICONTROL Style]** a destra. Ad esempio, puoi modificare lo stile del testo, la spaziatura interna o il margine di ciascun componente. `[Learn more about alignment and padding](alignment-and-padding.md)`

   SCHERMATA

1. Dal menu avanzato di **[!UICONTROL Content component]**, puoi eliminare o duplicare facilmente qualsiasi componente di contenuto in base alle esigenze.

   SCHERMATA

## Contenitore {#container}

Per applicare uno stile specifico a un gruppo di componenti di contenuto, è possibile aggiungere un componente **[!UICONTROL Container]** e quindi i componenti di contenuto desiderati al suo interno. Questo consente di applicare uno stile distinto al contenitore, che sarà diverso dallo stile applicato ai componenti di contenuto all’interno.

Aggiungere ad esempio un componente **[!UICONTROL Container]** e quindi un componente [Button](#button) all&#39;interno del contenitore. Puoi utilizzare uno sfondo specifico per il contenitore e un altro per il pulsante.

SCHERMATA

## Pulsante {#button}

Utilizza il componente **[!UICONTROL Button]** per inserire uno o più pulsanti nel messaggio e-mail e reindirizzare il pubblico e-mail a un&#39;altra pagina.

1. Da **[!UICONTROL Content components]** trascinare e rilasciare il componente **[!UICONTROL Button]** in un **[!UICONTROL Structure component]**.

1. Fai clic sul pulsante appena aggiunto per personalizzare il testo e accedere alle schede **[!UICONTROL Settings]** e **[!UICONTROL Styles]** nel riquadro a destra di E-mail Designer.

   SCHERMATA

1. Dal menu **[!UICONTROL Link]**, aggiungi l&#39;URL a cui desideri reindirizzare quando fai clic sul pulsante.

1. Scegli come verrà reindirizzato il pubblico con l&#39;elenco a discesa **[!UICONTROL Target]**:

   * **[!UICONTROL None]**: apre il collegamento nello stesso frame in cui è stato fatto clic (impostazione predefinita).
   * **[!UICONTROL Blank]**: apre il collegamento in una nuova finestra o scheda.
   * **[!UICONTROL Self]**: apre il collegamento nello stesso frame in cui è stato fatto clic.
   * **[!UICONTROL Parent]**: apre il collegamento nel frame principale.
   * **[!UICONTROL Top]**: apre il collegamento nel corpo completo della finestra.

   SCHERMATA

1. Puoi personalizzare ulteriormente il pulsante modificando gli attributi di stile come **[!UICONTROL Border]**, **[!UICONTROL Size]**, **[!UICONTROL Margin]** e così via. dal riquadro **[!UICONTROL Component settings]**.

## Testo {#text}

Utilizza il componente **[!UICONTROL Text]** per inserire testo nel messaggio e-mail e regolare lo stile (bordo, dimensione, spaziatura interna, ecc.) utilizzando la scheda **[!UICONTROL Styles]**.

SCHERMATA

1. Da **[!UICONTROL Content components]** trascinare e rilasciare il componente **[!UICONTROL Text]** in un **[!UICONTROL Structure component]**.

1. Fai clic sul componente appena aggiunto per personalizzare il testo e accedere alle schede **[!UICONTROL Settings]** e **[!UICONTROL Styles]** nel riquadro a destra di E-mail Designer.

1. Modifica il testo con le seguenti opzioni disponibili nella barra degli strumenti:

   SCHERMATA

   * **[!UICONTROL Change text style]**: applica il grassetto, il corsivo, la sottolineatura o il barrato al testo.
   * **Cambia allineamento**: scegli l&#39;allineamento a sinistra, a destra, al centro o giustificato per il testo.
   * **[!UICONTROL Create list]**: aggiungere un elenco puntato o numerato al testo.
   * **[!UICONTROL Set heading]**: aggiungi fino a sei livelli di intestazione al testo.
   * **Dimensione font**: seleziona la dimensione font del testo in pixel.
   * **[!UICONTROL Change font color]**: scegliere il colore del carattere.
   * **[!UICONTROL Insert link]**: aggiungi qualsiasi tipo di collegamento al contenuto.
   * **[!UICONTROL Edit image]**: aggiungi un&#39;immagine o una risorsa al componente testo. `[Learn more about asset management](../integrations/assets.md)`
   * **[!UICONTROL Change font color]**: scegliere il colore del carattere.
   * **[!UICONTROL Add personalization]**: aggiungi campi di personalizzazione per personalizzare il contenuto dai dati dei profili. `[Learn more about content personalization](../personalization/personalize.md)`
   * **[!UICONTROL Show the source code]**: visualizza il codice sorgente del testo. Non può essere modificato.
   * **[!UICONTROL Enable conditional content]**: aggiungi contenuto condizionale per adattare il contenuto del componente ai profili target. `[Learn more about dynamic content](../personalization/get-started-dynamic-content.md)`
   * **[!UICONTROL Duplicate]**: aggiungi una copia del componente testo.
   * **[!UICONTROL Delete]**: elimina il componente testo selezionato dal messaggio e-mail.

1. Regola gli altri attributi di stile, ad esempio il colore del testo, la famiglia di caratteri, il bordo, la spaziatura interna, il margine e così via. dalla scheda **[!UICONTROL Styles]**.

   SCHERMATA

## Divisore {#divider}

Utilizza il componente **[!UICONTROL Divider]** per inserire una linea di divisione per organizzare il layout e il contenuto dell&#39;e-mail.

È possibile regolare gli attributi di stile, ad esempio il colore della linea, lo stile e l&#39;altezza, dalle schede **[!UICONTROL Settings]** e **[!UICONTROL Styles]**.

SCHERMATA

## HTML {#HTML}

Utilizza il componente **[!UICONTROL HTML]** per copiare e incollare le diverse parti del HTML esistente. Questo consente di creare componenti HTML modulari gratuiti per riutilizzare alcuni contenuti esterni.

1. Da **[!UICONTROL Content Components]** trascinare e rilasciare il componente **[!UICONTROL HTML]** in un **[!UICONTROL Structure component]**.

1. Fai clic sul componente appena aggiunto, quindi seleziona **[!UICONTROL Show the source code]** dalla barra degli strumenti contestuale per aggiungere il tuo HTML.

   SCHERMATA

1. Copiare e incollare il codice HTML che si desidera aggiungere all&#39;e-mail e fare clic su **[!UICONTROL Save]**.

   SCHERMATA

>[!NOTE]
>
>Per rendere semplicemente un contenuto esterno conforme a E-mail Designer, Adobe consiglia di creare un messaggio da zero e copiare il contenuto dall’e-mail esistente nei componenti.

## Immagine {#image}

Utilizza il componente **[!UICONTROL Image]** per inserire un file immagine dal computer nel contenuto dell&#39;e-mail.

1. Da **[!UICONTROL Content components]** trascinare e rilasciare il componente **[!UICONTROL Image]** in un **[!UICONTROL Structure component]**.

   SCHERMATA

1. Dalla scheda **[!UICONTROL Settings]**, fai clic su **[!UICONTROL Browse]** per scegliere un file di immagine dalle risorse oppure su **[!UICONTROL Import media]** per caricare una risorsa in Adobe Experience Manager Assets.

   Per ulteriori informazioni su [!DNL Adobe Experience Manager Assets], consulta la [documentazione di Adobe Experience Manager Assets](https://experienceleague.adobe.com/docs/experience-manager-assets-essentials/help/introduction.html){target="_blank"}.

   >[!NOTE]
   >
   > Per garantire che i collegamenti rimangano attivi ed evitare problemi di scadenza, ti consigliamo di utilizzare Adobe Assets invece di fare affidamento su un URL di origine per le immagini.

1. È inoltre possibile eseguire ricerche direttamente in Adobe Stock con l&#39;opzione **[!UICONTROL Find Adobe Stock photos]**.

1. Fai clic sul componente appena aggiunto e imposta le proprietà dell’immagine:

   * **[!UICONTROL Image title]** consente di definire un titolo per l&#39;immagine.
   * **[!UICONTROL Alt text]** ti consente di definire la didascalia collegata all&#39;immagine. Corrisponde all’attributo alt HTML.

   SCHERMATA

1. Puoi anche scegliere di **[!UICONTROL Find similar Stock photos]**. `[Learn more](../integrations/stock.md)`

1. Dalla scheda **[!UICONTROL Styles]**, regola gli altri attributi di stile come margine, bordo e così via. o aggiungendo un collegamento per reindirizzare il pubblico a un altro contenuto dal riquadro **[!UICONTROL Component settings]**.

## Social {#social}

Utilizza il componente **[!UICONTROL Social]** per inserire collegamenti a pagine di social media nel contenuto delle e-mail.

1. Da **[!UICONTROL Content Components]** trascinare e rilasciare il componente **[!UICONTROL Social]** in un **[!UICONTROL Structure component]**.

1. Seleziona il componente appena aggiunto.

1. Nel campo **[!UICONTROL Social]** della scheda **[!UICONTROL Settings]**, scegli il social media da aggiungere o rimuovere.

   SCHERMATA

1. Scegli le dimensioni delle icone nel campo dedicato.

1. Fai clic su ciascuna delle icone dei social media per configurare **[!UICONTROL URL]** a cui verrà reindirizzato il pubblico.

   SCHERMATA

1. Se necessario, puoi anche cambiare le icone di ciascuno dei social media dal tuo Assets.

1. Regola gli altri attributi di stile come stile, margine, bordo e così via. dalla scheda **[!UICONTROL Styles]**.

## Decisione sull’offerta {#offer-decision}

Utilizza il componente **[!UICONTROL Offer decision]** per inserire le offerte nei messaggi. Il motore di `[decision management](../offers/get-started/starting-offer-decisioning.md)` sceglierà l&#39;offerta migliore da consegnare ai tuoi clienti.

1. Da **[!UICONTROL Content Components]** trascinare e rilasciare il componente **[!UICONTROL Offer decision]** in un **[!UICONTROL Structure component]**.

1. Fai clic su **[!UICONTROL Add]** per selezionare **[!UICONTROL Offer decision]**.

   SCHERMATA

1. Selezionare **[!UICONTROL Placements]** dall&#39;elenco a discesa.  Quindi, seleziona **[!UICONTROL Offer decision]** da aggiungere al contenuto e fai clic su **[!UICONTROL Add]**.

   SCHERMATA

1. Dalla scheda **[!UICONTROL Offer decision]**, puoi visualizzare in anteprima o modificare l&#39;offerta inserita.

Scopri come aggiungere offerte personalizzate in un messaggio e-mail in `[this section](add-offers-email.md)`.

>[!IMPORTANT]
>
>Se vengono apportate modifiche a una decisione di offerta utilizzata in un messaggio di un percorso, devi annullare la pubblicazione del percorso e ripubblicarlo.  In questo modo le modifiche verranno incorporate nel messaggio del percorso e il messaggio sarà coerente con gli ultimi aggiornamenti.
