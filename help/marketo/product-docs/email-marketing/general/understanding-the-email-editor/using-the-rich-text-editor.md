---
unique-page-id: 2953419
description: Utilizzo dell'Editor Rich Text - Marketo Docs - Documentazione prodotto
title: Utilizzo dell’editor Rich Text
translation-type: tm+mt
source-git-commit: c33b7ab59e612f37d3f64bb954579700dc574068
workflow-type: tm+mt
source-wordcount: '736'
ht-degree: 0%

---


# Utilizzo dell&#39;editor Rich Text {#using-the-rich-text-editor}

L’Editor Rich Text (RTE) viene visualizzato in tutto Marketo ed è disponibile ogni volta che si desidera aggiungere o modificare contenuti. Una versione di questo file verrà visualizzata nelle pagine di destinazione, nei programmi, nelle e-mail, nei moduli e negli snippet. Basta fare clic su **Modifica bozza** e verrà visualizzato per servirti.

## Impostazioni editor {#editor-settings}

L&#39;impostazione dell&#39;elemento blocco principale definisce quali tag racchiudono il contenuto. Per impostazione predefinita, l&#39;elemento blocco radice e-mail utilizza <p> tag. È possibile modificare tale impostazione seguendo la procedura riportata di seguito.

>[!TIP]
>
>Sebbene sia disponibile l&#39;opzione per scegliere l&#39;elemento blocco principale, si consiglia sempre di utilizzare le impostazioni predefinite per garantire la migliore esperienza utente.

1. Fare clic su **Admin**.

   ![](assets/one.png)

1. Fare clic su **E-mail**.

   ![](assets/two.png)

1. Fare clic su **Modifica impostazioni editor di testo**.

   ![](assets/three.png)

1. Nel menu a discesa **E-mail / Editor snippet**, selezionare <div> oppure Nessuno e fare clic su **Salva**. <div> viene utilizzato in questo esempio.

   ![](assets/four.png)

   Se <div class="&ldquo;mktEditable&rdquo;"></div> in un modello e-mail, all’apertura della sezione viene visualizzato il seguente comportamento Sorgente HTML e digitare &quot;Text Goes Here&quot; nell’editor:

<table> 
 <tbody> 
  <tr> 
   <th>&lt;p&gt;</th> 
   <th>&lt;div&gt;</th> 
   <th>None</th> 
  </tr> 
  <tr> 
   <td><p>&lt;div class="“mktEditable”"&gt;<br>&lt;p&gt;Testo da inserire qui&lt;/p&gt;<br>&lt;/div&gt;</p></td> 
   <td><p>&lt;div class="“mktEditable”"&gt;<br>&lt;div&gt;Testo da inserire qui&lt;/div&gt;<br>&lt;/div&gt;</p></td> 
   <td><p>&lt;div class="“mktEditable”"&gt;<br>Testo da inserire qui<br>&lt;/div&gt;</p></td> 
  </tr> 
 </tbody> 
</table>

>[!TIP]
>
>È inoltre possibile modificare l&#39;elemento blocco principale dell&#39;Editor pagina di destinazione seguendo gli stessi passaggi, ma facendo clic sul menu a discesa **Editor pagina di destinazione** al punto 4 anziché nell&#39;Editor di e-mail/snippet.

>[!NOTE]
>
>L&#39;elemento blocco principale è sempre <p> per token di programma RTF.

## Caratteristiche {#features}

Queste sono le caratteristiche che troverete in un editor Rich Text.

