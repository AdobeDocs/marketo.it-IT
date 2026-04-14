---
unique-page-id: 11371040
description: Scopri la sintassi del modello e-mail in Email Editor 2.0. Utilizza la sintassi corretta per i moduli e le sezioni modificabili nei modelli.
title: Sintassi del modello e-mail
exl-id: 84d6c0a8-1108-4b7e-8b4f-ac0682c6bdbb
feature: Email Editor
source-git-commit: 95da11838132f31a2728ca18dca39e781c7c3f44
workflow-type: tm+mt
source-wordcount: '2462'
ht-degree: 97%

---

# Sintassi del modello e-mail {#email-template-syntax}

Nella nuova esperienza E-mail 2.0 di Marketo, i modelli e-mail sono composti da qualsiasi combinazione di elementi, variabili, moduli o contenitori. Ciascuno viene definito aggiungendo all’HTML la sintassi specifica di Marketo. I precedenti modelli di e-mail (v1.0) sono supportati nell’editor e-mail 2.0; tuttavia, non includeranno tutte le funzioni del nuovo editor.

La sintassi delle e-mail di Marketo funziona solo nei modelli e nelle singole e-mail; **non** funziona se incorporata in snippet o token Rich Text.

>[!NOTE]
>
>L’assistenza Marketo non può fornire assistenza su CSS o HTML. Se non sei pratico del linguaggio CSS o HTML, rivolgiti al tuo sviluppatore.

>[!CAUTION]
>
>I valori delle classi contenenti sintassi Marketo (ad esempio mktoModule, mktoContainer, mktoText) sono soggetti a distinzione tra maiuscole e minuscole. I nomi degli attributi personalizzati (ad esempio mktoimgwidth, mktoname) non lo sono.

## Elementi {#elements}

Gli elementi sono aree di contenuto che definisci come modificabili nel modello e-mail. L’esperienza di modifica di un elemento dipende dal tipo di elemento e consente di lavorare con facilità sui contenuti. In un modello e-mail è possibile includere i seguenti elementi:

* Rich Text
* Immagini
* Snippet
* Video

## Rich Text {#rich-text}

Se definisci un’area come Rich Text, gli utenti potranno modificarne il contenuto [utilizzando l’Editor Rich Text di Marketo](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md). Esistono due modi per definire un elemento Rich Text all’interno di un modello e-mail: mktEditable e mktoText. Ricorda che un elemento Rich Text può sempre essere convertito in uno snippet dall’interno dell’editor e-mail.

### Opzione 1: mktEditable {#option-mkteditable}

Poiché l’editor e-mail 2.0 è compatibile con le versioni precedenti, alcuni modelli e-mail precedenti possono specificare elementi Rich Text aggiungendo class=&quot;mktEditable&quot; a qualsiasi elemento HTML. Questo è ancora supportato e l’ID dell’elemento funge da nome visualizzato all’interno dell’editor e-mail.

Attributi richiesti

* **class**: &quot;mktEditable&quot;.
* **id**: stringa ID. Contiene solo lettere, numeri, trattini “-” e trattini bassi “_”. Non sono consentiti spazi. Deve essere univoco.

Attributi facoltativi

* **mktoName**: stringa. Questo è il nome che verrà visualizzato nell’editor e-mail 2.0. Si consiglia di utilizzare un nome descrittivo.

Valore predefinito

Il contenuto all’interno dell’elemento HTML (se fornito) con class=&quot;mktEditable&quot; verrà utilizzato come valore predefinito per l’elemento Rich Text.

Esempio:

`<div class="mktEditable" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div>`

### Opzione 2: mktoText {#option-mktotext}

Si consiglia di specificare gli elementi Rich Text utilizzando la sintassi class=&quot;mktoText&quot;. In questo modo sarà sempre presente un nome visualizzato corretto.

Attributi richiesti

* **class**: &quot;mktoText&quot;
* **id**: stringa ID. Contiene solo lettere, numeri, trattini “-” e trattini bassi “_”. Non sono consentiti spazi. Deve essere univoco.
* **mktoName**: stringa. Questo è il nome che verrà visualizzato nell’editor e-mail 2.0. Si consiglia di utilizzare un nome descrittivo.

Valore predefinito

Il contenuto all’interno dell’elemento HTML (se fornito) con class=&quot;mktoText&quot; verrà utilizzato come valore predefinito per l’elemento Rich Text.

Esempio:

`<div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div>`

## Immagini {#images}

