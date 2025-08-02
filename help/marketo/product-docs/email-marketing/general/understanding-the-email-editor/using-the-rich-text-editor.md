---
unique-page-id: 2953419
description: Utilizzo dell’Editor Rich Text - Documentazione di Marketo - Documentazione del prodotto
title: Utilizzo dell’Editor Rich Text
exl-id: 9b2d6d41-f947-4859-aad9-a10c15eb013a
feature: Email Editor
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '659'
ht-degree: 1%

---

# Utilizzo dell’Editor Rich Text {#using-the-rich-text-editor}

L’editor Rich Text viene visualizzato in Marketo ed è disponibile ogni volta che desideri aggiungere o modificare contenuti. Ne vedrai una versione su pagine di destinazione, programmi, e-mail, moduli e snippet. Fai clic su **[!UICONTROL Edit Draft]** per visualizzarlo.

## Impostazioni editor {#editor-settings}

L’impostazione dell’elemento del blocco principale definisce i tag che racchiudono il contenuto. Per impostazione predefinita, l&#39;elemento blocco radice e-mail utilizza `<p>` tag. Puoi modificare questa impostazione seguendo la procedura descritta di seguito.

>[!TIP]
>
>Anche se puoi scegliere l’elemento del blocco principale, ti consigliamo sempre di utilizzare le impostazioni predefinite per una migliore esperienza utente.

1. Fai clic su **[!UICONTROL Admin]**.

   ![](assets/one.png)

1. Fai clic su **[!UICONTROL Email]**.

   ![](assets/two.png)

1. Fai clic su **[!UICONTROL Edit Text Editor Settings]**.

   ![](assets/three.png)

1. Nel menu a discesa **[!UICONTROL Email]/[!UICONTROL Snippet Editor]**, selezionare `<div>` o [!UICONTROL None] e fare clic su **[!UICONTROL Save]**. `<div>` è utilizzato in questo esempio.

   ![](assets/four.png)

   Se hai `<div class=“mktEditable”></div>` in un Modello e-mail, visualizzerai il seguente comportamento di HTML Source quando apri la sezione e digiti &quot;Text Goes Here&quot; nell&#39;editor:

<table>
 <tbody>
  <tr>
   <th>&lt;p&gt;</th>
   <th>&lt;div&gt;</th>
   <th>Nessuna</th>
  </tr>
  <tr>
   <td><p>&lt;div class="mktEditable"&gt;<br>&lt;p&gt;Il testo va qui&lt;/p&gt;<br>&lt;/div&gt;</p></td>
   <td><p>&lt;div class="mktEditable"&gt;<br>&lt;div&gt;Il testo va qui&lt;/div&gt;<br>&lt;/div&gt;</p></td>
   <td><p>&lt;div class="mktEditable"&gt;<br>Testo da inserire<br>&lt;/div&gt;</p></td>
  </tr>
 </tbody>
</table>

>[!TIP]
>
>È inoltre possibile modificare l&#39;elemento del blocco principale dell&#39;Editor pagina di destinazione seguendo gli stessi passaggi, ma facendo clic sull&#39;elenco a discesa **[!UICONTROL Landing Page Editor]** nel passaggio 4 anziché su [!UICONTROL Email] / [!UICONTROL Snippet Editor].

>[!NOTE]
>
>L&#39;elemento del blocco radice è sempre `<p>` per i token del programma Rich Text.

## Funzioni {#features}

Di seguito sono elencate le funzioni disponibili in un editor Rich Text.

