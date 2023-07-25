---
unique-page-id: 2953419
description: Utilizzo dell’Editor Rich Text - Documentazione di Marketo - Documentazione del prodotto
title: Utilizzo dell’Editor Rich Text
exl-id: 9b2d6d41-f947-4859-aad9-a10c15eb013a
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '736'
ht-degree: 1%

---

# Utilizzo dell’Editor Rich Text {#using-the-rich-text-editor}

L’editor Rich Text viene visualizzato in Marketo ed è disponibile ogni volta che desideri aggiungere o modificare contenuti. Ne vedrai una versione su pagine di destinazione, programmi, e-mail, moduli e snippet. Fai clic su **Modifica bozza** e salterà fuori per servirti.

## Impostazioni editor {#editor-settings}

L’impostazione dell’elemento del blocco principale definisce i tag che racchiudono il contenuto. Per impostazione predefinita, l’elemento del blocco principale e-mail utilizza `<p>` tag. Puoi modificare questa impostazione seguendo la procedura descritta di seguito.

>[!TIP]
>
>Anche se puoi scegliere l’elemento del blocco principale, ti consigliamo sempre di utilizzare le impostazioni predefinite per una migliore esperienza utente.

1. Clic **Amministratore**.

   ![](assets/one.png)

1. Clic **E-mail**.

   ![](assets/two.png)

1. Clic **Modifica impostazioni editor di testo**.

   ![](assets/three.png)

1. In **Editor e-mail/snippet** a discesa, seleziona `<div>` o Nessuno e fai clic su **Salva**. `<div>` in questo esempio.

   ![](assets/four.png)

   Se è stato `<div class=“mktEditable”></div>` In un Modello e-mail, quando apri la sezione e digiti &quot;Text Goes Here&quot; nell’editor, visualizzerai il seguente comportamento HTML Source:

<table> 
 <tbody> 
  <tr> 
   <th>&lt;p&gt;</th> 
   <th>&lt;div&gt;</th> 
   <th>Nessuna</th> 
  </tr> 
  <tr> 
   <td><p>&lt;div class="“mktEditable”"&gt;<br>&lt;p&gt;Il testo va qui&lt;/p&gt;<br>&lt;/div&gt;</p></td> 
   <td><p>&lt;div class="“mktEditable”"&gt;<br>&lt;div&gt;Il testo va qui&lt;/div&gt;<br>&lt;/div&gt;</p></td> 
   <td><p>&lt;div class="“mktEditable”"&gt;<br>Il testo va qui<br>&lt;/div&gt;</p></td> 
  </tr> 
 </tbody> 
</table>

>[!TIP]
>
>È inoltre possibile modificare l’elemento del blocco principale dell’Editor pagina di destinazione seguendo gli stessi passaggi, ma facendo clic su **Editor pagina di destinazione** al passaggio 4 invece di E-mail/Editor snippet.

>[!NOTE]
>
>L’elemento del blocco principale è sempre `<p>` per token di programmi rich-text.

## Funzioni {#features}

Di seguito sono elencate le funzioni disponibili in un editor Rich Text.