| Icona | Nome | Azioni |
|---|---|---|
| ![—](assets/image2015-7-9-10-3a23-3a24.png) | Famiglia di font | Scegli il tuo stile, ce ne sono molti! |
| ![—](assets/image2015-7-9-10-3a22-3a11.png) | Dimensione font | Quanto la vuoi grande? 25 opzioni, da 8 px a 90 px. |
| ![—](assets/image2015-7-9-10-3a59-3a4.png) | Stili | Scegliete Paragrafo o sei stili di titolo (per le pagine di destinazione). |
| ![—](assets/image2015-7-9-10-3a20-3a1.png) | Interlinea | Scegli la tua distanza tra le righe. |
| ![—](assets/image2015-7-9-10-3a25-3a52.png) | Colore testo | Nero, rosso o quello che vuoi. |
| ![—](assets/image2015-7-9-10-3a24-3a38.png) | Colore di sfondo | Evidenziazione per l&#39;enfasi. |
| ![—](assets/image2015-7-9-10-3a28-3a4.png) | Grassetto | **Più scuro e più spesso**. |
| ![—](assets/image2015-7-9-10-3a29-3a1.png) | Corsivo | *Angolato, per enfasi o* virgolette. |
| ![—](assets/image2015-7-9-10-3a30-3a56.png) | Sottolineato | Inserisce una riga sotto il testo. |
| ![—](assets/image2015-7-9-10-3a31-3a57.png) | Allineamento | Utilizzate questo menu a discesa per disporre il testo e le immagini. Centrali, scegli l’allineamento a sinistra o a destra, oppure distribuisci il bordo al bordo con la giustificazione completa. |  | ![—](assets/image2015-7-9-10-3a32-3a47.png) | Elenco | Scegliete i punti elenco o i numeri dal menu a discesa. I puntini sono buoni con elenchi e numeri con passaggi. |
| ![—](assets/image2015-7-9-10-3a38-3a0.png) | Rientro | Scegliete un rientro maggiore o minore. Utilizzare per i paragrafi o qualsiasi testo da evidenziare. |
| ![—](assets/image2015-7-9-10-3a38-3a58.png) | Inserisci/Modifica collegamento | Inserire un collegamento a un sito Web o ad altri contenuti; apportare facilmente modifiche. |
| ![—](assets/image2015-7-9-10-3a39-3a42.png) | Inserisci/Modifica immagine | Un&#39;immagine vale mille parole. Rilasciatene uno. Fate clic sull&#39;icona della fotocamera per sfogliare Design Studio. Potete inserire le immagini affiancate. |
| ![—](assets/image2015-7-9-10-3a40-3a36.png) | Inserisci token | Un potente strumento, ideale per la personalizzazione delle e-mail e il tracciamento dei dati. Assicuratevi di inserire un valore predefinito. |
| ![—](assets/image2015-7-9-10-3a41-3a21.png) | Annulla | Oops! Torniamo indietro e riproviamo. |
| ![—](assets/image2015-7-9-10-3a42-3a13.png) | Ripristina | Se va bene così, tornate all&#39;originale. |
| ![—](assets/image2015-7-9-10-3a43-3a29.png) | Tabella | Costruisci il tuo, come questo. Un menu a discesa consente di configurarlo. |
| ![—](assets/image2015-7-9-10-3a45-3a1.png) | Inserisci ancoraggio | Ancoraggio rilascio! |
| ![—](assets/image2015-7-9-10-3a45-3a48.png) | Linea orizzontale | Molti usi - Ottimo per dividere le sezioni. |
| ![—](assets/image2015-10-6-12-3a12-3a17.png) | Modifica HTML | Inserisce l’Editor sorgente HTML per modificare il codice. |
| ![—](assets/image2015-7-9-10-3a47-3a36.png) | Pedice | Lettere sporgenti (come in O`<sub>2</sub>`). |
| ![—](assets/image2015-7-9-10-3a48-3a35.png) | Apice | Hai il potere! (2`<sup>6</sup>`). |
| ![—](assets/image2015-7-9-10-3a49-3a31.png) | Barrato | `<s>Put a line through text, like this</s>`. |
| ![—](assets/image2015-7-9-10-3a50-3a11.png) | Carattere speciale | Vuoi parlare di euro? Matematica? Hai 243 scelte. |
| ![—](assets/image2015-7-9-10-3a52-3a26.png) | Trova e sostituisci | Cercare e cambiare le cose molto più velocemente che cercare ogni singola istanza. |
| ![—](assets/image2015-7-9-10-3a53-3a37.png) | Cancella formattazione | Riporta le cose allo standard. |
| ![—](assets/image2015-7-9-10-3a55-3a2.png) | Annulla | Premere il tasto per dire &quot;Lascia perdere&quot;. |
| ![—](assets/image2015-7-9-10-3a56-3a2.png) | Salva | Premere il pulsante per dire, &quot;OK, mi piace.&quot; |

>[!TIP]
>
>Potete modificare il codice HTML e il testo su schermate separate. Accertatevi di fare clic su **Copia da HTML** nella scheda **Testo**, quindi su **Salva** in modo che il testo corrisponda al codice HTML.

>[!NOTE]
>
>L&#39;utente non è limitato ai font presenti nel menu a discesa. Potete utilizzarne uno non elencato accedendo al codice HTML. Tutti i font Web sono supportati in Marketo, ma i font Web non funzionano universalmente in tutti i client e-mail.

## Pagine di destinazione {#landing-pages}

L&#39;impostazione dell&#39;elemento blocco principale definisce quali tag racchiudono il contenuto. Per impostazione predefinita, l&#39;elemento blocco principale della pagina di destinazione utilizza <div> tag. È possibile modificare tale impostazione seguendo la procedura riportata di seguito.

>[!TIP]
>
>Sebbene sia disponibile l&#39;opzione per scegliere l&#39;elemento blocco principale, si consiglia sempre di utilizzare le impostazioni predefinite per garantire la migliore esperienza utente.

1. Fare clic su **Admin**.

   ![](assets/one.png)

1. Fare clic su **E-mail**.

   ![](assets/two.png)

1. Fare clic su **Modifica impostazioni editor di testo**.

   ![](assets/three.png)

1. Nel menu a discesa **Editor pagina di destinazione**, selezionare <p> oppure Nessuno e fare clic su **Salva**. <p> viene utilizzato in questo esempio.

   ![](assets/five.png)

   Ed è tutto!

