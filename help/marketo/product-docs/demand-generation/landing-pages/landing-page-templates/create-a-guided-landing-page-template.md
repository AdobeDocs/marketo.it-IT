---
unique-page-id: 7515401
description: Creare un modello di pagina di destinazione guidata - Documentazione di Marketo - Documentazione del prodotto
title: Creare un modello di pagina di destinazione guidata
exl-id: 7d097162-d862-4d09-9440-aba1628450c2
feature: Landing Pages
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1254'
ht-degree: 1%

---

# Creare un modello di pagina di destinazione guidata {#create-a-guided-landing-page-template}

I modelli di pagina di destinazione guidata hanno una sintassi speciale. Utilizza questa sintassi per specificare cosa è personalizzabile e dove il contenuto finirà su ogni pagina di destinazione creata dal modello. Solo le aree geografiche o le variabili specificate come modificabili saranno disponibili per la personalizzazione nell’editor di pagine di destinazione &quot;Guidate&quot;.

>[!TIP]
>
>Utilizza le buone convenzioni di denominazione e il tuo team di marketing si innamorerà di te.

Esistono due modi per dichiarare che un elemento nella pagina deve essere modificabile:

* Dichiarare un oggetto come &quot;elemento&quot;. Il creatore della pagina di destinazione sarà in grado di aggiungere immagini, testo o risorse Marketo nelle aree specificate.
* Dichiara una stringa come &quot;variabile&quot;. Il creatore della pagina di destinazione sarà in grado di sostituire tale variabile con una stringa, un colore o uno stato booleano da una leva true/false.

## Elementi modificabili {#editable-elements}

Gli elementi vengono dichiarati aggiungendo un normale elemento DOM al modello, quindi decorando l’elemento con un nome di classe specifico per Marketo.

## Testo {#text}

Se si definisce un&#39;area come Testo formattato, gli utenti potranno modificarne il contenuto [utilizzo dell’editor Rich Text di Marketo](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md).

Attributi richiesti:\
**classe**: &quot;mktoText&quot;\
**id**: stringa ID. Contiene solo lettere, numeri, trattini &quot;-&quot; e trattini bassi &quot;_&quot;. Non sono consentiti spazi. Deve essere univoco.\
**mktoName** : stringa. Questo è il nome visualizzato che verrà visualizzato nell’editor pagina di destinazione. Si consiglia di utilizzare un nome descrittivo.

Facoltativo:\
Il contenuto di un elemento con la classe mktoText (se fornita) verrà utilizzato come valore predefinito per l’area modificabile.

Esempio:

`<div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area.</div>`

## Immagine {#image}

Sono disponibili due opzioni per definire gli elementi immagine modificabili. È possibile utilizzare una delle seguenti opzioni `<div>`, che specifica un contenitore in cui verrà inserita l&#39;immagine o un `<img>` tag.

## Opzione 1 - Utilizzare un `<div>` {#option-use-a-div}

Attributi richiesti:

class: &quot;mktoImg&quot;\
id: stringa ID. Contiene solo lettere, numeri, trattini &quot;-&quot; e trattini bassi &quot;_&quot;. Non sono consentiti spazi. Deve essere univoco.\
mktoName : Stringa. Questo è il nome visualizzato che verrà visualizzato nell’editor pagina di destinazione. Si consiglia di utilizzare un nome descrittivo.

Facoltativo:\
mktoImgClass: Stringa. Il valore qui verrà aggiunto all’attributo class del `<img>` all&#39;interno del div.

Esempio:

`<div class="mktoImg" id="exampleImg" mktoName="Example Image"></div>`

## Opzione 2 - Utilizzare un `<img>` {#option-use-a-img}

Attributi richiesti:\
class: &quot;mktoImg&quot;\
id: stringa ID. Contiene solo lettere, numeri, trattini &quot;-&quot; e trattini bassi &quot;_&quot;. Non sono consentiti spazi. Deve essere univoco.\
mktoName : Stringa. Questo è il nome visualizzato che verrà visualizzato nell’editor pagina di destinazione. Si consiglia di utilizzare un nome descrittivo.

Facoltativo:\
src: URL stringa. Verrà utilizzato come valore predefinito per l&#39;immagine.

Esempio:

`<img class="mktoImg" id="exampleImg" mktoName="Example Image">`

>[!NOTE]
>
>Quando si utilizza `<img>` versione, il HTML sottoposto a rendering conterrà un wrapper div generato intorno al `<img>` tag. Sarà impostato su class .&quot;mktoImg.mktoGen,&quot; e sarà visualizzato:inline-block.

