---
unique-page-id: 11371040
description: Sintassi modello e-mail - Documenti Marketo - Documentazione prodotto
title: Sintassi modello e-mail
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '2395'
ht-degree: 0%

---


# Sintassi modello e-mail {#email-template-syntax}

Nella nuova esperienza e-mail 2.0 di Marketo, i modelli e-mail sono composti da qualsiasi combinazione di elementi, variabili, moduli o contenitori. Ciascuno di essi è definito aggiungendo al codice HTML una sintassi specifica di Marketo. I modelli di e-mail precedenti (v1.0) sono supportati in Editor e-mail 2.0; tuttavia, non includeranno tutte le funzioni del nuovo editor.

La sintassi e-mail Marketo funziona solo nei modelli e nelle singole e-mail; se incorporato in snippet o token RTF, non funziona **non**.

>[!NOTE]
>
>Il supporto di Marketo non è impostato per fornire assistenza con CSS/HTML. Se non avete familiarità con CSS/HTML, rivolgetevi al vostro sviluppatore.

>[!CAUTION]
>
>I valori delle classi contenenti la sintassi Marketo (ad es. mktoModule, mktoContainer, mktoText) fanno distinzione tra maiuscole e minuscole. I nomi degli attributi personalizzati (ad es. mktoimgwidth, mktoname) non lo sono.

## Elementi {#elements}

Gli elementi sono aree di contenuto definite come modificabili nel modello e-mail. L&#39;esperienza di modifica di un elemento è univoca per il suo tipo e offre un modo semplice per lavorare con i contenuti. Gli elementi che possono essere inclusi in un modello e-mail sono:

* Rich Text
* Immagini
* Snippet
* Video

## Rich Text {#rich-text}

Se si definisce un&#39;area come RTF, gli utenti potranno modificarne il contenuto [utilizzando l&#39;Editor Rich Text di Marketo](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md). Esistono due modi per definire un elemento RTF all’interno di un modello e-mail: mktEditable e mktoText. Tenete presente che un elemento Rich Text può sempre essere convertito in uno snippet dall’editor e-mail.

### Opzione 1 - mktEditable {#option-mkteditable}

Poiché Editor e-mail 2.0 è retrocompatibile, alcuni vecchi modelli di e-mail potrebbero specificare elementi RTF aggiungendo class=&quot;mktEditable&quot; a qualsiasi elemento HTML. Questo è ancora supportato e l&#39;ID dell&#39;elemento è quello che verrà utilizzato come nome visualizzato all&#39;interno dell&#39;editor e-mail.

Attributi richiesti

* **class**: &quot;mktEditable&quot;.
* **id**: Stringa ID. Contiene solo lettere, numeri, trattino &quot;-&quot; e carattere di sottolineatura &quot;_&quot;. Nessun spazio consentito. Deve essere univoco.

Attributi opzionali

* **mktoName** : Stringa. Questo è il nome visualizzato che verrà visualizzato in Editor e-mail 2.0. Come procedura ottimale si consiglia di utilizzare un nome descrittivo.

Valore predefinito

Il contenuto all&#39;interno dell&#39;elemento HTML (se fornito) con class=&quot;mktEditable&quot; verrà utilizzato come valore predefinito per l&#39;elemento Rich Text.

Esempio:

`<pre data-theme="Confluence"><div class="mktEditable" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div></pre>`

### Opzione 2 - mktoText {#option-mktotext}

Si consiglia di specificare elementi Rich Text utilizzando la sintassi class=&quot;mktoText&quot;. In questo modo viene sempre visualizzato un nome corretto per l&#39;elemento.

Attributi richiesti

* **class**: &quot;mktoText&quot;
* **id**: Stringa ID. Contiene solo lettere, numeri, trattino &quot;-&quot; e carattere di sottolineatura &quot;_&quot;. Nessun spazio consentito. Deve essere univoco.
* **mktoName** : Stringa. Questo è il nome visualizzato che verrà visualizzato in Editor e-mail 2.0. Come procedura ottimale si consiglia di utilizzare un nome descrittivo.

