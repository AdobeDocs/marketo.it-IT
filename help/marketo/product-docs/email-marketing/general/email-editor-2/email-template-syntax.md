---
unique-page-id: 11371040
description: Sintassi del modello e-mail - Documentazione di Marketo - Documentazione del prodotto
title: Sintassi del modello e-mail
exl-id: 84d6c0a8-1108-4b7e-8b4f-ac0682c6bdbb
feature: Email Editor
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '2449'
ht-degree: 2%

---

# Sintassi del modello e-mail {#email-template-syntax}

Nella nuova esperienza E-mail 2.0 di Marketo, i modelli e-mail sono composti da qualsiasi combinazione di elementi, variabili, moduli o contenitori. Ciascuno viene definito aggiungendo la sintassi specifica di Marketo al HTML. I precedenti modelli di e-mail (v1.0) sono supportati in Editor e-mail 2.0; tuttavia, non includeranno tutte le funzioni del nuovo editor.

La sintassi delle e-mail di Marketo funziona solo nei modelli e nelle singole e-mail; **non** funziona se incorporata in snippet o token Rich Text.

>[!NOTE]
>
>Il supporto Marketo non è configurato per l’assistenza con CSS/HTML. Se non conosci CSS/HTML, consulta il tuo sviluppatore.

>[!CAUTION]
>
>I valori delle classi contenenti la sintassi Marketo (ad esempio mktoModule, mktoContainer, mktoText) fanno distinzione tra maiuscole e minuscole. I nomi degli attributi personalizzati (ad esempio mktoimgwidth, mktoname) non sono consentiti.

## Elementi {#elements}

Gli elementi sono aree di contenuto che puoi definire modificabili nel modello e-mail. L’esperienza di modifica di un elemento è unica per il suo tipo e offre un modo semplice di lavorare con il contenuto. I possibili elementi che possono essere inclusi in un modello e-mail sono:

* Rich Text
* Immagini
* Snippet
* Video

## Rich Text {#rich-text}

Se si definisce un&#39;area come Rich Text, gli utenti potranno modificarne il contenuto [utilizzando l&#39;Editor Rich Text di Marketo](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md). Esistono due modi per definire un elemento Rich Text all’interno di un modello e-mail: mktEditable e mktoText. Nota: un elemento Rich Text può sempre essere convertito in uno snippet dall’interno dell’editor e-mail.

### Opzione 1 - Modificabile {#option-mkteditable}

Poiché Email Editor 2.0 è compatibile con le versioni precedenti, alcuni vecchi modelli e-mail possono specificare elementi in formato Rich Text aggiungendo class=&quot;mktEditable&quot; a qualsiasi elemento di HTML. Questo è ancora supportato e l’ID dell’elemento sarà utilizzato come nome visualizzato all’interno dell’editor e-mail.

Attributi richiesti

* **classe**: &quot;mktEditable&quot;.
* **id**: stringa ID. Contiene solo lettere, numeri, trattini &quot;-&quot; e trattini bassi &quot;_&quot;. Non sono consentiti spazi. Deve essere univoco.

Attributi facoltativi

* **mktoName**: stringa. Questo è il nome visualizzato in Email Editor 2.0. Si consiglia di utilizzare un nome descrittivo.

Valore predefinito

Il contenuto all’interno dell’elemento HTML (se fornito) con class=&quot;mktEditable&quot; verrà utilizzato come valore predefinito per l’elemento Rich Text.

Esempio:

`<div class="mktEditable" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div>`

### Opzione 2: mktoText {#option-mktotext}

Si consiglia di specificare gli elementi Rich Text utilizzando la sintassi class=&quot;mktoText&quot;. In questo modo viene sempre fornito un nome visualizzato corretto per l’elemento.

Attributi richiesti

* **classe**: &quot;mktoText&quot;
* **id**: stringa ID. Contiene solo lettere, numeri, trattini &quot;-&quot; e trattini bassi &quot;_&quot;. Non sono consentiti spazi. Deve essere univoco.
* **mktoName**: stringa. Questo è il nome visualizzato in Email Editor 2.0. Si consiglia di utilizzare un nome descrittivo.

Valore predefinito

Il contenuto all’interno dell’elemento HTML (se fornito) con class=&quot;mktoText&quot; verrà utilizzato come valore predefinito per l’elemento Rich Text.

Esempio:

`<div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div>`

## Immagini {#images}