| Icona | Nome | Funzionamento |
|---|---|---|
| ![--](assets/image2015-7-9-10-3a23-3a24.png) | Famiglia font | Scegli il tuo stile. Ce n&#39;è un sacco! |
| ![--](assets/image2015-7-9-10-3a22-3a11.png) | Dimensione font | Quanto la volete grande? 25 opzioni, da 8 a 90 px. |
| ![--](assets/image2015-7-9-10-3a59-3a4.png) | Stili | Scegliere Paragrafo o sei stili Titolo (per le pagine di destinazione). |
| ![--](assets/image2015-7-9-10-3a20-3a1.png) | Interlinea | Scegliete la distanza tra le linee. |
| ![--](assets/image2015-7-9-10-3a25-3a52.png) | Colore testo | Nero, rosso o qualsiasi altra cosa tu voglia. |
| ![--](assets/image2015-7-9-10-3a24-3a38.png) | Colore di sfondo | Evidenzia per enfasi. |
| ![--](assets/image2015-7-9-10-3a28-3a4.png) | Bold | **Più scuro e più spesso**. |
| ![--](assets/image2015-7-9-10-3a29-3a1.png) | Corsivo | *Angolato, per enfasi o citazione* s. |
| ![--](assets/image2015-7-9-10-3a30-3a56.png) | Sottolinea | Inserisce una riga sotto il testo. |
| ![--](assets/image2015-7-9-10-3a31-3a57.png) | Allineamento | Utilizza questo menu a discesa per disporre il testo e le immagini. Centrali, scegliete l&#39;allineamento a sinistra o a destra oppure distribuite il bordo allo spigolo con una giustificazione completa. |  | ![--](assets/image2015-7-9-10-3a32-3a47.png) | Elenco | Scegli punti elenco o numeri dal menu a discesa. Gli elenchi puntati sono utili per elenchi e numeri con passaggi. |
| ![--](assets/image2015-7-9-10-3a38-3a0.png) | Rientro | Scegli un rientro maggiore o minore. Utilizzare per i paragrafi o per qualsiasi testo che si desidera evidenziare. |
| ![--](assets/image2015-7-9-10-3a38-3a58.png) | Inserisci/Modifica collegamento | Inserisci un collegamento a un sito web o a un altro contenuto; apporta facilmente modifiche. |
| ![--](assets/image2015-7-9-10-3a39-3a42.png) | Inserisci/Modifica immagine | Un&#39;immagine vale mille parole. Rilasciane uno. Fare clic sull&#39;icona della fotocamera per sfogliare Design Studio. È possibile inserire le immagini una accanto all&#39;altra. |
| ![--](assets/image2015-7-9-10-3a40-3a36.png) | Inserisci token | Uno strumento potente, ottimo per la personalizzazione e-mail e il tracciamento dei dati. Assicurati di immettere un valore predefinito. |
| ![--](assets/image2015-7-9-10-3a41-3a21.png) | Annulla | Ops! Torniamo indietro di un passo e riproviamo. |
| ![--](assets/image2015-7-9-10-3a42-3a13.png) | Ripeti | Se va davvero bene così com&#39;è, torna all&#39;originale. |
| ![--](assets/image2015-7-9-10-3a43-3a29.png) | Tabella | Costruisci il tuo, come questo. Un menu a discesa consente di configurarlo. |
| ![--](assets/image2015-7-9-10-3a45-3a1.png) | Inserisci ancoraggio | Rilascia l&#39;ancora! |
| ![--](assets/image2015-7-9-10-3a45-3a48.png) | Linea orizzontale | Molti utilizzi: ottimo per la divisione delle sezioni. |
| ![--](assets/image2015-10-6-12-3a12-3a17.png) | Modifica HTML | Attiva l&#39;Editor origine HTML per modificare il codice. |
| ![--](assets/image2015-7-9-10-3a47-3a36.png) | Pedice | Lettere poco sporgenti (come in O`<sub>2</sub>`). |
| ![--](assets/image2015-7-9-10-3a48-3a35.png) | Apice | Hai il potere! (2`<sup>6</sup>`). |
| ![--](assets/image2015-7-9-10-3a49-3a31.png) | Barrato | `<s>Put a line through text, like this</s>`. |
| ![--](assets/image2015-7-9-10-3a50-3a11.png) | Carattere speciale | Vuoi parlare di euro? Matematica? Hai 243 scelte. |
| ![--](assets/image2015-7-9-10-3a52-3a26.png) | Trova e sostituisci | Cerca e modifica le cose molto più rapidamente rispetto alla ricerca di ogni istanza. |
| ![--](assets/image2015-7-9-10-3a53-3a37.png) | Cancella formattazione | Ripristina gli standard. |
| ![--](assets/image2015-7-9-10-3a55-3a2.png) | Annulla | Premi il pulsante per dire, &quot;Non importa&quot;. |
| ![--](assets/image2015-7-9-10-3a56-3a2.png) | Salva | Premete il pulsante per dire &quot;OK, mi piace&quot;. |

>[!TIP]
>
>Puoi modificare il HTML e il testo su schermate separate. Assicurati di fare clic su **Copia da HTML** il **Testo** e quindi **Salva** in modo che il testo corrisponda al HTML.

>[!NOTE]
>
>Non sei limitato ai font presenti nel menu a discesa. Per utilizzarne uno non elencato, accedi al codice HTML. Tutti i tipi di carattere Web sono supportati in Marketo, ma i tipi di carattere Web non funzionano in modo universale in tutti i client di posta elettronica.

## Pagine di destinazione {#landing-pages}

L’impostazione dell’elemento del blocco principale definisce i tag che racchiudono il contenuto. Per impostazione predefinita, l’elemento del blocco principale della pagina di destinazione utilizza `<div>` tag. Per modificare questa impostazione, segui la procedura riportata di seguito.

>[!TIP]
>
>Anche se puoi scegliere l’elemento del blocco principale, ti consigliamo sempre di utilizzare le impostazioni predefinite per una migliore esperienza utente.

1. Clic **Amministratore**.

   ![](assets/one.png)

1. Clic **E-mail**.

   ![](assets/two.png)

1. Clic **Modifica impostazioni editor di testo**.

   ![](assets/three.png)

1. In **Editor pagina di destinazione** a discesa, seleziona `<p>` o Nessuno e fai clic su **Salva**. `<p>` in questo esempio.

   ![](assets/five.png)

   Ed è tutto!