## Modulo {#form}

Esempio:Attributi obbligatori:\
**classe**: &quot;mktoForm&quot;\
**id**: stringa ID. Contiene solo lettere, numeri, trattini &quot;-&quot; e trattini bassi &quot;_&quot;. Non sono consentiti spazi. Deve essere univoco.\
**mktoName** : stringa. Questo è il nome visualizzato che verrà visualizzato nell’editor pagina di destinazione. Si consiglia di utilizzare un nome descrittivo.

`<div class="mktoForm" id="exampleForm" mktoName="Example Form"></div>`

## Frammento {#snippet}

Attributi richiesti:\
**classe**: &quot;mktoSnippet&quot;\
**id**: stringa ID. Contiene solo lettere, numeri, trattini &quot;-&quot; e trattini bassi &quot;_&quot;. Non sono consentiti spazi. Deve essere univoco.\
**mktoName** : stringa. Questo è il nome visualizzato che verrà visualizzato nell’editor pagina di destinazione. Si consiglia di utilizzare un nome descrittivo.

Esempio:

`<div class="mktoSnippet" id="exampleSnippet" mktoName="Example Snippet"></div>`

## Pulsante Condividi {#share-button}

Attributi richiesti:\
**classe**: &quot;mktoShareButton&quot;\
**id**: stringa ID. Contiene solo lettere, numeri, trattini &quot;-&quot; e trattini bassi &quot;_&quot;. Non sono consentiti spazi. Deve essere univoco.\
**mktoName** : stringa. Questo è il nome visualizzato che verrà visualizzato nell’editor pagina di destinazione. Si consiglia di utilizzare un nome descrittivo.

Esempio:

`<div class="mktoShareButton" id="exampleShareButton" mktoName="Example Share Button"></div>`

## Video {#video}

>[!NOTE]
>
>Quando utilizzi l’elemento video in una pagina di destinazione, Marketo supporta solo i video di YouTube. Se utilizzi un altro servizio, ti consigliamo di utilizzare una casella di testo RTF e di incollarla nel codice di incorporamento del video.

Attributi richiesti:
**classe**: &quot;mktoVideo&quot;
**id**: stringa ID. Contiene solo lettere, numeri, trattini &quot;-&quot; e trattini bassi &quot;_&quot;. Non sono consentiti spazi. Deve essere univoco.
**mktoName** : stringa. Questo è il nome visualizzato che verrà visualizzato nell’editor pagina di destinazione. Si consiglia di utilizzare un nome descrittivo.

Esempio:

`<div class="mktoVideo" id="exampleVideo" mktoName="Example Video"></div>`

## Sondaggio {#poll}

Attributi richiesti:\
**classe**: &quot;mktoPoll&quot;\
**id**: stringa ID. Contiene solo lettere, numeri, trattini &quot;-&quot; e trattini bassi &quot;_&quot;. Non sono consentiti spazi. Deve essere univoco.\
**mktoName** : stringa. Questo è il nome visualizzato che verrà visualizzato nell’editor pagina di destinazione. Si consiglia di utilizzare un nome descrittivo.

Esempio:

`<div class="mktoPoll" id="examplePoll" mktoName="Example Poll"></div>`

## Referral {#referral}

Attributi richiesti:\
**classe**: &quot;mktoReferral&quot;\
**id**: stringa ID. Contiene solo lettere, numeri, trattini &quot;-&quot; e trattini bassi &quot;_&quot;. Non sono consentiti spazi. Deve essere univoco.\
**mktoName** : stringa. Questo è il nome visualizzato che verrà visualizzato nell’editor pagina di destinazione. Si consiglia di utilizzare un nome descrittivo.

Esempio:

`<div class="mktoReferral" id="exampleReferral" mktoName="Example Referral"></div>`

## Lotterie {#sweepstakes}

Attributi richiesti:\
**classe**: &quot;mktoSweepstakes&quot;\
**id**: stringa ID. Contiene solo lettere, numeri, trattini &quot;-&quot; e trattini bassi &quot;_&quot;. Non sono consentiti spazi. Deve essere univoco.\
**mktoName** : stringa. Questo è il nome visualizzato che verrà visualizzato nell’editor pagina di destinazione. Si consiglia di utilizzare un nome descrittivo.

Esempio:

`<div class="mktoSweepstakes" id="exampleSweepstakes" mktoName="Example Sweepstakes"></div>`