Valore predefinito

Il contenuto all&#39;interno dell&#39;elemento HTML (se fornito) con class=&quot;mktoText&quot; verrà utilizzato come valore predefinito per l&#39;elemento Rich Text.

Esempio:

`<pre data-theme="Confluence"><div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div></pre>`

## Immagini {#images}

Sono disponibili due opzioni per definire gli elementi immagine modificabili. È possibile utilizzare un `<div>` che specifica un contenitore in cui inserire il tag `<img>` oppure un tag `<img>`. Se si desidera che l’utente finale scelga semplicemente un’immagine che restituisca l’URL dell’immagine (anziché il DOM), fare riferimento a &quot;variabili di immagine&quot; nella sezione seguente. Le due opzioni seguenti inseriranno un elemento HTML `<img>`.

### Opzione 1 - Utilizzare un `<div>` {#option-use-a-div}

Attributi richiesti

* **class:** &quot;mktoImg&quot;.
* **stringa id:** ID. Contiene solo lettere, numeri, trattino &quot;-&quot; e carattere di sottolineatura &quot;_&quot;. Nessun spazio consentito. Deve essere univoco.
* **mktoName:** String. Questo è il nome visualizzato che verrà visualizzato in Editor e-mail 2.0. Come procedura ottimale si consiglia di utilizzare un nome descrittivo.

Attributi opzionali

* **mktoImgClass:** String. Il valore qui verrà aggiunto all&#39;attributo class dell&#39;elemento `<img>` all&#39;interno del div.
* **mktoImgSrc:** Da utilizzare come valore predefinito per l&#39;immagine inserita all&#39;interno di questo div. Se omesso, verrà utilizzato un segnaposto.
* **mktoImgLink:** Indicate che il  `<img>` tag deve essere circondato da un  `<a>` tag con questo URL di destinazione. L’utente può modificare questa impostazione nell’editor e-mail.
* **mktoImgLinkTarget:** Indicate che il  `<a>` tag dall’attributo mktoImgLink deve usare questa destinazione. Non ha alcun effetto se non viene utilizzato anche mktoImgLink.
* **mktoImgWidth:** utilizzato come larghezza nella larghezza inclusa  `<img>`.
* **mktoImgHeight:** utilizzata come altezza nella parte racchiusa  `<img>`.
* **mktoLockImgSize:** Utilizzato per sbloccare le proprietà relative all&#39;altezza e alla larghezza dell&#39; `<img>` elemento in modo che l&#39;utente finale possa modificare (l&#39;impostazione predefinita è true se omesso).
* **mktoLockImgStyle:** Utilizzato per bloccare la proprietà di stile dell&#39; `<img>` elemento (il valore predefinito è false).

Valore predefinito (facoltativo)

**`<img>`**: Da usare come  `<img>` elemento in cui verrà inserita l’immagine. Utile per aggiungere all’immagine uno stile in linea. Ricorda di includere i tag `<a> </a>` circostanti, in modo che se l&#39;utente aggiunge un collegamento, lo stile non verrà rimosso!

Esempio:

`<pre data-theme="Confluence"><div class="mktoImg" id="exampleImg" mktoName="Example Image" mktoImgLink="https://www.marketo.com"> <a><img style="border:10px solid red;"></a> </div></pre>`

### Opzione 2 - Utilizzate \&lt;img\> {#option-use-an-img}

>[!NOTE]
>
>Questa opzione non consente agli utenti finali di aggiungere un collegamento alla propria immagine. Utilizzate l&#39;opzione 1 se questo è importante per il modello.

Attributi richiesti