Sono disponibili due opzioni per definire gli elementi immagine modificabili. È possibile utilizzare un `<div>`, che specifica un contenitore in cui verrà inserito l’elemento `<img>`, o un tag `<img>`. Se vuoi che l’utente finale possa semplicemente selezionare un’immagine che ne restituirà l’URL (invece del DOM), consulta la sezione “Variabile immagine”, più avanti. Le due opzioni seguenti consentono di inserire un elemento HTML `<img>`.

### Opzione 1: Utilizzare un elemento `<div>` {#option-use-a-div}

Attributi richiesti

* **class:** &quot;mktoImg&quot;.
* **id:** stringa ID. Contiene solo lettere, numeri, trattini “-” e trattini bassi “_”. Non sono consentiti spazi. Deve essere univoco.
* **mktoName:** stringa. Questo è il nome che verrà visualizzato nell’editor e-mail 2.0. Si consiglia di utilizzare un nome descrittivo.

Attributi facoltativi

* **mktoImgClass:** stringa. Il valore verrà aggiunto all’attributo classe dell’elemento `<img>` all’interno del div.
* **mktoImgSrc:** da utilizzare come valore predefinito per l’immagine inserita in questo div. Se viene omesso, viene utilizzato un segnaposto.
* **mktoImgLink:** indica che `<img>` deve essere racchiuso in un tag `<a>` con questo URL di destinazione. L’utente può modificarlo nell’Editor e-mail.
* **mktoImgLinkTarget:** indica che il tag `<a>` dell’attributo mktoImgLink deve utilizzare questa destinazione. Non produce alcun effetto se non si utilizza anche mktoImgLink.
* **mktoImgWidth:** utilizzato come larghezza dell’elemento `<img>` allegato.
* **mktoImgHeight:** utilizzato come altezza dell’elemento `<img>` allegato.
* **mktoLockImgSize:** utilizzato per sbloccare le proprietà height e width dell’elemento `<img>` in modo che l’utente finale possa modificarle (se omesso, il valore predefinito è vero).
* **mktoLockImgStyle:** utilizzato per bloccare la proprietà di stile dell’elemento `<img>` (il valore predefinito è falso).

Valore predefinito (facoltativo)

**`<img>`**: da utilizzare come elemento `<img>` in cui verrà inserita l’immagine. Utile se desideri aggiungere all’immagine uno stile in linea. Ricordati di racchiuderlo tra tag `<a> </a>`, in modo che se l’utente aggiunge un collegamento, lo stile non verrà rimosso.

Esempio:

`<div class="mktoImg" id="exampleImg" mktoName="Example Image" mktoImgLink="https://www.adobe.com"> <a><img style="border:10px solid red;"></a> </div>`

### Opzione 2: Utilizzare un elemento \&lt;img\> {#option-use-an-img}

>[!NOTE]
>
>Questa opzione non consente agli utenti finali di aggiungere un collegamento alla propria immagine. Se il modello dovrà consentire l’aggiunta di un collegamento, utilizza l’opzione 1.

Attributi richiesti

* **class:** &quot;mktoImg&quot;.
* **id:** stringa ID. Contiene solo lettere, numeri, trattini “-” e trattini bassi “_”. Non sono consentiti spazi. Deve essere univoco.
* **mktoName:** stringa. Questo è il nome che verrà visualizzato nell’editor e-mail 2.0. Si consiglia di utilizzare un nome descrittivo.  Valore predefinito (facoltativo)
* **src:** da utilizzare come valore predefinito per l’immagine. Se viene omesso, viene utilizzato un segnaposto.
* **mktoLockImgSize:** utilizzato per sbloccare le proprietà height e width dell’elemento `<img>` in modo che l’utente finale possa modificarle (se omesso, il valore predefinito è vero).
* **mktoLockImgStyle:** utilizzato per bloccare la proprietà di stile dell’elemento `<img>` (il valore predefinito è falso).

Esempio:
`<img class="mktoImg" id="exampleImg" mktoName="Example Image">`

## Snippet {#snippets}

Se si definisce un&#39;area come Snippet, gli utenti finali potranno scegliere quale [Snippet](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-snippet-to-an-email.md) approvato desiderano inserire in questa area. Sebbene gli elementi Rich Text possano essere convertiti in Snippet all’interno dell’editor e-mail, se definisci specificatamente un’area come Snippet, questa non può essere convertita in Rich Text. Puoi specificare un’area Snippet utilizzando un `<div>` con class=“mktoSnippet”

Attributi richiesti

