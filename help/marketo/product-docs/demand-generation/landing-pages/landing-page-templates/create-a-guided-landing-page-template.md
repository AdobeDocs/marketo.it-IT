---
unique-page-id: 7515401
description: Creare un modello di pagina di destinazione guidata - Documenti Marketo - Documentazione del prodotto
title: Creare un modello di pagina di destinazione guidata
exl-id: 7d097162-d862-4d09-9440-aba1628450c2
source-git-commit: c309b69198c6f61d7475c6d3a6b1672e045b9b4a
workflow-type: tm+mt
source-wordcount: '1254'
ht-degree: 0%

---

# Creare un modello di pagina di destinazione guidata {#create-a-guided-landing-page-template}

I modelli delle pagine di destinazione guidati hanno una sintassi particolare. Utilizza questa sintassi per specificare cosa è personalizzabile e dove termina il contenuto in ogni pagina di destinazione creata a partire dal modello. Solo le aree o variabili specificate come modificabili saranno disponibili per la personalizzazione nell’editor pagina di destinazione &quot;Guidata&quot;.

>[!TIP]
>
>Utilizza buone convenzioni di denominazione e il tuo team marketing si innamorerà di te.

Esistono due modi per dichiarare che un elemento della pagina deve essere modificabile:

* Dichiara un oggetto come &quot;elemento&quot;. Il creatore della pagina di destinazione potrà aggiungere immagini, testo o risorse Marketo nelle aree specificate.
* Dichiara una stringa come &quot;variabile&quot;. Il creatore della pagina di destinazione sarà in grado di sostituire tale variabile con una stringa, un colore o uno stato booleano da una leva true/false.

## Elementi modificabili {#editable-elements}

Gli elementi vengono dichiarati aggiungendo un normale elemento DOM al modello, quindi decorando l’elemento con un nome di classe specifico per Marketo.

## Testo {#text}

Se definisci un’area come RTF, gli utenti potranno modificarne il contenuto [utilizzo dell’editor Rich Text di Marketo](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md).

Attributi richiesti:\
**Classe**: &quot;mktoText&quot;\
**id**: Stringa ID. Contiene solo lettere, numeri, trattino &quot;-&quot; e trattino basso &quot;_&quot;. Non sono consentiti spazi. Deve essere univoco.\
**mktoName** : Stringa. Questo è il nome visualizzato che verrà mostrato nell’editor delle pagine di destinazione. Si consiglia di utilizzare un nome descrittivo.

Facoltativo:\
Il contenuto di un elemento con classe mktoText (se fornito) verrà utilizzato come valore predefinito per l’area modificabile.

Esempio:

`<pre data-theme="Confluence"><div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area.</div></pre>`

## Immagine {#image}

Sono disponibili due opzioni per la definizione degli elementi immagine modificabili. Puoi utilizzare una delle due opzioni `<div>`, che specifica un contenitore in cui verrà inserita l’immagine, o un `<img>` tag .

## Opzione 1 - Utilizza un `<div>` {#option-use-a-div}

Attributi richiesti:

Classe: &quot;mktoImg&quot;\
id: Stringa ID. Contiene solo lettere, numeri, trattino &quot;-&quot; e trattino basso &quot;_&quot;. Non sono consentiti spazi. Deve essere univoco.\
mktoName : Stringa. Questo è il nome visualizzato che verrà mostrato nell’editor delle pagine di destinazione. Si consiglia di utilizzare un nome descrittivo.

Facoltativo:\
mktoImgClass: Stringa. Il valore qui verrà aggiunto all&#39;attributo class del `<img>` all’interno del div.

Esempio:

`<pre data-theme="Confluence"><div class="mktoImg" id="exampleImg" mktoName="Example Image"></div></pre>`

## Opzione 2 - Utilizza un `<img>` {#option-use-a-img}

Attributi richiesti:\
Classe: &quot;mktoImg&quot;\
id: Stringa ID. Contiene solo lettere, numeri, trattino &quot;-&quot; e trattino basso &quot;_&quot;. Non sono consentiti spazi. Deve essere univoco.\
mktoName : Stringa. Questo è il nome visualizzato che verrà mostrato nell’editor delle pagine di destinazione. Si consiglia di utilizzare un nome descrittivo.

Facoltativo:\
src: URL stringa. Viene utilizzato come valore predefinito per l’immagine.

Esempio:

`<pre data-theme="Confluence"><img class="mktoImg" id="exampleImg" mktoName="Example Image"></pre>`

>[!NOTE]
>
>Quando utilizzi `<img>` Il HTML renderizzato conterrà un wrapper div generato intorno alla `<img>` tag . Sarà impostato su class .&quot;mktoImg.mktoGen,&quot; e sarà display:inline-block.

## Modulo {#form}