* **class:** &quot;mktoImg&quot;.
* **stringa id:** ID. Contiene solo lettere, numeri, trattino &quot;-&quot; e carattere di sottolineatura &quot;_&quot;. Nessun spazio consentito. Deve essere univoco.
* **mktoName:** String. Questo è il nome visualizzato che verrà visualizzato in Editor e-mail 2.0. Come procedura ottimale si consiglia di utilizzare un nome descrittivo.  Valore predefinito (facoltativo)
* **src:** Da usare come valore predefinito per l&#39;immagine. Se omesso, verrà utilizzato un segnaposto.
* **mktoLockImgSize:** Utilizzato per sbloccare le proprietà relative all&#39;altezza e alla larghezza dell&#39; `<img>` elemento in modo che l&#39;utente finale possa modificare (l&#39;impostazione predefinita è true se omesso).
* **mktoLockImgStyle:** Utilizzato per bloccare la proprietà di stile dell&#39; `<img>` elemento (il valore predefinito è false).

Esempio:
`<pre data-theme="Confluence"><img class="mktoImg" id="exampleImg" mktoName="Example Image"></pre>`

## Snippet {#snippets}

Se definite un&#39;area come snippet, gli utenti finali potranno scegliere quale [snippet](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-snippet-to-an-email.md)approvato inserire in questa area. Sebbene sia possibile convertire gli elementi RTF in snippet dall’editor e-mail, quando si definisce un’area specifica come snippet non è possibile convertirla in RTF. Potete specificare un&#39;area Snippet utilizzando un `<div>` con class=&quot;mktoSnippet&quot;

Attributi richiesti

* **stringa id:** ID. Contiene solo lettere, numeri, trattino &quot;-&quot; e carattere di sottolineatura &quot;_&quot;. Nessun spazio consentito. Deve essere univoco.
* **mktoName:** String. Questo è il nome visualizzato che verrà visualizzato in Editor e-mail 2.0. Come procedura ottimale si consiglia di utilizzare un nome descrittivo.

Valore predefinito (facoltativo)

**mktoDefaultSnippetId**: L&#39;ID numerico dello snippet di Marketo che dovrebbe essere visualizzato per impostazione predefinita (funzionerà solo se uno snippet con tale ID esiste e viene approvato in tale area di lavoro).

Esempio:

`<pre data-theme="Confluence"><div class="mktoSnippet" id="unsubscribeFooter" mktoName="Unsubscribe Footer" mktoDefaultSnippetId="12"></div></pre>`

## Video {#video}

Se definite un&#39;area come video, gli utenti finali potranno inserire un URL YouTube o Vimeo che verrà visualizzato come miniatura (con il pulsante &quot;play&quot;) all&#39;interno dell&#39;e-mail. Potete specificare un&#39;area Video utilizzando un `<div>` con class=&quot;mktoVideo&quot;

Attributi richiesti

* **stringa id:** ID. Contiene solo lettere, numeri, trattino &quot;-&quot; e carattere di sottolineatura &quot;_&quot;. Nessun spazio consentito. Deve essere univoco.
* **mktoName:** String. Questo è il nome visualizzato che verrà visualizzato in Editor e-mail 2.0. Come procedura ottimale si consiglia di utilizzare un nome descrittivo.

Attributi opzionali

* **mktoImgClass:** String. Il valore qui verrà aggiunto all&#39;attributo class della miniatura video `<img>` all&#39;interno del div.

Esempio:

`<pre data-theme="Confluence"><div class="mktoVideo" id="productVideo" mktoName="Product Announcement Video"></div></pre>`

## Variabili {#variables}

Le variabili sono come token. Per prima cosa, è necessario definirli all&#39;interno della sezione `<head>` del modello e-mail utilizzando i tag `<meta>`, quindi utilizzarli il numero desiderato di volte nel modello. Poiché sono definiti nel modello, l&#39;utente finale potrà modificare i propri valori in base alle proprie regole. È possibile definire una variabile come locale o globale nell&#39;ambito. Se si utilizza una variabile all&#39;interno di un &quot;modulo&quot; (vedere di seguito) e un utente finale duplica tale modulo, le variabili locali avranno valori indipendenti, mentre le variabili globali saranno applicabili a entrambi i moduli.