## Variabili Modificabili {#editable-variables}

Tutti i tipi di variabili vengono utilizzati facendo riferimento al valore del loro attributo id racchiuso all&#39;interno di una sequenza di caratteri ${ }. Possono essere utilizzati in qualsiasi punto del documento, ad eccezione delle dichiarazioni di altre variabili.

Esempio:

`${var1}`

**Dichiarazione:**

Le variabili vengono dichiarate come metatag all’interno del `<head>` del modello. Sono disponibili tre tipi di variabili: String, Color e Boolean.

## Stringa {#string}

Attributi obbligatori:\
**classe** : &quot;mktoString&quot;,\
**id**: stringa ID. Contiene solo lettere, numeri, trattini &quot;-&quot; e trattini bassi &quot;_&quot;. Non sono consentiti spazi. Deve essere univoco.\
**mktoName** : stringa. Questo è il nome visualizzato che verrà visualizzato nell’editor pagina di destinazione. Si consiglia di utilizzare un nome descrittivo.

Facoltativo:\
**predefinito**: valore stringa per l’attributo. Vuoto se non specificato.\
**allowHtml**: &quot;true&quot; o &quot;false&quot;. Controlla se il valore verrà stampato senza escape HTML. Se non viene impostato, il valore predefinito è &quot;false&quot;.

Esempio di base:

`<meta class="mktoString" id="var1" mktoName="My Variable">`

Esempio con tutti gli attributi:

`<meta class="mktoString" id="var1" mktoName="My Variable" default="This is my default value" allowHtml="true">`

## Colore {#color}

Attributi obbligatori:\
**classe** : &quot;mktoColor&quot;,\
**id**: stringa ID. Contiene solo lettere, numeri, trattini &quot;-&quot; e trattini bassi &quot;_&quot;. Non sono consentiti spazi. Deve essere univoco.\
**mktoName** : stringa. Questo è il nome visualizzato che verrà visualizzato nell’editor pagina di destinazione. Si consiglia di utilizzare un nome descrittivo.

Facoltativo:\
**predefinito**: codice colore del carattere HEX a 7 cifre. Esempio: &quot;#336699&quot;

Esempio di base:

`<meta class="mktoColor" id="color1" mktoName="My Color Variable">`

Esempio con tutti gli attributi:

`<meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699">`

## Booleano {#boolean}

Attributi obbligatori:\
**classe** : &quot;mktoBoolean&quot;,\
**id**: stringa ID. Contiene solo lettere, numeri, trattini &quot;-&quot; e trattini bassi &quot;_&quot;. Non sono consentiti spazi. Deve essere univoco.\
**mktoName** : stringa. Questo è il nome visualizzato che verrà visualizzato nell’editor pagina di destinazione. Si consiglia di utilizzare un nome descrittivo.

Facoltativo:\
**predefinito**: stringa booleana. &quot;true&quot; o &quot;false&quot; controlla se il valore inizia in posizione ON o OFF. &quot;false&quot; se non specificato.\
**false_value**: stringa. Il valore da inserire per la variabile quando è in posizione OFF. &quot;false&quot; se non specificato.\
**true_value**: stringa. Valore da inserire per la variabile quando è in posizione ON. &quot;true&quot; se non specificato.\
**false_value_name**: stringa. Il nome visualizzato da visualizzare nell’editor pagina di destinazione quando il valore è in posizione OFF. &quot;OFF&quot; se non specificato.\
**true_value_name**: stringa. Il nome visualizzato da visualizzare nell’editor pagina di destinazione quando il valore è nella posizione ON. &quot;ON&quot; se non specificato.

Esempio di base:

`<meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699">`

`<meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable">`

Esempio con tutti gli attributi:

Questo esempio mostra un caso d’uso comune in cui una variabile booleana controlla la visibilità di un elemento css impostando il valore della proprietà di visualizzazione css su &quot;block&quot; o &quot;none&quot; per mostrare/nascondere un elemento per id con gli stili CSS. L’editor della pagina di destinazione utilizza il nome visualizzato Mostra/Nascondi invece di OFF/ON.

`<meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable" default="true" true_value="block" false_value="none" false_value_name="Hide" true_value_name="Show"> <style> #myConditionalDisplayArea { display: ${boolean1}; } </style>`

>[!NOTE]
>
>I token del programma (my.token) possono essere utilizzati anche in qualsiasi punto delle pagine di destinazione guidate o in formato libero.