Sono disponibili due opzioni per definire gli elementi immagine modificabili. È possibile utilizzare un tag `<div>`, che specifica un contenitore in cui verrà inserito `<img>`, o un tag `<img>`. Se desideri che l’utente finale selezioni semplicemente un’immagine che restituirà l’URL dell’immagine (anziché il DOM), consulta &quot;variabili immagine&quot; nella sezione seguente. Nelle due opzioni seguenti verrà inserito un elemento HTML `<img>`.

### Opzione 1 - Utilizzare `<div>` {#option-use-a-div}

Attributi richiesti

* **classe:** &quot;mktoImg&quot;.
* **id:** stringa ID. Contiene solo lettere, numeri, trattini &quot;-&quot; e trattini bassi &quot;_&quot;. Non sono consentiti spazi. Deve essere univoco.
* **mktoName :** Stringa. Questo è il nome visualizzato in Email Editor 2.0. Si consiglia di utilizzare un nome descrittivo.

Attributi facoltativi

* **mktoImgClass:** Stringa. Il valore verrà aggiunto all&#39;attributo class dell&#39;elemento `<img>` all&#39;interno del div.
* **mktoImgSrc:** Da utilizzare come valore predefinito per l&#39;immagine inserita in questo div. Se viene omesso, viene utilizzato un segnaposto.
* **mktoImgLink:** Indica che `<img>` deve essere circondato da un tag `<a>` con questo URL di destinazione. L’utente può modificarlo nell’Editor e-mail.
* **mktoImgLinkTarget:** Indica che il tag `<a>` dell&#39;attributo mktoImgLink deve utilizzare questa destinazione. Non produce alcun effetto se non si utilizza anche mktoImgLink.
* **mktoImgWidth:** Utilizzata come larghezza del `<img>` allegato.
* **mktoImgHeight:** Utilizzata come altezza nell&#39;allegato `<img>`.
* **mktoLockImgSize:** Utilizzato per sbloccare la proprietà height e width dell&#39;elemento `<img>` in modo che l&#39;utente finale possa modificarla (se omesso, l&#39;impostazione predefinita è true).
* **mktoLockImgStyle:** Utilizzato per bloccare la proprietà di stile dell&#39;elemento `<img>` (il valore predefinito è false).

Valore predefinito (facoltativo)

**`<img>`**: da utilizzare come elemento `<img>` in cui verrà inserita l&#39;immagine. Utile se desideri aggiungere all’immagine uno stile in linea. Ricordati di includere i tag `<a> </a>` circostanti, quindi se l&#39;utente aggiunge un collegamento, lo stile non verrà rimosso.

Esempio:

`<div class="mktoImg" id="exampleImg" mktoName="Example Image" mktoImgLink="https://www.marketo.com"> <a><img style="border:10px solid red;"></a> </div>`

### Opzione 2 - Utilizzare un \&lt;img\> {#option-use-an-img}

>[!NOTE]
>
>Questa opzione non consente agli utenti finali di aggiungere un collegamento alla propria immagine. Utilizza l’opzione 1 se è importante per il modello.

Attributi richiesti

* **classe:** &quot;mktoImg&quot;.
* **id:** stringa ID. Contiene solo lettere, numeri, trattini &quot;-&quot; e trattini bassi &quot;_&quot;. Non sono consentiti spazi. Deve essere univoco.
* **mktoName:** stringa. Questo è il nome visualizzato in Email Editor 2.0. Si consiglia di utilizzare un nome descrittivo.  Valore predefinito (facoltativo)
* **src:** Da utilizzare come valore predefinito per l&#39;immagine. Se viene omesso, viene utilizzato un segnaposto.
* **mktoLockImgSize:** Utilizzato per sbloccare la proprietà height e width dell&#39;elemento `<img>` in modo che l&#39;utente finale possa modificarla (se omesso, l&#39;impostazione predefinita è true).
* **mktoLockImgStyle:** Utilizzato per bloccare la proprietà di stile dell&#39;elemento `<img>` (il valore predefinito è false).

Esempio:
`<img class="mktoImg" id="exampleImg" mktoName="Example Image">`

## Snippet {#snippets}

Se definisci un&#39;area come Snippet, gli utenti finali potranno scegliere quale [Snippet](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-snippet-to-an-email.md)hanno approvato e desiderano inserire in questa area. Sebbene gli elementi Rich Text possano essere convertiti in snippet dall’editor e-mail, quando definisci un’area specifica come Snippet non può essere convertita in Rich Text. È possibile specificare un&#39;area Snippet utilizzando `<div>` con class=&quot;mktoSnippet&quot;