## Stringa {#string}

Se si specifica una variabile come String, l&#39;utente finale potrà immettere del testo all&#39;interno di una casella di testo nell&#39;editor di posta elettronica. È possibile specificare una variabile String utilizzando `<meta>` con class=&quot;mktoString&quot;

Attributi richiesti

* **id:** Come si fa riferimento alla variabile all’interno del modello e-mail.
* **mktoName:** String. Questo è il nome visualizzato che verrà visualizzato in Editor e-mail 2.0. Come procedura ottimale si consiglia di utilizzare un nome descrittivo.

Attributi opzionali

* **allowHTML:** Boolean. Controlla se il valore della variabile è caratterizzato da un carattere di escape HTML. Il valore predefinito è False se viene omesso.
* **predefinito**: Valore predefinito per la stringa. Vuoto se omesso.
* **mktoModuleScope**: Boolean. Controlla se la variabile è locale (true) o globale (false) quando viene utilizzata in un modulo. Il valore predefinito è False se viene omesso.

Esempio di dichiarazione:

`<pre data-theme="Confluence"><meta class="mktoString" id="textHeader" mktoName="Text Header" default="Edit Me"></pre>`

Esempio di utilizzo:

`<pre data-theme="Confluence">${textHeader}</pre>`

## Elenco {#list}

Se si specifica una variabile come Elenco, l’utente finale potrà scegliere tra un set di valori definito nell’editor e-mail. Per specificare una variabile Elenco, utilizzate `<meta>` con class=&quot;mktoList&quot;

Attributi richiesti

* **id**: Come si fa riferimento alla variabile all’interno del modello e-mail.
* **mktoName:** String. Questo è il nome visualizzato che verrà visualizzato in Editor e-mail 2.0. Come procedura ottimale si consiglia di utilizzare un nome descrittivo.
* **valori:elenco di valori separati da** virgole. Deve contenere almeno una stringa.

Attributi opzionali

* **predefinito:valore** predefinito del menu a discesa di selezione. Se omesso, verrà utilizzato il primo valore dell&#39;attributo &quot;values&quot;.
* **mktoModuleScope**: Boolean. Controlla se la variabile è locale (true) o globale (false) quando viene utilizzata in un modulo. Il valore predefinito è False se viene omesso.

Esempio di dichiarazione:

`<pre data-theme="Confluence"><meta class="mktoList" id="textFontFamily" mktoName="Main Text Font Family" values="Arial,Verdana,Times New Roman"></pre>`

Esempio di utilizzo:

`<pre data-theme="Confluence">${textFontFamily}</pre>`

## Numero {#number}

Se si specifica una variabile come numero, l&#39;utente finale potrà immettere un numero nell&#39;editor e-mail. È possibile specificare una variabile Number utilizzando `<meta>` con class=&quot;mktoNumber&quot;

Attributi richiesti

* **id**: Come si fa riferimento alla variabile all’interno del modello e-mail.
* **mktoName**: Stringa. Questo è il nome visualizzato che verrà visualizzato in Editor e-mail 2.0. Come procedura ottimale si consiglia di utilizzare un nome descrittivo.
* **predefinito:valore numerico** predefinito per la variabile.

Attributi opzionali

* **min: valore** minimo accettato.
* **max:** Valore accettato max.
* **unità:** Unità da aggiungere al valore numerico (ad esempio: px, pt, em, ecc.) quando vengono visualizzati nell&#39;Editor e-mail e nel codice risultante.
* **step:** Quante unità la variabile number deve aumentare/diminuire di (0,1, 1, 10, ecc.). Se omesso, il valore predefinito è 1.
* **mktoModuleScope**: Boolean. Controlla se la variabile è locale (true) o globale (false) quando viene utilizzata in un modulo. Il valore predefinito è False se viene omesso.

Esempio di dichiarazione:

`<pre data-theme="Confluence"><meta class="mktoNumber" id="textFontSize" mktoName="Main Text Font Size" default="12" min="8" max="18" units="px" step="1"> </pre>`

