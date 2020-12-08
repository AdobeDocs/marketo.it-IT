---
unique-page-id: 7515401
description: Creare un modello di pagina di destinazione guidata - Documenti Marketo - Documentazione prodotto
title: Creare un modello di pagina di destinazione guidato
translation-type: tm+mt
source-git-commit: 975e048271dae6a877ae9ff5d39360b159afcc8a
workflow-type: tm+mt
source-wordcount: '1271'
ht-degree: 0%

---


# Creare un modello di pagina di destinazione guidato {#create-a-guided-landing-page-template}

>[!NOTE]
>
>**Dive profonde:** Stanco di leggere? [Guardate questo video](https://youtu.be/3O7e4GdZKsM) con istruzioni dettagliate.

I modelli delle pagine di destinazione guidati hanno una sintassi particolare. Utilizzate questa sintassi per specificare cosa è personalizzabile e dove termina il contenuto su ciascuna pagina di destinazione creata a partire dal modello. Solo le aree o le variabili specificate come modificabili saranno disponibili per la personalizzazione nell’editor della pagina di destinazione &quot;Guidata&quot;.

>[!TIP]
>
>Utilizza buone convenzioni di denominazione e il tuo team marketing si innamorerà di te.

Esistono due modi per dichiarare che qualcosa sulla pagina deve essere modificabile:

* Dichiarare un oggetto come &quot;elemento&quot;. L’autore della pagina di destinazione potrà aggiungere immagini, testo o risorse Marketo nelle aree specificate.
* Dichiarare una stringa come &quot;variabile&quot;. Il creatore della pagina di destinazione sarà in grado di sostituire tale variabile con una stringa, un colore o uno stato booleano da una leva true/false.

## Elementi modificabili {#editable-elements}

Gli elementi vengono dichiarati aggiungendo al modello un normale elemento DOM, quindi decorando l’elemento con un nome di classe specifico per Marketo.

## Testo {#text}

Se definite un&#39;area come RTF, gli utenti potranno modificarne il contenuto [utilizzando l&#39;Editor](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md)Rich Text di Marketo.

Attributi richiesti:\
**class**: &quot;mktoText&quot;\
**id**: Stringa ID. Contiene solo lettere, numeri, trattino &quot;-&quot; e carattere di sottolineatura &quot;_&quot;. Nessun spazio consentito. Deve essere univoco.\
**mktoName** : Stringa. Questo è il nome visualizzato che verrà visualizzato nell&#39;editor della pagina di destinazione. Come procedura ottimale si consiglia di utilizzare un nome descrittivo.

Facoltativo:\
Il contenuto di un elemento con classe mktoText (se fornito) verrà utilizzato come valore predefinito per l&#39;area modificabile.

Esempio:

`<pre data-theme="Confluence"><div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div></pre>`

### Immagine {#image}

Sono disponibili due opzioni per definire gli elementi immagine modificabili. Potete usare un `<div>`, che specifica un contenitore in cui inserire l’immagine, o un `<img>` tag.

## Opzione 1 - Utilizzate un <div> {#option-use-a-div}

Attributi richiesti:

class: &quot;mktoImg&quot;\
id: Stringa ID. Contiene solo lettere, numeri, trattino &quot;-&quot; e carattere di sottolineatura &quot;_&quot;. Nessun spazio consentito. Deve essere univoco.\
mktoName : Stringa. Questo è il nome visualizzato che verrà visualizzato nell&#39;editor della pagina di destinazione. Come procedura ottimale si consiglia di utilizzare un nome descrittivo.

Facoltativo:\
mktoImgClass: Stringa. Il valore qui verrà aggiunto all&#39;attributo class dell&#39; `<img>` elemento all&#39;interno del div.

Esempio:

`<pre data-theme="Confluence"><div class="mktoImg" id="exampleImg" mktoName="Example Image"></div></pre>`

## Opzione 2 - Utilizzate un `<img>` {#option-use-a-img}

Attributi richiesti:\
class: &quot;mktoImg&quot;\
id: Stringa ID. Contiene solo lettere, numeri, trattino &quot;-&quot; e carattere di sottolineatura &quot;_&quot;. Nessun spazio consentito. Deve essere univoco.\
mktoName : Stringa. Questo è il nome visualizzato che verrà visualizzato nell&#39;editor della pagina di destinazione. Come procedura ottimale si consiglia di utilizzare un nome descrittivo.

Facoltativo:\
src: URL stringa. Questo verrà utilizzato come valore predefinito per l&#39;immagine.

Esempio:

`<pre data-theme="Confluence"><img class="mktoImg" id="exampleImg" mktoName="Example Image"></pre>`

>[!NOTE]
>
>Quando si utilizza la `<img>` versione, l&#39;HTML rappresentato conterrà un wrapper div generato intorno al `<img>` tag . Sarà impostato su class.&quot;mktoImg.mktoGen,&quot; e sarà display:inline-block.

## Modulo {#form}

Esempio:Attributi richiesti:\
**class**: &quot;mktoForm&quot;\
**id**: Stringa ID. Contiene solo lettere, numeri, trattino &quot;-&quot; e carattere di sottolineatura &quot;_&quot;. Nessun spazio consentito. Deve essere univoco.\
**mktoName** : Stringa. Questo è il nome visualizzato che verrà visualizzato nell&#39;editor della pagina di destinazione. Come procedura ottimale si consiglia di utilizzare un nome descrittivo.

`<pre data-theme="Confluence"><div class="mktoForm" id="exampleForm" mktoName="Example Form"></div></pre>`

## Snippet {#snippet}

Attributi richiesti:\
**class**: &quot;mktoSnippet&quot;\
**id**: Stringa ID. Contiene solo lettere, numeri, trattino &quot;-&quot; e carattere di sottolineatura &quot;_&quot;. Nessun spazio consentito. Deve essere univoco.\
**mktoName** : Stringa. Questo è il nome visualizzato che verrà visualizzato nell&#39;editor della pagina di destinazione. Come procedura ottimale si consiglia di utilizzare un nome descrittivo.

Esempio:

`<pre data-theme="Confluence"><div class="mktoSnippet" id="exampleSnippet" mktoName="Example Snippet"></div></pre>`

## Pulsante Condividi {#share-button}

Attributi richiesti:\
**class**: &quot;mktoShareButton&quot;\
**id**: Stringa ID. Contiene solo lettere, numeri, trattino &quot;-&quot; e carattere di sottolineatura &quot;_&quot;. Nessun spazio consentito. Deve essere univoco.\
**mktoName** : Stringa. Questo è il nome visualizzato che verrà visualizzato nell&#39;editor della pagina di destinazione. Come procedura ottimale si consiglia di utilizzare un nome descrittivo.

Esempio:

`<pre data-theme="Confluence"><div class="mktoShareButton" id="exampleShareButton" mktoName="Example Share Button"></div></pre>`

## Video {#video}

>[!NOTE]
>
>Quando si utilizza l’elemento video in una pagina di destinazione, Marketo supporta solo i video di YouTube. Se utilizzate un altro servizio, è consigliabile utilizzare una casella di testo RTF e incollare nel codice da incorporare del video.

Attributi richiesti:
**class**: &quot;mktoVideo&quot;**id**: Stringa ID. Contiene solo lettere, numeri, trattino &quot;-&quot; e carattere di sottolineatura &quot;_&quot;. Nessun spazio consentito. Deve essere univoco.
**mktoName** : Stringa. Questo è il nome visualizzato che verrà visualizzato nell&#39;editor della pagina di destinazione. Come procedura ottimale si consiglia di utilizzare un nome descrittivo.

Esempio:

`<pre data-theme="Confluence"><div class="mktoVideo" id="exampleVideo" mktoName="Example Video"></div></pre>`

## Sondaggio {#poll}

Attributi richiesti:\
**class**: &quot;mktoPoll&quot;\
**id**: Stringa ID. Contiene solo lettere, numeri, trattino &quot;-&quot; e carattere di sottolineatura &quot;_&quot;. Nessun spazio consentito. Deve essere univoco.\
**mktoName** : Stringa. Questo è il nome visualizzato che verrà visualizzato nell&#39;editor della pagina di destinazione. Come procedura ottimale si consiglia di utilizzare un nome descrittivo.

Esempio:

`<pre data-theme="Confluence"><div class="mktoPoll" id="examplePoll" mktoName="Example Poll"></div></pre>`

## Riferimento {#referral}

Attributi richiesti:\
**class**: &quot;mktoReferral&quot;\
**id**: Stringa ID. Contiene solo lettere, numeri, trattino &quot;-&quot; e carattere di sottolineatura &quot;_&quot;. Nessun spazio consentito. Deve essere univoco.\
**mktoName** : Stringa. Questo è il nome visualizzato che verrà visualizzato nell&#39;editor della pagina di destinazione. Come procedura ottimale si consiglia di utilizzare un nome descrittivo.

Esempio:

`<pre data-theme="Confluence"><div class="mktoReferral" id="exampleReferral" mktoName="Example Referral"></div></pre>`

## Sweepstakes {#sweepstakes}

Attributi richiesti:\
**class**: &quot;mktoSweepstakes&quot;\
**id**: Stringa ID. Contiene solo lettere, numeri, trattino &quot;-&quot; e carattere di sottolineatura &quot;_&quot;. Nessun spazio consentito. Deve essere univoco.\
**mktoName** : Stringa. Questo è il nome visualizzato che verrà visualizzato nell&#39;editor della pagina di destinazione. Come procedura ottimale si consiglia di utilizzare un nome descrittivo.

Esempio:

`<pre data-theme="Confluence"><div class="mktoSweepstakes" id="exampleSweepstakes" mktoName="Example Sweepstakes"></div></pre>`

## Variabili modificabili {#editable-variables}

Tutti i tipi di variabili vengono utilizzati facendo riferimento al valore dell&#39;attributo id racchiuso all&#39;interno di una sequenza di caratteri ${ }. Possono essere utilizzati in qualsiasi punto del documento, ad eccezione dell&#39;interno di altre dichiarazioni di variabili.

Esempio:

`<pre data-theme="Confluence">${var1}</pre>`

**Dichiarazione:**

Le variabili sono dichiarate come tag meta all&#39;interno dell&#39; `<head>` elemento del modello. Sono disponibili tre tipi di variabili: Stringa, Colore e Booleano.

## Stringa {#string}

Attributi richiesti:\
**class** : &quot;mktoString&quot;,\
**id**: Stringa ID. Contiene solo lettere, numeri, trattino &quot;-&quot; e carattere di sottolineatura &quot;_&quot;. Nessun spazio consentito. Deve essere univoco.\
**mktoName** : Stringa. Questo è il nome visualizzato che verrà visualizzato nell&#39;editor della pagina di destinazione. Come procedura ottimale si consiglia di utilizzare un nome descrittivo.

Facoltativo:\
**predefinito**: Valore stringa per l&#39;attributo. Vuoto se non è stato fornito alcun valore.\
**allowHtml**: &quot;true&quot; o &quot;false&quot;. Controlla se il valore verrà stampato senza che sia stato eseguito l&#39;escape HTML. Il valore predefinito è &quot;false&quot; se non viene impostato.

Esempio di base:

`<pre data-theme="Confluence"><meta class="mktoString" id="var1" mktoName="My Variable"></pre>`

Esempio con tutti gli attributi:

`<pre data-theme="Confluence"><meta class="mktoString" id="var1" mktoName="My Variable" default="This is my default value" allowHtml="true"></pre>`

## Colore {#color}

Attributi richiesti:\
**class** : &quot;mktoColor&quot;,\
**id**: Stringa ID. Contiene solo lettere, numeri, trattino &quot;-&quot; e carattere di sottolineatura &quot;_&quot;. Nessun spazio consentito. Deve essere univoco.\
**mktoName** : Stringa. Questo è il nome visualizzato che verrà visualizzato nell&#39;editor della pagina di destinazione. Come procedura ottimale si consiglia di utilizzare un nome descrittivo.

Facoltativo:\
**predefinito**: Un codice colore HEX a 7 cifre. Esempio: &quot;#336699&quot;

Esempio di base:

`<pre data-theme="Confluence"><meta class="mktoColor" id="color1" mktoName="My Color Variable"></pre>`

Esempio con tutti gli attributi:

`<pre data-theme="Confluence"><meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699"></pre>`

## Booleano {#boolean}

Attributi richiesti:\
**class** : &quot;mktoBoolean&quot;,\
**id**: Stringa ID. Contiene solo lettere, numeri, trattino &quot;-&quot; e carattere di sottolineatura &quot;_&quot;. Nessun spazio consentito. Deve essere univoco.\
**mktoName** : Stringa. Questo è il nome visualizzato che verrà visualizzato nell&#39;editor della pagina di destinazione. Come procedura ottimale si consiglia di utilizzare un nome descrittivo.

Facoltativo:\
**predefinito**: Stringa booleana. &quot;true&quot; o &quot;false&quot; controlla se il valore inizia nella posizione ON o OFF. &quot;false&quot; se non viene fornito.\
**false_value**: Stringa. Il valore da inserire per la variabile quando si trova nella posizione OFF. &quot;false&quot; se non viene fornito.\
**true_value**: Stringa. Il valore da inserire per la variabile quando si trova nella posizione ON. &quot;true&quot; se non viene fornito.\
**false_value_name**: Stringa. Nome visualizzato da visualizzare nell&#39;editor della pagina di destinazione quando il valore è nella posizione OFF. &quot;OFF&quot; se non fornito.\
**true_value_name**: Stringa. Nome visualizzato da visualizzare nell&#39;editor della pagina di destinazione quando il valore si trova nella posizione Attivato. &quot;ON&quot; se non fornito.

Esempio di base:

`<pre data-theme="Confluence"><meta class="mktoColor" id="color" mktoName="My Color Variable" default="#336699"></pre>`

`<pre data-theme="Confluence"><meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable"></pre>`

Esempio con tutti gli attributi:

Questo esempio mostra un caso d’uso comune in cui una variabile booleana controlla la visibilità di un elemento css impostando il valore della proprietà di visualizzazione css su &quot;block&quot; o &quot;none&quot; per mostrare/nascondere un elemento per ID con CSS. L&#39;editor della pagina di destinazione utilizza il nome visualizzato Mostra/Nascondi invece di OFF/ON.

`<pre data-theme="Confluence"><meta class="mktoBoolean" id="boolean1" mktoName="My Boolean Variable" default="true" true_value="block" false_value="none" false_value_name="Hide" true_value_name="Show"> <style> #myConditionalDisplayArea { display: ${boolean1}; } </style></pre>`

>[!NOTE]
>
>I token del programma (my.token) possono essere utilizzati anche in qualsiasi punto delle pagine di destinazione Guided o Free-form.