Esempio:Attributi richiesti:\
**Classe**: &quot;mktoForm&quot;\
**id**: Stringa ID. Contiene solo lettere, numeri, trattino &quot;-&quot; e trattino basso &quot;_&quot;. Non sono consentiti spazi. Deve essere univoco.\
**mktoName** : Stringa. Questo è il nome visualizzato che verrà mostrato nell’editor delle pagine di destinazione. Si consiglia di utilizzare un nome descrittivo.

`<pre data-theme="Confluence"><div class="mktoForm" id="exampleForm" mktoName="Example Form"></div></pre>`

## Frammento {#snippet}

Attributi richiesti:\
**Classe**: &quot;mktoSnippet&quot;\
**id**: Stringa ID. Contiene solo lettere, numeri, trattino &quot;-&quot; e trattino basso &quot;_&quot;. Non sono consentiti spazi. Deve essere univoco.\
**mktoName** : Stringa. Questo è il nome visualizzato che verrà mostrato nell’editor delle pagine di destinazione. Si consiglia di utilizzare un nome descrittivo.

Esempio:

`<pre data-theme="Confluence"><div class="mktoSnippet" id="exampleSnippet" mktoName="Example Snippet"></div></pre>`

## Pulsante Condividi {#share-button}

Attributi richiesti:\
**Classe**: &quot;mktoShareButton&quot;\
**id**: Stringa ID. Contiene solo lettere, numeri, trattino &quot;-&quot; e trattino basso &quot;_&quot;. Non sono consentiti spazi. Deve essere univoco.\
**mktoName** : Stringa. Questo è il nome visualizzato che verrà mostrato nell’editor delle pagine di destinazione. Si consiglia di utilizzare un nome descrittivo.

Esempio:

`<pre data-theme="Confluence"><div class="mktoShareButton" id="exampleShareButton" mktoName="Example Share Button"></div></pre>`

## Video {#video}

>[!NOTE]
>
>Quando utilizzi l’elemento video in una pagina di destinazione, Marketo supporta solo i video provenienti da YouTube. Se utilizzi un altro servizio, ti consigliamo di utilizzare una casella di testo RTF e incollare nel codice di incorporamento del video.

Attributi richiesti:
**Classe**: &quot;mktoVideo&quot;
**id**: Stringa ID. Contiene solo lettere, numeri, trattino &quot;-&quot; e trattino basso &quot;_&quot;. Non sono consentiti spazi. Deve essere univoco.
**mktoName** : Stringa. Questo è il nome visualizzato che verrà mostrato nell’editor delle pagine di destinazione. Si consiglia di utilizzare un nome descrittivo.

Esempio:

`<pre data-theme="Confluence"><div class="mktoVideo" id="exampleVideo" mktoName="Example Video"></div></pre>`

## Sondaggio {#poll}

Attributi richiesti:\
**Classe**: &quot;mktoPoll&quot;\
**id**: Stringa ID. Contiene solo lettere, numeri, trattino &quot;-&quot; e trattino basso &quot;_&quot;. Non sono consentiti spazi. Deve essere univoco.\
**mktoName** : Stringa. Questo è il nome visualizzato che verrà mostrato nell’editor delle pagine di destinazione. Si consiglia di utilizzare un nome descrittivo.

Esempio:

`<pre data-theme="Confluence"><div class="mktoPoll" id="examplePoll" mktoName="Example Poll"></div></pre>`

## Riferimento {#referral}

Attributi richiesti:\
**Classe**: &quot;mktoReferral&quot;\
**id**: Stringa ID. Contiene solo lettere, numeri, trattino &quot;-&quot; e trattino basso &quot;_&quot;. Non sono consentiti spazi. Deve essere univoco.\
**mktoName** : Stringa. Questo è il nome visualizzato che verrà mostrato nell’editor delle pagine di destinazione. Si consiglia di utilizzare un nome descrittivo.

Esempio:

`<pre data-theme="Confluence"><div class="mktoReferral" id="exampleReferral" mktoName="Example Referral"></div></pre>`

## Lotterie {#sweepstakes}

Attributi richiesti:\
**Classe**: &quot;mktoSweepstakes&quot;\
**id**: Stringa ID. Contiene solo lettere, numeri, trattino &quot;-&quot; e trattino basso &quot;_&quot;. Non sono consentiti spazi. Deve essere univoco.\
**mktoName** : Stringa. Questo è il nome visualizzato che verrà mostrato nell’editor delle pagine di destinazione. Si consiglia di utilizzare un nome descrittivo.

Esempio:

`<pre data-theme="Confluence"><div class="mktoSweepstakes" id="exampleSweepstakes" mktoName="Example Sweepstakes"></div></pre>`

## Variabili modificabili {#editable-variables}