Attributi richiesti

* **id:** stringa ID. Contiene solo lettere, numeri, trattini &quot;-&quot; e trattini bassi &quot;_&quot;. Non sono consentiti spazi. Deve essere univoco.
* **mktoName:** stringa. Questo è il nome visualizzato in Email Editor 2.0. Si consiglia di utilizzare un nome descrittivo.

Valore predefinito (facoltativo)

**mktoDefaultSnippetId**: l&#39;ID numerico dello snippet di Marketo che deve essere visualizzato per impostazione predefinita (funziona solo se uno snippet con tale ID esiste ed è approvato in tale area di lavoro).

Esempio:

`<div class="mktoSnippet" id="unsubscribeFooter" mktoName="Unsubscribe Footer" mktoDefaultSnippetId="12"></div>`

## Video {#video}

Se definisci un’area geografica come video, gli utenti finali potranno inserire un URL YouTube o Vimeo da visualizzare come immagine in miniatura (con il pulsante &quot;play&quot;) all’interno dell’e-mail. È possibile specificare un&#39;area Video utilizzando `<div>` con class=&quot;mktoVideo&quot;

Attributi richiesti

* **id:** stringa ID. Contiene solo lettere, numeri, trattini &quot;-&quot; e trattini bassi &quot;_&quot;. Non sono consentiti spazi. Deve essere univoco.
* **mktoName:** stringa. Questo è il nome visualizzato in Email Editor 2.0. Si consiglia di utilizzare un nome descrittivo.

Attributi facoltativi

* **mktoImgClass:** Stringa. Il valore qui verrà aggiunto all&#39;attributo class della miniatura video `<img>` all&#39;interno del div.

Esempio:

`<div class="mktoVideo" id="productVideo" mktoName="Product Announcement Video"></div>`

## Variabili {#variables}

Le variabili sono simili ai token. Puoi innanzitutto definirli all&#39;interno della sezione `<head>` del modello di e-mail utilizzando `<meta>` tag, quindi utilizzarli tutte le volte che desideri in tutto il modello. Poiché sono definiti nel modello, l’utente finale sarà in grado di modificare i propri valori in base alle proprie regole. Tieni presente che puoi definire una variabile come locale o globale nell’ambito. Se utilizzi una variabile all’interno di un &quot;modulo&quot; (vedi sotto) e un utente finale duplica tale modulo, le variabili locali avranno valori indipendenti, mentre le variabili globali saranno applicabili a entrambi i moduli.

## Stringa {#string}

Se specifichi una variabile come stringa, l’utente finale potrà immettere il testo all’interno di una casella di testo nell’editor e-mail. È possibile specificare una variabile String utilizzando `<meta>` con class=&quot;mktoString&quot;

Attributi richiesti

* **id:** Come si fa riferimento alla variabile all&#39;interno del modello di e-mail.
* **mktoName:** stringa. Questo è il nome visualizzato in Email Editor 2.0. Si consiglia di utilizzare un nome descrittivo.

Attributi facoltativi

* **allowHTML:** Boolean. Controlla se il valore della variabile è con escape HTML. Se omesso, il valore predefinito è False.
* **default**: valore predefinito per la stringa. Vuoto se omesso.
* **mktoModuleScope**: valore booleano. Controlla se la variabile è locale (true) o globale (false) quando viene utilizzata in un modulo. Se omesso, il valore predefinito è False.

Esempio di dichiarazione:

`<meta class="mktoString" id="textHeader" mktoName="Text Header" default="Edit Me">`

Esempio di utilizzo:

`${textHeader}`

## Elenco {#list}

Se specifichi una variabile come Elenco, l’utente finale potrà scegliere da un set di valori definito nell’editor e-mail. È stata specificata una variabile List utilizzando `<meta>` con class=&quot;mktoList&quot;

Attributi richiesti

* **id**: come fare riferimento alla variabile all&#39;interno del modello e-mail.
* **mktoName:** stringa. Questo è il nome visualizzato in Email Editor 2.0. Si consiglia di utilizzare un nome descrittivo.
* **valori:** elenco di valori separato da virgole. Deve essere presente almeno una stringa.

Attributi facoltativi

* **default:** Valore predefinito del menu a discesa di selezione. Se omesso, viene utilizzato il primo valore dell’attributo &quot;values&quot;.
* **mktoModuleScope**: valore booleano. Controlla se la variabile è locale (true) o globale (false) quando viene utilizzata in un modulo. Se omesso, il valore predefinito è False.