| Icona | Nome | Funzionamento |
|---|---|---|
| ![—](assets/image2015-7-9-10-3a23-3a24.png) | [!UICONTROL Font Family] | Scegli il tuo stile. Ce n&#39;è un sacco! |
| ![—](assets/image2015-7-9-10-3a22-3a11.png) | [!UICONTROL Font Size] | Quanto la volete grande? 25 opzioni, da 8 a 90 px. |
| ![—](assets/image2015-7-9-10-3a59-3a4.png) | [!UICONTROL Styles] | Scegliere Paragrafo o sei stili Titolo (per le pagine di destinazione). |
| ![—](assets/image2015-7-9-10-3a20-3a1.png) | [!UICONTROL Line Spacing] | Scegliete la distanza tra le linee. |
| ![—](assets/image2015-7-9-10-3a25-3a52.png) | [!UICONTROL Text Color] | Nero, rosso o qualsiasi altra cosa tu voglia. |
| ![—](assets/image2015-7-9-10-3a24-3a38.png) | [!UICONTROL Background Color] | Evidenzia per enfasi. |
| ![—](assets/image2015-7-9-10-3a28-3a4.png) | [!UICONTROL Bold] | **Più scuro e più spesso**. |
| ![—](assets/image2015-7-9-10-3a29-3a1.png) | [!UICONTROL Italic] | *Angolato, per enfasi o offerta*. |
| ![—](assets/image2015-7-9-10-3a30-3a56.png) | [!UICONTROL Underline] | Inserisce una riga sotto il testo. |
| ![—](assets/image2015-7-9-10-3a31-3a57.png) | [!UICONTROL Alignment] | Utilizza questo menu a discesa per disporre il testo e le immagini. Centrali, scegliete l&#39;allineamento a sinistra o a destra oppure distribuite il bordo allo spigolo con una giustificazione completa. |  | ![—](assets/image2015-7-9-10-3a32-3a47.png) | Elenco | Scegli punti elenco o numeri dal menu a discesa. Gli elenchi puntati sono utili per elenchi e numeri con passaggi. |
| ![—](assets/image2015-7-9-10-3a38-3a0.png) | [!UICONTROL Indent] | Scegli un rientro maggiore o minore. Utilizzare per i paragrafi o per qualsiasi testo che si desidera evidenziare. |
| ![—](assets/image2015-7-9-10-3a38-3a58.png) | [!UICONTROL Insert/Edit Link] | Inserisci un collegamento a un sito web o a un altro contenuto; apporta facilmente modifiche. |
| ![—](assets/image2015-7-9-10-3a39-3a42.png) | [!UICONTROL Insert/Edit Image] | Un&#39;immagine vale mille parole. Rilasciane uno. Fare clic sull&#39;icona della fotocamera per sfogliare Design Studio. È possibile inserire le immagini una accanto all&#39;altra. |
| ![—](assets/image2015-7-9-10-3a40-3a36.png) | [!UICONTROL Insert Token] | Uno strumento potente, ottimo per la personalizzazione e-mail e il tracciamento dei dati. Assicurati di immettere un valore predefinito. |
| ![—](assets/image2015-7-9-10-3a41-3a21.png) | [!UICONTROL Undo] | Ops! Torniamo indietro di un passo e riproviamo. |
| ![—](assets/image2015-7-9-10-3a42-3a13.png) | [!UICONTROL Redo] | Se va davvero bene così com&#39;è, torna all&#39;originale. |
| ![—](assets/image2015-7-9-10-3a43-3a29.png) | [!UICONTROL Table] | Costruisci il tuo, come questo. Un menu a discesa consente di configurarlo. |
| ![—](assets/image2015-7-9-10-3a45-3a1.png) | [!UICONTROL Insert Anchor] | Rilascia l&#39;ancora! |
| ![—](assets/image2015-7-9-10-3a45-3a48.png) | [!UICONTROL Horizontal Line] | Molti utilizzi: ottimo per la divisione delle sezioni. |
| ![—](assets/image2015-10-6-12-3a12-3a17.png) | [!UICONTROL Edit HTML] | Attiva HTML Source Editor per modificare il codice. |
| ![—](assets/image2015-7-9-10-3a47-3a36.png) | [!UICONTROL Subscript] | Lettere poco sporgenti (come in O`<sub>2</sub>`). |
| ![—](assets/image2015-7-9-10-3a48-3a35.png) | [!UICONTROL Superscript] | Hai il potere! (2`<sup>6</sup>`). |
| ![—](assets/image2015-7-9-10-3a49-3a31.png) | [!UICONTROL Strikethrough] | `<s>Put a line through text, like this</s>`. |
| ![—](assets/image2015-7-9-10-3a50-3a11.png) | [!UICONTROL Special Character] | Vuoi parlare di euro? Matematica? Hai 243 scelte. |
| ![—](assets/image2015-7-9-10-3a52-3a26.png) | [!UICONTROL Find and Replace] | Cerca e modifica le cose molto più rapidamente rispetto alla ricerca di ogni istanza. |
| ![—](assets/image2015-7-9-10-3a53-3a37.png) | [!UICONTROL Clear Formatting] | Ripristina gli standard. |
| ![—](assets/image2015-7-9-10-3a55-3a2.png) | [!UICONTROL Cancel] | Premi il pulsante per dire, &quot;Non importa&quot;. |
| ![—](assets/image2015-7-9-10-3a56-3a2.png) | [!UICONTROL Save] | Premete il pulsante per dire &quot;OK, mi piace&quot;. |

>[!TIP]
>
>Puoi modificare il HTML e il testo su schermate separate. Assicurarsi di fare clic su **[!UICONTROL Copy from HTML]** nella scheda **[!UICONTROL Text]** e quindi su **[!UICONTROL Save]** in modo che il testo corrisponda al HTML.

>[!NOTE]
>
>Non sei limitato ai font presenti nel menu a discesa. Per utilizzarne uno non elencato, accedi al codice HTML. Tutti i tipi di carattere Web sono supportati in Marketo, ma i tipi di carattere Web non funzionano in modo universale in tutti i client di posta elettronica.

## Pagine di destinazione {#landing-pages}

L’impostazione dell’elemento del blocco principale definisce i tag che racchiudono il contenuto. Per impostazione predefinita, l&#39;elemento del blocco principale della pagina di destinazione utilizza `<div>` tag. Per modificare questa impostazione, segui la procedura riportata di seguito.

>[!TIP]
>
>Anche se puoi scegliere l’elemento del blocco principale, ti consigliamo sempre di utilizzare le impostazioni predefinite per una migliore esperienza utente.

1. Fai clic su **[!UICONTROL Admin]**.

   ![](assets/one.png)

1. Fai clic su **[!UICONTROL Email]**.

   ![](assets/two.png)

1. Fai clic su **[!UICONTROL Edit Text Editor Settings]**.

   ![](assets/three.png)

1. Nel menu a discesa **[!UICONTROL Landing Page Editor]**, selezionare `<p>` o [!UICONTROL None] e fare clic su **[!UICONTROL Save]**. `<p>` è utilizzato in questo esempio.

   ![](assets/five.png)

   Ed è tutto!