* **id:** ID stringa. Contiene solo lettere, numeri, trattini “-” e trattini bassi “_”. Non sono consentiti spazi. Deve essere univoco.
* **mktoName:** stringa. Questo è il nome che verrà visualizzato nell’editor e-mail 2.0. Si consiglia di utilizzare un nome descrittivo.

Valore predefinito (facoltativo)

**mktoDefaultSnippetId**: l’ID numerico dello Snippet di Marketo che deve essere visualizzato per impostazione predefinita (funzionerà solo se esiste uno Snippet con tale ID esiste e se questo risulta approvato in quell’area di lavoro).

Esempio:

`<div class="mktoSnippet" id="unsubscribeFooter" mktoName="Unsubscribe Footer" mktoDefaultSnippetId="12"></div>`

## Video {#video}

Se definisci un’area come video, gli utenti finali potranno inserire un URL YouTube o Vimeo che verrà visualizzato all’interno dell’e-mail come immagine miniatura (con il pulsante “Riproduci”). Puoi specificare un’area video utilizzando un `<div>` con class=“mktoVideo”

Attributi richiesti

* **id:** ID stringa. Contiene solo lettere, numeri, trattini “-” e trattini bassi “_”. Non sono consentiti spazi. Deve essere univoco.
* **mktoName:** stringa. Questo è il nome che verrà visualizzato nell’editor e-mail 2.0. Si consiglia di utilizzare un nome descrittivo.

Attributi facoltativi

* **mktoImgClass:** stringa. Il valore verrà aggiunto all’attributo classe della miniatura video `<img>` all’interno del div.

Esempio:

`<div class="mktoVideo" id="productVideo" mktoName="Product Announcement Video"></div>`

## Variabili {#variables}

Le variabili sono simili ai token. Prima le definisci all’interno della sezione `<head>` del modello di e-mail utilizzando i tag `<meta>`, quindi puoi utilizzarle nel modello tutte le volte che vuoi. Poiché sono definite nel modello, l’utente finale potrà modificarne i valori in base alle proprie regole. Tieni presente che puoi definire una variabile come locale o globale nel rispettivo ambito. Se utilizzi una variabile all’interno di un “Modulo” (vedi di seguito) e un utente finale lo duplica, le variabili locali avranno valori indipendenti, mentre quelle globali saranno applicabili a entrambi i moduli.

## Stringa {#string}

Se specifichi una variabile come Stringa, l’utente finale potrà inserire il testo all’interno di una casella di testo nell’editor e-mail. Puoi specificare una variabile stringa utilizzando `<meta>` con class=“mktoString”

Attributi richiesti

* **id:** il modo in cui fai riferimento alla variabile all’interno del modello e-mail.
* **mktoName:** stringa. Questo è il nome che verrà visualizzato nell’editor e-mail 2.0. Si consiglia di utilizzare un nome descrittivo.

Attributi facoltativi

* **allowHTML:** booleano. Controlla se il valore della variabile è sottoposto a escaping HTML. Se omesso, il valore predefinito è Falso.
* **default**: il valore predefinito per la stringa. Se omesso, è vuoto.
* **mktoModuleScope**: booleano. Controlla se la variabile è locale (vero) o globale (falso) quando viene utilizzata in un modulo. Se omesso, il valore predefinito è Falso.

Esempio di dichiarazione:

`<meta class="mktoString" id="textHeader" mktoName="Text Header" default="Edit Me">`

Esempio di utilizzo:

`${textHeader}`

## Elenco {#list}

Se specifichi una variabile come Elenco, l’utente finale potrà scegliere da un set di valori che hai definito nell’editor e-mail. Puoi specificare una variabile elenco utilizzando `<meta>` con class=“mktoList”

Attributi richiesti

* **id**: il modo in cui fai riferimento alla variabile all’interno del modello e-mail.
* **mktoName:** stringa. Questo è il nome che verrà visualizzato nell’editor e-mail 2.0. Si consiglia di utilizzare un nome descrittivo.
* **valori:** elenco di valori separato da virgole. Deve disporre di almeno una stringa.

Attributi facoltativi

* **default:** il valore predefinito del menu a discesa di selezione. Se omesso, viene utilizzato il primo valore dell’attributo “values”.
* **mktoModuleScope**: booleano. Controlla se la variabile è locale (vero) o globale (falso) quando viene utilizzata in un modulo. Se omesso, il valore predefinito è Falso.

Esempio di dichiarazione:

`<meta class="mktoList" id="textFontFamily" mktoName="Main Text Font Family" values="Arial,Verdana,Times New Roman">`

Esempio di utilizzo:

`${textFontFamily}`

## Numero {#number}

Se specifichi una variabile come Numero, l’utente finale potrà inserire un numero nell’editor e-mail. Puoi specificare una variabile Numero utilizzando `<meta>` con class=“mktoNumber”

Attributi richiesti

* **id**: il modo in cui fai riferimento alla variabile all’interno del modello e-mail.
* **mktoName**: stringa. Questo è il nome che verrà visualizzato nell’editor e-mail 2.0. Si consiglia di utilizzare un nome descrittivo.
* **default:** il valore numerico predefinito per la variabile.

Attributi facoltativi

* **min:** il valore minimo accettato.
* **max:** il valore massimo accettato.
* **units:** unità da aggiungere al valore numerico (ad es. px, pt, em, ecc.) quando viene visualizzato nell’editor e-mail e nel codice risultante.
* **passaggio:** di quante unità la variabile Numero deve aumentare/diminuire di (0,1, 1, 10, ecc.). Se omesso, il valore predefinito è 1.
* **mktoModuleScope**: booleano. Controlla se la variabile è locale (vero) o globale (falso) quando viene utilizzata in un modulo. Se omesso, il valore predefinito è Falso.

Esempio di dichiarazione:

`<meta class="mktoNumber" id="textFontSize" mktoName="Main Text Font Size" default="12" min="8" max="18" units="px" step="1">`

Esempio di utilizzo:

`${textFontSize}`

## Colore {#color}

Se specifichi una variabile come Colore, l’utente finale potrà inserire un valore esadecimale dei colori o scegliere un colore dal rispettivo selettore all’interno dell’editor e-mail. Puoi specificare una variabile Colore utilizzando `<meta>` con class=“mktoColor”

Attributi richiesti

* **id**: il modo in cui fai riferimento alla variabile all’interno del modello e-mail.
* **mktoName**: stringa. Questo è il nome che verrà visualizzato nell’editor e-mail 2.0. Si consiglia di utilizzare un nome descrittivo.

Attributi facoltativi

* **default:** il valore predefinito per il colore. Codice colore esadecimale a 6 cifre. Esempio: #ffffff.
* **mktoModuleScope**: booleano. Controlla se la variabile è locale (vero) o globale (falso) quando viene utilizzata in un modulo. Se omesso, il valore predefinito è Falso.

Esempio di dichiarazione:

`<meta class="mktoColor" id="textColor" mktoName="Main Text Color" default="#FFFFFF">`

Esempio di utilizzo:

`${textColor}`

## Booleano {#boolean}

Se specifichi una variabile come Booleana, l’utente finale potrà attivare/disattivare l’opzione nell’editor e-mail. Puoi specificare una variabile Booleana utilizzando `<meta>` con class=“mktoBoolean”

Attributi richiesti

* **id**: il modo in cui fai riferimento alla variabile all’interno del modello e-mail.
* **mktoName**: stringa. Questo è il nome che verrà visualizzato nell’editor e-mail 2.0. Si consiglia di utilizzare un nome descrittivo.

Attributi facoltativi

* **default:** valore booleano che determina lo stato predefinito del pulsante di attivazione/disattivazione. Se omesso, è falso.
* **false_value:** valore da inserire quando il pulsante di attivazione/disattivazione è in posizione OFF (disattivato). Se omesso, è falso.
* **true_value:** valore da inserire quando il pulsante di attivazione/disattivazione è in posizione ON (attivato). Se omesso, è vero.
* **false_value_name:** etichetta visualizzata nell’interfaccia del pulsante di attivazione/disattivazione quando è in posizione OFF (disattivato). Se omesso, è falso.
* **true_value_name:** etichetta visualizzata nell’interfaccia del pulsante di attivazione/disattivazione quando è in posizione ON (attivato). Se omesso, è vero.
* **mktoModuleScope**: booleano. Controlla se la variabile è locale (vero) o globale (falso) quando viene utilizzata in un modulo. Se omesso, il valore predefinito è Falso.

Esempio di dichiarazione:

`<meta class="mktoBoolean" id="showFooter" mktoName="Show Footer BG?" default="false" false_value="transparent" true_value="black" false_value_name="NO" true_value_name="YES">`

Esempio di utilizzo:

`${showFooter}`

## Blocco HTML {#html-block}

Se specifichi una variabile come Blocco HTML, l’utente finale potrà inserire l’HTML non elaborato dall’editor e-mail. Puoi specificare una variabile Blocco HTML utilizzando `<meta>` con class=“mktoHTML”