Esempio di dichiarazione:

`<meta class="mktoList" id="textFontFamily" mktoName="Main Text Font Family" values="Arial,Verdana,Times New Roman">`

Esempio di utilizzo:

`${textFontFamily}`

## Numero {#number}

Se specifichi una variabile come Numero, l’utente finale potrà immettere un numero nell’editor e-mail. Specificare una variabile Number utilizzando `<meta>` con class=&quot;mktoNumber&quot;

Attributi richiesti

* **id**: come fare riferimento alla variabile all&#39;interno del modello e-mail.
* **mktoName**: stringa. Questo è il nome visualizzato in Email Editor 2.0. Si consiglia di utilizzare un nome descrittivo.
* **default:** Valore numerico predefinito per la variabile.

Attributi facoltativi

* **min:** valore minimo accettato.
* **max:** valore massimo accettato.
* **unità:** unità da aggiungere al valore numerico (ad es. px, pt, em, ecc.) quando vengono visualizzate nell&#39;editor e-mail e nel codice risultante.
* **passaggio:** quante unità la variabile numerica deve aumentare/diminuire di (0,1, 1, 10, ecc.). Se omesso, il valore predefinito è 1.
* **mktoModuleScope**: valore booleano. Controlla se la variabile è locale (true) o globale (false) quando viene utilizzata in un modulo. Se omesso, il valore predefinito è False.

Esempio di dichiarazione:

`<meta class="mktoNumber" id="textFontSize" mktoName="Main Text Font Size" default="12" min="8" max="18" units="px" step="1">`

Esempio di utilizzo:

`${textFontSize}`

## Colore {#color}

Se specifichi una variabile come Colore, l’utente finale potrà immettere un valore di colore esadecimale o scegliere un colore dal selettore colore all’interno dell’editor e-mail. È stata specificata una variabile Color utilizzando `<meta>` con class=&quot;mktoColor&quot;

Attributi richiesti

* **id**: come fare riferimento alla variabile all&#39;interno del modello e-mail.
* **mktoName**: stringa. Questo è il nome visualizzato in Email Editor 2.0. Si consiglia di utilizzare un nome descrittivo.

Attributi facoltativi

* **default:** Valore predefinito per il colore. Codice colore esadecimale a 6 cifre. Esempio: #ffffff.
* **mktoModuleScope**: valore booleano. Controlla se la variabile è locale (true) o globale (false) quando viene utilizzata in un modulo. Se omesso, il valore predefinito è False.

Esempio di dichiarazione:

`<meta class="mktoColor" id="textColor" mktoName="Main Text Color" default="#FFFFFF">`

Esempio di utilizzo:

`${textColor}`

## Booleano {#boolean}

Se specifichi una variabile come booleano, l’utente finale potrà attivare/disattivare l’opzione nell’editor e-mail. Specificare una variabile booleana utilizzando `<meta>` con class=&quot;mktoBoolean&quot;

Attributi richiesti

* **id**: come fare riferimento alla variabile all&#39;interno del modello e-mail.
* **mktoName**: stringa. Questo è il nome visualizzato in Email Editor 2.0. Si consiglia di utilizzare un nome descrittivo.

Attributi facoltativi

* **default:** valore booleano che determina lo stato predefinito dell&#39;interruttore di attivazione. False se omesso.
* **false_value:** Valore da inserire quando l&#39;interruttore è in posizione OFF. False se omesso.
* **true_value:** Valore da inserire quando l&#39;interruttore è in posizione ON. True se omesso.
* **false_value_name:** Interfaccia utente visualizzata quando è in posizione OFF. False se omesso.
* **true_value_name:** UI mostrata nell&#39;interruttore quando è in posizione ON. True se omesso.
* **mktoModuleScope**: valore booleano. Controlla se la variabile è locale (true) o globale (false) quando viene utilizzata in un modulo. Se omesso, il valore predefinito è False.

Esempio di dichiarazione:

`<meta class="mktoBoolean" id="showFooter" mktoName="Show Footer BG?" default="false" false_value="transparent" true_value="black" false_value_name="NO" true_value_name="YES">`

Esempio di utilizzo:

`${showFooter}`

## Blocco HTML {#html-block}

Se specifichi una variabile come blocco HTML, l’utente finale potrà inserire il testo letterale di HTML dall’editor e-mail. È stata specificata una variabile di blocco HTML utilizzando `<meta>` con class=&quot;mktoHTML&quot;

Attributi richiesti

