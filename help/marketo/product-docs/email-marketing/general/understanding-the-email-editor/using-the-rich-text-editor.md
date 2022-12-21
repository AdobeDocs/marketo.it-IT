---
unique-page-id: 2953419
description: Utilizzo dell’editor Rich Text - Marketo Docs - Documentazione del prodotto
title: Utilizzo dell’editor Rich Text
exl-id: 9b2d6d41-f947-4859-aad9-a10c15eb013a
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '736'
ht-degree: 1%

---

# Utilizzo dell’editor Rich Text {#using-the-rich-text-editor}

L’Editor Rich Text viene visualizzato in Marketo ed è disponibile ogni volta che desideri aggiungere o modificare contenuti. Ne vedrai una versione su pagine di destinazione, programmi, e-mail, moduli e snippet. Fai clic su **Modifica bozza** E salterà fuori per servirti.

## Impostazioni editor {#editor-settings}

L’impostazione dell’elemento del blocco principale definisce quali tag racchiudono il contenuto. Per impostazione predefinita, l’elemento del blocco principale e-mail utilizza `<p>` tag. Puoi modificare questa impostazione seguendo i passaggi seguenti.

>[!TIP]
>
>Sebbene sia possibile scegliere l’elemento del blocco principale, si consiglia sempre di utilizzare le impostazioni predefinite per la migliore esperienza utente.

1. Fai clic su **Amministratore**.

   ![](assets/one.png)

1. Fai clic su **E-mail**.

   ![](assets/two.png)

1. Fai clic su **Modifica impostazioni editor di testo**.

   ![](assets/three.png)

1. In **Editor e-mail/snippet** a discesa, seleziona `<div>` o Nessuno e fai clic su **Salva**. `<div>` viene utilizzato in questo esempio.

   ![](assets/four.png)

   Se `<div class=“mktEditable”></div>` in un modello e-mail, visualizzerai il seguente comportamento Origine HTML quando apri la sezione e digita &quot;Testo torna qui&quot; nell’editor:

<table> 
 <tbody> 
  <tr> 
   <th>&lt;p&gt;</th> 
   <th>&lt;div&gt;</th> 
   <th>Nessuna</th> 
  </tr> 
  <tr> 
   <td><p>&lt;div class="“mktEditable”"&gt;<br>&lt;p&gt;Testo visualizzato qui&lt;/p&gt;<br>&lt;/div&gt;</p></td> 
   <td><p>&lt;div class="“mktEditable”"&gt;<br>&lt;div&gt;Testo visualizzato qui&lt;/div&gt;<br>&lt;/div&gt;</p></td> 
   <td><p>&lt;div class="“mktEditable”"&gt;<br>Testo visualizzato qui<br>&lt;/div&gt;</p></td> 
  </tr> 
 </tbody> 
</table>

>[!TIP]
>
>Puoi anche modificare l’elemento del blocco principale dell’Editor pagina di destinazione seguendo gli stessi passaggi, ma facendo clic sul pulsante **Editor pagina di destinazione** al passaggio 4 anziché tramite e-mail/Editor snippet.

>[!NOTE]
>
>L’elemento del blocco principale è sempre `<p>` per token di programma rich-text.

## Funzioni {#features}

Di seguito sono elencate le funzioni disponibili in un editor Rich Text.

