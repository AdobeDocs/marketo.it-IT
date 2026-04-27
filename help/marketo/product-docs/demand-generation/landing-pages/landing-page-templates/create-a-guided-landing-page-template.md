---
unique-page-id: 7515401
description: Learn how to create a guided landing page template in Marketo. Use syntax to define editable regions and variables for the guided editor.
title: Creare un modello di pagina di destinazione in formato guidato
exl-id: 7d097162-d862-4d09-9440-aba1628450c2
feature: Landing Pages
source-git-commit: 4a95c37fe8c09cdbe3cc84e701f0fc50286fc276
workflow-type: tm+mt
source-wordcount: '1127'
ht-degree: 21%

---

# Creare un modello di pagina di destinazione in formato guidato {#create-a-guided-landing-page-template}

Guided landing page templates have a special syntax. Use this syntax to specify what is customizable and where content will end up on each landing page built from your template. Only the regions or variables you specify as editable will be available for customization within the &quot;Guided&quot; landing page editor.

>[!TIP]
>
>Use good naming conventions and your marketing team will fall in love with you.

There are two ways to declare that something on your page should be editable:

* Declare an object as an &quot;element&quot;. The landing page creator will be able to add images, text, or Marketo assets into those specified regions.
* Declare a string as a &quot;variable&quot;. The landing page creator will be able to replace that variable with a string, color, or boolean state from a true/false lever.

## Editable Elements {#editable-elements}

Elements are declared by adding a normal DOM element to the template, then decorating the element with a Marketo-specific class name.

## Testo {#text}

Se definisci un’area come Rich Text, gli utenti potranno modificarne il contenuto [utilizzando l’Editor Rich Text di Marketo](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md).

Required attributes:
**class**: &quot;mktoText&quot;
**id**: stringa ID. Contiene solo lettere, numeri, trattini “-” e trattini bassi “_”. Non sono consentiti spazi. Deve essere univoco.
**mktoName**: stringa. This is the display name that will be shown in the landing page editor. Best practice is to use a descriptive name.

Optional:
The content of an element with class mktoText (if provided) will be used as the default value for the editable region.

Esempio:

`<div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area.</div>`

## Immagine {#image}

You have two options for defining editable Image Elements. You may use either a `<div>`, which specifies a container that the image will be inserted into, or an `<img>` tag.

## Opzione 1: Utilizzare un elemento `<div>` {#option-use-a-div}

Required attributes:

class: &quot;mktoImg&quot;
id: ID string. Contiene solo lettere, numeri, trattini “-” e trattini bassi “_”. Non sono consentiti spazi. Deve essere univoco.
mktoName : String. This is the display name that will be shown in the landing page editor. Si consiglia di utilizzare un nome descrittivo.

Facoltativo:
mktoImgClass: Stringa. Il valore verrà aggiunto all’attributo classe dell’elemento `<img>` all’interno del div.

Esempio:

`<div class="mktoImg" id="exampleImg" mktoName="Example Image"></div>`

## Opzione 2 - Utilizzare un `<img>` {#option-use-a-img}

Attributi richiesti:
class: &quot;mktoImg&quot;
id: stringa ID. Contiene solo lettere, numeri, trattini “-” e trattini bassi “_”. Non sono consentiti spazi. Deve essere univoco.
mktoName : Stringa. Questo è il nome visualizzato che verrà visualizzato nell’editor pagina di destinazione. Si consiglia di utilizzare un nome descrittivo.

Facoltativo:
src: URL stringa. Verrà utilizzato come valore predefinito per l&#39;immagine.

Esempio:

`<img class="mktoImg" id="exampleImg" mktoName="Example Image">`

>[!NOTE]
>
>Quando si utilizza la versione `<img>`, il HTML sottoposto a rendering conterrà un wrapper div generato intorno al tag `<img>`. Verrà impostata sulla classe .&quot;mktoImg.mktoGen&quot; e verrà visualizzata:inline-block.

## Modulo {#form}

Attributi :Required di esempio:
**classe**: &quot;mktoForm&quot;
**id**: stringa ID. Contiene solo lettere, numeri, trattini “-” e trattini bassi “_”. Non sono consentiti spazi. Deve essere univoco.
**mktoName**: stringa. Questo è il nome visualizzato che verrà visualizzato nell’editor pagina di destinazione. Si consiglia di utilizzare un nome descrittivo.

`<div class="mktoForm" id="exampleForm" mktoName="Example Form"></div>`

## Snippet {#snippet}

Attributi richiesti:
**class**: &quot;mktoSnippet&quot;
**id**: stringa ID. Contiene solo lettere, numeri, trattini “-” e trattini bassi “_”. Non sono consentiti spazi. Deve essere univoco.
**mktoName**: stringa. Questo è il nome visualizzato che verrà visualizzato nell’editor pagina di destinazione. Si consiglia di utilizzare un nome descrittivo.

Esempio:

`<div class="mktoSnippet" id="exampleSnippet" mktoName="Example Snippet"></div>`

## Pulsante Condividi {#share-button}

Attributi richiesti:
**classe**: &quot;mktoShareButton&quot;
**id**: stringa ID. Contiene solo lettere, numeri, trattini “-” e trattini bassi “_”. Non sono consentiti spazi. Deve essere univoco.
**mktoName**: stringa. Questo è il nome visualizzato che verrà visualizzato nell’editor pagina di destinazione. Si consiglia di utilizzare un nome descrittivo.