* **id**: come fare riferimento alla variabile all&#39;interno del modello e-mail.
* **mktoName**: stringa. Questo è il nome visualizzato in Email Editor 2.0. Si consiglia di utilizzare un nome descrittivo.

Attributi facoltativi

* **valore predefinito:** valore codificato HTML da utilizzare come contenuto predefinito del blocco.
* **mktoModuleScope**: valore booleano. Controlla se la variabile è locale (true) o globale (false) quando viene utilizzata in un modulo. Se omesso, il valore predefinito è False.

Esempio di dichiarazione:

`<meta class="mktoHTML" id="trackingPixel" mktoName="Add Tracking Pixel">`

Esempio di utilizzo:

`${trackingPixel}`

## Variabile immagine {#image-variable}

Se specifichi una variabile come Immagine, l’utente finale potrà scegliere un’immagine dal selettore delle immagini nell’editor e-mail. L’URL immagine selezionato sarà il valore della variabile. È stata specificata una variabile immagine utilizzando `<meta>` con class=&quot;mktoImg&quot;

Attributi richiesti

* **id**: come fare riferimento alla variabile all&#39;interno del modello e-mail.
* **mktoName**: stringa. Questo è il nome visualizzato in Email Editor 2.0. Si consiglia di utilizzare un nome descrittivo.

Attributi facoltativi

* **default:** URL immagine predefinito per l&#39;elemento.
* **mktoModuleScope**: valore booleano. Controlla se la variabile è locale (true) o globale (false) quando viene utilizzata in un modulo. Se omesso, il valore predefinito è False.

Esempio di dichiarazione:

`<meta class="mktoImg" id="heroBackgroundImage" mktoName="Hero Background Image" default="https://www.company.com/image.jpg">`

Esempio di utilizzo:

`${heroBackgroundImage}`

## Moduli {#modules}

I moduli sono sezioni con modelli definite a livello di modello che verranno visualizzate e inserite dagli utenti finali nelle e-mail. Poiché questi moduli sono stati pregenerati, puoi assicurarti che interagiranno con il resto del contenuto dell’e-mail in modo agevole (in modo completamente reattivo). Puoi inserire un modulo solo in un contenitore.

>[!IMPORTANT]
>
>Quando un messaggio e-mail viene generato da un modello e-mail che contiene componenti modulo definiti, eventuali modifiche apportate ai moduli del modello **non** verranno inviate a tale messaggio e-mail.

**Per contenitori di tipo `<table>`, `<tbody>`, `<thead>` o `<tfoot>`:**

Specificato utilizzando `<tr>` con class=&quot;mktoModule&quot;

**Per contenitori di tipo `<td>`:**

Specificato utilizzando `<table>` con class=&quot;mktoModule&quot;

Attributi richiesti

* **id**: come fai riferimento al modulo nel modello e-mail.
* **mktoName**: stringa. Questo è il nome visualizzato in Email Editor 2.0. Si consiglia di utilizzare un nome descrittivo.

Attributi facoltativi

* **mktoActive:** Determina se questo modulo viene visualizzato nell&#39;elenco dei moduli all&#39;interno dell&#39;editor di posta elettronica. Impostazione predefinita: true. Se false, il modulo non può essere aggiunto a un’e-mail da un utente finale.
* **mktoAddByDefault:** Determina se il modulo verrà incluso nell&#39;area di lavoro di un nuovo messaggio di posta elettronica che utilizza questo modello al momento della creazione. Il valore predefinito è true (se mktoActive è false, questo valore viene ignorato).

>[!NOTE]
>
>I valori delle classi contenenti la sintassi Marketo (ad esempio mktoModule, mktoContainer, mktoText) fanno distinzione tra maiuscole e minuscole. I nomi degli attributi personalizzati (ad esempio mktoimgwidth, mktoname) non sono consentiti.

## Contenitori {#containers}

Un contenitore contiene i Moduli e definisce dove possono essere posizionati. Quando gli utenti finali riordinano e inseriscono moduli nelle e-mail, il contenitore controlla dove possono andare.

**Specificato utilizzando `<table>`, `<tbody>`, `<thead>`, `<tfoot>` o `<td>` con class=&quot;mktoContainer&quot;**

Attributi richiesti

**id**: come fai riferimento al modulo nel modello e-mail.

>[!CAUTION]
>
>I contenitori possono contenere solo moduli: se è presente qualcos’altro, il contenitore viene considerato non valido. È consentito un solo contenitore per modello.