| Icona | Nome | Funzionamento |
|---|---|---|
| ![--](assets/image2015-7-9-10-3a23-3a24.png) | Famiglia di font | Scegli il tuo stile, ne abbiamo un sacco! |
| ![--](assets/image2015-7-9-10-3a22-3a11.png) | Dimensione font | Quanto la volete grande? 25 scelte, da 8 px a 90 px. |
| ![--](assets/image2015-7-9-10-3a59-3a4.png) | Stili | Scegli Paragrafo o sei stili di intestazione (per le pagine di destinazione). |
| ![--](assets/image2015-7-9-10-3a20-3a1.png) | Interlinea | Scegli la tua distanza tra le linee. |
| ![--](assets/image2015-7-9-10-3a25-3a52.png) | Colore testo | Nero, rosso o quello che vuoi. |
| ![--](assets/image2015-7-9-10-3a24-3a38.png) | Colore di sfondo | Evidenziazione dell&#39;enfasi. |
| ![--](assets/image2015-7-9-10-3a28-3a4.png) | Grassetto | **Più scuro e più spesso**. |
| ![--](assets/image2015-7-9-10-3a29-3a1.png) | Corsivo | *Angolato, per enfasi o virgolette* s. |
| ![--](assets/image2015-7-9-10-3a30-3a56.png) | Sottolineato | Inserisce una riga sotto il testo. |
| ![--](assets/image2015-7-9-10-3a31-3a57.png) | Allineamento | Utilizza questo menu a discesa per impostare il layout del testo e delle immagini. Centrali, scegli l&#39;allineamento a sinistra o a destra, o lo distribuisci al bordo con la giustificazione completa. |  | ![--](assets/image2015-7-9-10-3a32-3a47.png) | Elenco | Scegli punti elenco o numeri dal menu a discesa. I punti elenco sono buoni con elenchi e numeri con passaggi. |
| ![--](assets/image2015-7-9-10-3a38-3a0.png) | Rientro | Scegliere un rientro maggiore o minore. Utilizzare per i paragrafi o qualsiasi testo che si desidera evidenziare. |
| ![--](assets/image2015-7-9-10-3a38-3a58.png) | Inserisci/Modifica collegamento | inserire un link a un sito web o ad altri contenuti; apportare facilmente le modifiche desiderate. |
| ![--](assets/image2015-7-9-10-3a39-3a42.png) | Inserisci/Modifica immagine | Una foto vale mille parole. Mettetene uno. Fare clic sull&#39;icona della fotocamera per sfogliare Design Studio. È possibile rilasciare le immagini affiancate. |
| ![--](assets/image2015-7-9-10-3a40-3a36.png) | Inserisci token | Un potente strumento, ideale per la personalizzazione delle e-mail e il tracciamento dei dati. Assicurati di inserire un valore predefinito. |
| ![--](assets/image2015-7-9-10-3a41-3a21.png) | Annulla | Oops! Torniamo indietro e riproviamo. |
| ![--](assets/image2015-7-9-10-3a42-3a13.png) | Ripeti | Se va bene così com&#39;è, torna all&#39;originale. |
| ![--](assets/image2015-7-9-10-3a43-3a29.png) | Tabella | Costruisci il tuo, come questo. Un menu a discesa consente di configurarlo. |
| ![--](assets/image2015-7-9-10-3a45-3a1.png) | Inserisci ancoraggio | Ancoraggio a terra! |
| ![--](assets/image2015-7-9-10-3a45-3a48.png) | Linea orizzontale | Molti usi - Ottimo per dividere le sezioni. |
| ![--](assets/image2015-10-6-12-3a12-3a17.png) | Modifica HTML | Inserisce l’Editor sorgente di HTML per modificare il codice. |
| ![--](assets/image2015-7-9-10-3a47-3a36.png) | Pedice | Lettere poco sporgenti (come in O`<sub>2</sub>`). |
| ![--](assets/image2015-7-9-10-3a48-3a35.png) | Apice | Hai il potere! (2`<sup>6</sup>`). |
| ![--](assets/image2015-7-9-10-3a49-3a31.png) | Barrato | `<s>Put a line through text, like this</s>`. |
| ![--](assets/image2015-7-9-10-3a50-3a11.png) | Carattere speciale | Vuoi parlare di euro? Matematica? Hai 243 scelte. |
| ![--](assets/image2015-7-9-10-3a52-3a26.png) | Trova e sostituisci | Cerca e cambia le cose molto più velocemente che cercare ogni istanza da solo. |
| ![--](assets/image2015-7-9-10-3a53-3a37.png) | Cancella formattazione | Restituisci le cose allo standard. |
| ![--](assets/image2015-7-9-10-3a55-3a2.png) | Annulla | Premi il pulsante per dire &quot;Lascia perdere&quot;. |
| ![--](assets/image2015-7-9-10-3a56-3a2.png) | Salva | Premi il pulsante per dire &quot;OK, mi piace.&quot; |

>[!TIP]
>
>È possibile modificare il HTML e il testo in schermate separate. Assicurati di fare clic su **Copia da HTML** sulla **Testo** e quindi **Salva** quindi il tuo testo corrisponde al tuo HTML.

>[!NOTE]
>
>Non sei limitato ai font nel menu a discesa. Puoi utilizzarne una non elencata accedendo al codice HTML. Tutti i font web sono supportati in Marketo, ma i font web non funzionano universalmente in tutti i client e-mail.

## Pagine di destinazione {#landing-pages}

L’impostazione dell’elemento del blocco principale definisce quali tag racchiudono il contenuto. Per impostazione predefinita, l’elemento del blocco principale della pagina di destinazione utilizza `<div>` tag. Puoi modificare questa impostazione seguendo i passaggi seguenti.

>[!TIP]
>
>Sebbene sia possibile scegliere l’elemento del blocco principale, si consiglia sempre di utilizzare le impostazioni predefinite per la migliore esperienza utente.

1. Fai clic su **Amministratore**.

   ![](assets/one.png)

1. Fai clic su **E-mail**.

   ![](assets/two.png)

1. Fai clic su **Modifica impostazioni editor di testo**.

   ![](assets/three.png)

1. In **Editor pagina di destinazione** a discesa, seleziona `<p>` o Nessuno e fai clic su **Salva**. `<p>` viene utilizzato in questo esempio.

   ![](assets/five.png)

   Ed è tutto!