Esempio:

`<div class="mktoShareButton" id="exampleShareButton" mktoName="Example Share Button"></div>`

## Video {#video}

>[!NOTE]
>
>Quando utilizzi l’elemento video in una pagina di destinazione, Marketo supporta solo i video di YouTube. Se utilizzi un altro servizio, ti consigliamo di utilizzare una casella di testo RTF e di incollarla nel codice di incorporamento del video.

Attributi richiesti:
**classe**: &quot;mktoVideo&quot;
**id**: stringa ID. Contiene solo lettere, numeri, trattini “-” e trattini bassi “_”. Non sono consentiti spazi. Deve essere univoco.
**mktoName**: stringa. Questo è il nome visualizzato che verrà visualizzato nell’editor pagina di destinazione. Si consiglia di utilizzare un nome descrittivo.

Esempio:

`<div class="mktoVideo" id="exampleVideo" mktoName="Example Video"></div>`

## Variabili Modificabili {#editable-variables}

Tutti i tipi di variabili vengono utilizzati facendo riferimento al valore del loro attributo id racchiuso all&#39;interno di una sequenza di caratteri ${ }. Possono essere utilizzati in qualsiasi punto del documento, ad eccezione delle dichiarazioni di altre variabili.

Esempio:

`${var1}`

**Dichiarazione:**

Le variabili sono dichiarate come metatag nell&#39;elemento `<head>` del modello. Sono disponibili tre tipi di variabili: String, Color e Boolean.

## Stringa {#string}

Attributi obbligatori:
**classe**: &quot;mktoString&quot;,
**id**: stringa ID. Contiene solo lettere, numeri, trattini “-” e trattini bassi “_”. Non sono consentiti spazi. Deve essere univoco.
**mktoName**: stringa. Questo è il nome visualizzato che verrà visualizzato nell’editor pagina di destinazione. Si consiglia di utilizzare un nome descrittivo.

Facoltativo:
**default**: valore stringa per l&#39;attributo. Vuoto se non specificato.
**allowHtml**: &quot;true&quot; o &quot;false&quot;. Controlla se il valore verrà stampato senza escape di HTML. Se non viene impostato, il valore predefinito è &quot;false&quot;.

Esempio di base:

`<meta class="mktoString" id="var1" mktoName="My Variable">`

Esempio con tutti gli attributi:

`<meta class="mktoString" id="var1" mktoName="My Variable" default="This is my default value" allowHtml="true">`

## Colore {#color}

Attributi obbligatori:
**classe**: &quot;mktoColor&quot;,
**id**: stringa ID. Contiene solo lettere, numeri, trattini “-” e trattini bassi “_”. Non sono consentiti spazi. Deve essere univoco.
**mktoName**: stringa. Questo è il nome visualizzato che verrà visualizzato nell’editor pagina di destinazione. Si consiglia di utilizzare un nome descrittivo.

Facoltativo:
**default**: codice di colore del carattere HEX a 7 cifre. Esempio: &quot;#336699&quot;

Esempio di base:

`<meta class="mktoColor" id="color1" mktoName="My Color Variable">`

Esempio con tutti gli attributi:

`<meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699">`

## Booleano {#boolean}

Attributi obbligatori:
**class** : &quot;mktoBoolean&quot;,
**id**: stringa ID. Contiene solo lettere, numeri, trattini “-” e trattini bassi “_”. Non sono consentiti spazi. Deve essere univoco.
**mktoName**: stringa. Questo è il nome visualizzato che verrà visualizzato nell’editor pagina di destinazione. Si consiglia di utilizzare un nome descrittivo.

Facoltativo:
**default**: stringa booleana. &quot;true&quot; o &quot;false&quot; controlla se il valore inizia in posizione ON o OFF. &quot;false&quot; se non specificato.
**false_value**: stringa. Il valore da inserire per la variabile quando è in posizione OFF. &quot;false&quot; se non specificato.
**true_value**: stringa. Valore da inserire per la variabile quando è in posizione ON. &quot;true&quot; se non specificato.
**false_value_name**: stringa. Il nome visualizzato da visualizzare nell’editor pagina di destinazione quando il valore è in posizione OFF. &quot;OFF&quot; se non specificato.
**true_value_name**: stringa. Il nome visualizzato da visualizzare nell’editor pagina di destinazione quando il valore è nella posizione ON. &quot;ON&quot; se non specificato.

Esempio di base:

`<meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable">`

Esempio con tutti gli attributi:

`<meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699">`

Questo esempio mostra un caso d’uso comune in cui una variabile booleana controlla la visibilità di un elemento css impostando il valore della proprietà di visualizzazione css su &quot;block&quot; o &quot;none&quot; per mostrare/nascondere un elemento per id con gli stili CSS. L’editor della pagina di destinazione utilizza il nome visualizzato Mostra/Nascondi invece di OFF/ON.

`<meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable" default="true" true_value="block" false_value="none" false_value_name="Hide" true_value_name="Show"> <style> #myConditionalDisplayArea { display: ${boolean1}; } </style>`

>[!NOTE]
>
>I token del programma (my.token) possono essere utilizzati anche in qualsiasi punto delle pagine di destinazione guidate o in formato libero.