Attributi richiesti

* **id**: il modo in cui fai riferimento alla variabile all’interno del modello e-mail.
* **mktoName**: stringa. Questo è il nome che verrà visualizzato nell’editor e-mail 2.0. Si consiglia di utilizzare un nome descrittivo.

Attributi facoltativi

* **default:** valore codificato HTML in da utilizzare come contenuto predefinito del blocco.
* **mktoModuleScope**: booleano. Controlla se la variabile è locale (vero) o globale (falso) quando viene utilizzata in un modulo. Se omesso, il valore predefinito è Falso.

Esempio di dichiarazione:

`<meta class="mktoHTML" id="trackingPixel" mktoName="Add Tracking Pixel">`

Esempio di utilizzo:

`${trackingPixel}`

## Variabile immagine {#image-variable}

Se specifichi una variabile come Immagine, l’utente finale potrà scegliere un’immagine dal relativo selettore nell’editor e-mail. L’URL dell’immagine selezionata sarà il valore della variabile. Puoi specificare una variabile Immagine utilizzando `<meta>` con class=“mktoImg”

Attributi richiesti

* **id**: il modo in cui fai riferimento alla variabile all’interno del modello e-mail.
* **mktoName**: stringa. Questo è il nome che verrà visualizzato nell’editor e-mail 2.0. Si consiglia di utilizzare un nome descrittivo.

Attributi facoltativi

* **default:** URL dell’immagine predefinita per l’elemento.
* **mktoModuleScope**: booleano. Controlla se la variabile è locale (vero) o globale (falso) quando viene utilizzata in un modulo. Se omesso, il valore predefinito è Falso.

Esempio di dichiarazione:

`<meta class="mktoImg" id="heroBackgroundImage" mktoName="Hero Background Image" default="https://www.company.com/image.jpg">`

Esempio di utilizzo:

`${heroBackgroundImage}`

## Moduli {#modules}

I moduli sono sezioni predefinite a livello di modello che verranno visualizzate agli utenti finali affinché possano inserirle nelle e-mail. Poiché hai predefinito questi moduli, puoi assicurarti che interagiranno armoniosamente con il resto del contenuto dell’e-mail (in modo completamente reattivo). Puoi inserire solo un modulo all’interno di un contenitore.

>[!IMPORTANT]
>
>Quando un’e-mail viene generata da un modello e-mail che contiene componenti del modulo definiti, qualsiasi modifica apportata ai moduli del modello **non** verrà trasmessa a tale e-mail.

**Per contenitori di tipo `<table>`, `<tbody>`, `<thead>` o `<tfoot>`:**

Può essere specificato utilizzando `<tr>` con class=“mktoModule”

**Per contenitori di tipo `<td>`:**

Può essere specificato utilizzando `<table>` con class=“mktoModule”

Attributi richiesti

* **id**: il modo in cui fai riferimento al modulo all’interno del modello e-mail.
* **mktoName**: stringa. Questo è il nome che verrà visualizzato nell’editor e-mail 2.0. Si consiglia di utilizzare un nome descrittivo.

Attributi facoltativi

* **mktoActive:** determina se questo modulo viene visualizzato nell’elenco dei moduli all’interno dell’editor e-mail. Il valore predefinito è vero. Se falso, il modulo non può essere aggiunto a un’e-mail da un utente finale.
* **mktoAddByDefault:** determina se questo modulo sarà presente nell’area di lavoro di una nuova e-mail che utilizza questo modello al momento della creazione. Il valore predefinito è vero (se mktoActive è falso, questo valore viene ignorato).

>[!NOTE]
>
>I valori delle classi contenenti sintassi Marketo (ad esempio mktoModule, mktoContainer, mktoText) sono soggetti a distinzione tra maiuscole e minuscole. I nomi degli attributi personalizzati (ad esempio mktoimgwidth, mktoname) non lo sono.

## Contenitori {#containers}

Un contenitore contiene i moduli e definisce dove possono essere posizionati. Quando gli utenti finali riordinano e inseriscono moduli nell’e-mail, il contenitore controlla le posizioni in cui possono essere collocati.

**Può essere specificato utilizzando `<table>`, `<tbody>`, `<thead>`, `<tfoot>` o `<td>` con class=“mktoContainer”**

Attributi richiesti

**id**: il modo in cui fai riferimento al modulo all’interno del modello e-mail.

>[!CAUTION]
>
>I contenitori possono contenere solo moduli: se è presente qualcos’altro, il contenitore viene considerato non valido. È consentito un solo contenitore per modello.