Esempio di utilizzo:

`<pre data-theme="Confluence">${textFontSize}</pre>`

## Colore {#color}

Se specificate una variabile come Colore, l’utente finale potrà immettere un valore di colore esadecimale o scegliere un colore dal selettore colore nell’editor e-mail. Per specificare una variabile di colore, utilizzate `<meta>` con class=&quot;mktoColor&quot;

Attributi richiesti

* **id**: Come si fa riferimento alla variabile all’interno del modello e-mail.
* **mktoName**: Stringa. Questo è il nome visualizzato che verrà visualizzato in Editor e-mail 2.0. Come procedura ottimale si consiglia di utilizzare un nome descrittivo.

Attributi opzionali

* **predefinito:valore** predefinito per il colore. Codice colore esadecimale a 6 cifre. Ex: #ffffff.
* **mktoModuleScope**: Boolean. Controlla se la variabile è locale (true) o globale (false) quando viene utilizzata in un modulo. Il valore predefinito è False se viene omesso.

Esempio di dichiarazione:

`<pre data-theme="Confluence"><meta class="mktoColor" id="textColor" mktoName="Main Text Color" default="#FFFFFF"></pre>`

Esempio di utilizzo:

`<pre data-theme="Confluence">${textColor}</pre>`

## Booleano {#boolean}

Se si specifica una variabile come booleana, l&#39;utente finale sarà in grado di attivare/disattivare l&#39;opzione all&#39;interno dell&#39;editor e-mail. È possibile specificare una variabile booleana utilizzando `<meta>` con class=&quot;mktoBoolean&quot;

Attributi richiesti

* **id**: Come si fa riferimento alla variabile all’interno del modello e-mail.
* **mktoName**: Stringa. Questo è il nome visualizzato che verrà visualizzato in Editor e-mail 2.0. Come procedura ottimale si consiglia di utilizzare un nome descrittivo.

Attributi opzionali

* **default:valore** booleano che determina lo stato predefinito dell&#39;interruttore di attivazione/disattivazione. False se omesso.
* **false_value:** Valore da inserire quando l&#39;interruttore è nella posizione OFF. False se omesso.
* **true_value:** Valore da inserire quando l&#39;attivazione è attiva. True se omesso.
* **false_value_name:** interfaccia utente visualizzata nella posizione OFF. False se omesso.
* **true_value_name:** interfaccia utente visualizzata nella posizione Attivato. True se omesso.
* **mktoModuleScope**: Boolean. Controlla se la variabile è locale (true) o globale (false) quando viene utilizzata in un modulo. Il valore predefinito è False se viene omesso.

Esempio di dichiarazione:

`<pre data-theme="Confluence"><meta class="mktoBoolean" id="showFooter" mktoName="Show Footer BG?" default="false" false_value="transparent" true_value="black" false_value_name="NO" true_value_name="YES"></pre>`

Esempio di utilizzo:

`<pre data-theme="Confluence">${showFooter}</pre>`

## Blocco HTML {#html-block}

Se si specifica una variabile come blocco HTML, l&#39;utente finale sarà in grado di inserire il testo HTML integrale dall&#39;editor e-mail. È possibile specificare una variabile Blocco HTML utilizzando `<meta>` con class=&quot;mktoHTML&quot;

Attributi richiesti

* **id**: Come si fa riferimento alla variabile all’interno del modello e-mail.
* **mktoName**: Stringa. Questo è il nome visualizzato che verrà visualizzato in Editor e-mail 2.0. Come procedura ottimale si consiglia di utilizzare un nome descrittivo.

Attributi opzionali

* **predefinito:valore codificato** HTML da utilizzare come contenuto predefinito del blocco.
* **mktoModuleScope**: Boolean. Controlla se la variabile è locale (true) o globale (false) quando viene utilizzata in un modulo. Il valore predefinito è False se viene omesso.

Esempio di dichiarazione:

`<pre data-theme="Confluence"><meta class="mktoHTML" id="trackingPixel" mktoName="Add Tracking Pixel"></pre>`

Esempio di utilizzo:

`<pre data-theme="Confluence">${trackingPixel}</pre>`

## Variabile immagine {#image-variable}

Se specificate una variabile come immagine, l’utente finale potrà scegliere un’immagine dal selettore immagini all’interno dell’editor e-mail. L’URL immagine selezionato sarà il valore della variabile. Per specificare una variabile immagine, utilizzate `<meta>` con class=&quot;mktoImg&quot;

Attributi richiesti

* **id**: Come si fa riferimento alla variabile all’interno del modello e-mail.
* **mktoName**: Stringa. Questo è il nome visualizzato che verrà visualizzato in Editor e-mail 2.0. Come procedura ottimale si consiglia di utilizzare un nome descrittivo.

Attributi opzionali

* **predefinito:URL immagine** predefinita per l’elemento.
* **mktoModuleScope**: Boolean. Controlla se la variabile è locale (true) o globale (false) quando viene utilizzata in un modulo. Il valore predefinito è False se viene omesso.

Esempio di dichiarazione:

`<pre data-theme="Confluence"><meta class="mktoImg" id="heroBackgroundImage" mktoName="Hero Background Image" default="https://www.company.com/image.jpg"></pre>`

Esempio di utilizzo:

`<pre data-theme="Confluence">${heroBackgroundImage}</pre>`

## Moduli {#modules}

I moduli sono sezioni con modelli definite a livello di modello che verranno visualizzate per consentire agli utenti finali di inserire il proprio messaggio e-mail. Poiché questi moduli sono già stati creati, potete assicurarvi che interagiscano con il resto del contenuto delle e-mail in modo corretto (in modo completamente reattivo). È possibile inserire un modulo solo in un contenitore.

**Per contenitori di tipo  `<table>`,  `<tbody>`,  `<thead>`, o  `<tfoot>`:**

Specificato utilizzando `<tr>` con class=&quot;mktoModule&quot;

**Per contenitori di tipo  `<td>`:**

Specificato utilizzando `<table>` con class=&quot;mktoModule&quot;

Attributi richiesti

* **id**: Come si fa riferimento al modulo all’interno del modello e-mail.
* **mktoName**: Stringa. Questo è il nome visualizzato che verrà visualizzato in Editor e-mail 2.0. Come procedura ottimale si consiglia di utilizzare un nome descrittivo.

Attributi opzionali

* **mktoActive:** Determina se il modulo viene visualizzato nell’elenco dei moduli all’interno dell’editor e-mail. Il valore predefinito è true. Se false, il modulo non può essere aggiunto da un utente finale a un&#39;e-mail.
* **mktoAddByDefault:** Determina se il modulo sarà incluso nel quadro di un nuovo messaggio e-mail che utilizza questo modello al momento della creazione. Il valore predefinito è true (se mktoActive è false, questo valore viene ignorato).

>[!NOTE]
>
>I valori delle classi contenenti la sintassi Marketo (ad es. mktoModule, mktoContainer, mktoText) fanno distinzione tra maiuscole e minuscole. I nomi degli attributi personalizzati (ad es. mktoimgwidth, mktoname) non lo sono.

## Contenitori {#containers}

Un contenitore contiene dei moduli e definisce la posizione in cui possono essere posizionati. Quando gli utenti finali riordinano e inseriscono moduli nella propria e-mail, il contenitore controlla dove possono andare.

**Specificato utilizzando  `<table>`,  `<tbody>`,  `<thead>`o  `<tfoot>`   `<td>` con class=&quot;mktoContainer&quot;**

Attributi richiesti

**id**: Come si fa riferimento al modulo all’interno del modello e-mail.

>[!CAUTION]
>
>I contenitori possono contenere solo moduli. Se c&#39;è altro presente, il contenitore è considerato non valido. È consentito un solo contenitore per modello.