Tutti i tipi di variabili vengono utilizzati facendo riferimento al valore del relativo attributo id racchiuso all&#39;interno di una sequenza di caratteri ${ }. Possono essere utilizzati in qualsiasi punto del documento, ad eccezione dell’interno di altre dichiarazioni di variabili.

Esempio:

`<pre data-theme="Confluence">${var1}</pre>`

**Dichiarazione:**

Le variabili vengono dichiarate come meta tag all’interno di `<head>` elemento del modello. Sono disponibili tre tipi di variabili da utilizzare: Stringa, colore e booleana.

## Stringa {#string}

Attributi richiesti:\
**Classe** : &quot;mktoString&quot;,\
**id**: Stringa ID. Contiene solo lettere, numeri, trattino &quot;-&quot; e trattino basso &quot;_&quot;. Non sono consentiti spazi. Deve essere univoco.\
**mktoName** : Stringa. Questo è il nome visualizzato che verrà mostrato nell’editor delle pagine di destinazione. Si consiglia di utilizzare un nome descrittivo.

Facoltativo:\
**default**: Valore stringa per l&#39;attributo. Vuoto se non ne è stato fornito uno.\
**allowHtml**: &quot;true&quot; o &quot;false&quot;. Controlla se il valore verrà stampato senza l’escape di HTML. Predefinito su &quot;false&quot; se non impostato.

Esempio di base:

`<pre data-theme="Confluence"><meta class="mktoString" id="var1" mktoName="My Variable"></pre>`

Esempio con tutti gli attributi:

`<pre data-theme="Confluence"><meta class="mktoString" id="var1" mktoName="My Variable" default="This is my default value" allowHtml="true"></pre>`

## Colore {#color}

Attributi richiesti:\
**Classe** : &quot;mktoColor&quot;,\
**id**: Stringa ID. Contiene solo lettere, numeri, trattino &quot;-&quot; e trattino basso &quot;_&quot;. Non sono consentiti spazi. Deve essere univoco.\
**mktoName** : Stringa. Questo è il nome visualizzato che verrà mostrato nell’editor delle pagine di destinazione. Si consiglia di utilizzare un nome descrittivo.

Facoltativo:\
**default**: Codice a colori HEX a 7 cifre. Esempio: &quot;#336699&quot;

Esempio di base:

`<pre data-theme="Confluence"><meta class="mktoColor" id="color1" mktoName="My Color Variable"></pre>`

Esempio con tutti gli attributi:

`<pre data-theme="Confluence"><meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699"></pre>`

## Booleano {#boolean}

Attributi richiesti:\
**Classe** : &quot;mktoBoolean&quot;,\
**id**: Stringa ID. Contiene solo lettere, numeri, trattino &quot;-&quot; e trattino basso &quot;_&quot;. Non sono consentiti spazi. Deve essere univoco.\
**mktoName** : Stringa. Questo è il nome visualizzato che verrà mostrato nell’editor delle pagine di destinazione. Si consiglia di utilizzare un nome descrittivo.

Facoltativo:\
**default**: Stringa booleana. &quot;true&quot; o &quot;false&quot; controlla se il valore inizia nella posizione ON o OFF. &quot;false&quot; se non specificato.\
**false_value**: Stringa. Il valore da inserire per la variabile quando si trova in posizione OFF. &quot;false&quot; se non specificato.\
**true_value**: Stringa. Il valore da inserire per la variabile quando si trova nella posizione ON. &quot;true&quot; se non viene fornito.\
**false_value_name**: Stringa. Nome visualizzato nell’editor della pagina di destinazione quando il valore è in posizione OFF. &quot;OFF&quot; se non fornito.\
**true_value_name**: Stringa. Nome visualizzato da visualizzare nell’editor delle pagine di destinazione quando il valore è nella posizione ON. &quot;ON&quot; se non viene fornito.

Esempio di base:

`<pre data-theme="Confluence"><meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699"></pre>`

`<pre data-theme="Confluence"><meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable"></pre>`

Esempio con tutti gli attributi:

Questo esempio mostra un caso d’uso comune in cui una variabile booleana controlla la visibilità di un elemento css impostando il valore della proprietà di visualizzazione css su &quot;block&quot; o &quot;none&quot; per mostrare/nascondere un elemento per id con CSS. L’editor della pagina di destinazione utilizza il nome visualizzato Mostra/Nascondi invece di OFF/ON.

`<pre data-theme="Confluence"><meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable" default="true" true_value="block" false_value="none" false_value_name="Hide" true_value_name="Show"> <style> #myConditionalDisplayArea { display: ${boolean1}; } </style></pre>`

>[!NOTE]
>
>I token del programma (my.token) possono essere utilizzati anche ovunque nelle pagine di destinazione Guided o Free-form.
