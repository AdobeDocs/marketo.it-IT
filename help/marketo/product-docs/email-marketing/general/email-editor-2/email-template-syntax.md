---
unique-page-id: 11371040
description: Sintassi dei modelli e-mail - Documenti Marketo - Documentazione del prodotto
title: Sintassi del modello e-mail
exl-id: 84d6c0a8-1108-4b7e-8b4f-ac0682c6bdbb
source-git-commit: a59b6b2505c6e5a83c6137a1925aa4e60e56eac8
workflow-type: tm+mt
source-wordcount: '2423'
ht-degree: 0%

---

# Sintassi del modello e-mail {#email-template-syntax}

Nella nuova esperienza e-mail 2.0 di Marketo, i modelli e-mail sono composti da qualsiasi combinazione di elementi, variabili, moduli o contenitori. Ognuna di esse è definita aggiungendo al tuo HTML una sintassi specifica per Marketo. I vecchi modelli e-mail (v1.0) sono supportati in Email Editor 2.0; tuttavia, non includeranno tutte le funzioni del nuovo editor.

La sintassi e-mail Marketo funziona solo nei modelli e nelle singole e-mail; lo fa **not** funziona se è incorporato in snippet o token Rich Text.

>[!NOTE]
>
>Il supporto Marketo non è impostato per l&#39;assistenza con CSS/HTML. Se non hai familiarità con CSS/HTML, consulta il tuo sviluppatore.

>[!CAUTION]
>
>I valori delle classi contenenti la sintassi Marketo (ad esempio mktoModule, mktoContainer, mktoText) fanno distinzione tra maiuscole e minuscole. I nomi degli attributi personalizzati (ad esempio mktoimgwidth, mktoname) non lo sono.

## Elementi {#elements}

Gli elementi sono aree di contenuto definite modificabili nel modello e-mail. L’esperienza di modifica di un elemento è unica nel suo tipo e offre un modo semplice per lavorare con i contenuti. Gli elementi possibili che possono essere inclusi in un modello e-mail sono:

* Rich Text
* Immagini
* Frammenti
* Video

## Rich Text {#rich-text}

Se definisci un’area come RTF, gli utenti potranno modificarne il contenuto [utilizzo dell’editor Rich Text di Marketo](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md). Esistono due modi per definire un elemento Rich Text all’interno di un modello e-mail: mktEditable e mktoText. Tieni presente che un elemento Rich Text può sempre essere convertito in uno snippet dall’interno dell’editor e-mail.

### Opzione 1 - mktEditable {#option-mkteditable}

Poiché Email Editor 2.0 è compatibile con le versioni precedenti, alcuni modelli e-mail precedenti possono specificare elementi di testo RTF aggiungendo class=&quot;mktEditable&quot; su qualsiasi elemento HTML. Questo è ancora supportato e l’ID dell’elemento è ciò che verrà utilizzato come nome visualizzato all’interno dell’editor e-mail.

Attributi richiesti

* **Classe**: &quot;mktEditable&quot;.
* **id**: Stringa ID. Contiene solo lettere, numeri, trattino &quot;-&quot; e trattino basso &quot;_&quot;. Non sono consentiti spazi. Deve essere univoco.

Attributi opzionali

* **mktoName** : Stringa. Questo è il nome visualizzato che verrà visualizzato in Email Editor 2.0. Si consiglia di utilizzare un nome descrittivo.

Valore predefinito

Il contenuto all’interno dell’elemento HTML (se fornito) con class=&quot;mktEditable&quot; verrà utilizzato come valore predefinito per l’elemento Rich Text.

Esempio:

`<pre data-theme="Confluence"><div class="mktEditable" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div></pre>`

### Opzione 2 - mktoText {#option-mktotext}

Si consiglia di specificare gli elementi Rich Text utilizzando la sintassi class=&quot;mktoText&quot;. In questo modo si garantisce che l’elemento disponga sempre di un nome visualizzato corretto.

Attributi richiesti

* **Classe**: &quot;mktoText&quot;
* **id**: Stringa ID. Contiene solo lettere, numeri, trattino &quot;-&quot; e trattino basso &quot;_&quot;. Non sono consentiti spazi. Deve essere univoco.
* **mktoName** : Stringa. Questo è il nome visualizzato che verrà visualizzato in Email Editor 2.0. Si consiglia di utilizzare un nome descrittivo.

Valore predefinito

Il contenuto all’interno dell’elemento HTML (se fornito) con class=&quot;mktoText&quot; verrà utilizzato come valore predefinito per l’elemento Rich Text.

Esempio:

`<pre data-theme="Confluence"><div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div></pre>`

## Immagini {#images}

Sono disponibili due opzioni per la definizione degli elementi immagine modificabili. Puoi utilizzare una delle due opzioni `<div>`, che specifica un contenitore `<img>` verranno inseriti in oppure in `<img>` tag . Se desideri che l’utente finale selezioni semplicemente un’immagine che restituirà l’URL dell’immagine (anziché il DOM), fai riferimento a &quot;variabili immagine&quot; nella sezione seguente. Le due opzioni seguenti consentono di inserire un HTML `<img>` elemento.

### Opzione 1 - Utilizza un `<div>` {#option-use-a-div}

Attributi richiesti

* **Classe:** &quot;mktoImg&quot;.
* **id:** Stringa ID. Contiene solo lettere, numeri, trattino &quot;-&quot; e trattino basso &quot;_&quot;. Non sono consentiti spazi. Deve essere univoco.
* **mktoName :** Stringa. Questo è il nome visualizzato che verrà visualizzato in Email Editor 2.0. Si consiglia di utilizzare un nome descrittivo.

Attributi opzionali

* **mktoImgClass:** Stringa. Il valore qui verrà aggiunto all&#39;attributo class del `<img>` all’interno del div.
* **mktoImgSrc:** Da utilizzare come valore predefinito per l’immagine inserita all’interno di questo div. Se viene omesso, viene utilizzato un segnaposto.
* **mktoImgLink:** Indica che la `<img>` devono essere circondati da un `<a>` con questo URL di destinazione. L’utente può modificarlo nell’editor e-mail.
* **mktoImgLinkTarget:** Indica che la `<a>` Usa questa destinazione dal tag mktoImgLink . Non ha effetto se non viene utilizzato anche mktoImgLink.
* **mktoImgWidth:** Utilizzato come larghezza nel racchiuso `<img>`.
* **mktoImgHeight:** Utilizzato come altezza sul racchiuso `<img>`.
* **mktoLockImgSize:** Utilizzato per sbloccare il `<img>` proprietà height e width dell’elemento in modo che l’utente finale possa modificare (l’impostazione predefinita è true se omesso).
* **mktoLockImgStyle:** Utilizzato per bloccare il `<img>` proprietà di stile dell’elemento (il valore predefinito è false).

Valore predefinito (facoltativo)

**`<img>`**: Da utilizzare come `<img>` che l’immagine verrà inserita. Utile per aggiungere all’immagine uno stile in linea. Ricorda di includere i dati circostanti `<a> </a>` tag, quindi se l’utente aggiunge un collegamento, lo stile non verrà rimosso!

Esempio:

`<pre data-theme="Confluence"><div class="mktoImg" id="exampleImg" mktoName="Example Image" mktoImgLink="https://www.marketo.com"> <a><img style="border:10px solid red;"></a> </div></pre>`

### Opzione 2 - Utilizza un \&lt;img> {#option-use-an-img}

>[!NOTE]
>
>Questa opzione non consente agli utenti finali di aggiungere un collegamento alla propria immagine. Utilizza l&#39;opzione 1 se questo è importante per il modello.

Attributi richiesti

* **Classe:** &quot;mktoImg&quot;.
* **id:** Stringa ID. Contiene solo lettere, numeri, trattino &quot;-&quot; e trattino basso &quot;_&quot;. Non sono consentiti spazi. Deve essere univoco.
* **mktoName:** Stringa. Questo è il nome visualizzato che verrà visualizzato in Email Editor 2.0. Si consiglia di utilizzare un nome descrittivo.  Valore predefinito (facoltativo)
* **src:** Da utilizzare come valore predefinito dell’immagine. Se viene omesso, viene utilizzato un segnaposto.
* **mktoLockImgSize:** Utilizzato per sbloccare il `<img>` proprietà height e width dell’elemento in modo che l’utente finale possa modificare (l’impostazione predefinita è true se omesso).
* **mktoLockImgStyle:** Utilizzato per bloccare il `<img>` proprietà di stile dell’elemento (il valore predefinito è false).

Esempio:
`<pre data-theme="Confluence"><img class="mktoImg" id="exampleImg" mktoName="Example Image"></pre>`

## Frammenti {#snippets}

Se definisci un&#39;area come frammento, gli utenti finali potranno scegliere quale area approvata [Frammento](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-snippet-to-an-email.md)a loro piacerebbe inserire in questa regione. Anche se gli elementi Rich Text possono essere convertiti in snippet dall’interno dell’editor e-mail, quando definisci un’area specifica come frammento non può essere convertita in Rich Text. È possibile specificare un’area Snippet utilizzando un `<div>` con class=&quot;mktoSnippet&quot;

Attributi richiesti

* **id:** Stringa ID. Contiene solo lettere, numeri, trattino &quot;-&quot; e trattino basso &quot;_&quot;. Non sono consentiti spazi. Deve essere univoco.
* **mktoName:** Stringa. Questo è il nome visualizzato che verrà visualizzato in Email Editor 2.0. Si consiglia di utilizzare un nome descrittivo.

Valore predefinito (facoltativo)

**mktoDefaultSnippetId**: L’ID numerico del frammento di Marketo che deve essere visualizzato per impostazione predefinita (funziona solo se un frammento con tale ID esiste e viene approvato in quell’area di lavoro).

Esempio:

`<pre data-theme="Confluence"><div class="mktoSnippet" id="unsubscribeFooter" mktoName="Unsubscribe Footer" mktoDefaultSnippetId="12"></div></pre>`

## Video {#video}

Se definisci un’area come video, gli utenti finali potranno inserire all’interno dell’e-mail un URL YouTube o Vimeo che verrà visualizzato come miniatura (con il pulsante &quot;play&quot;). È possibile specificare un’area video utilizzando una `<div>` con class=&quot;mktoVideo&quot;

Attributi richiesti

* **id:** Stringa ID. Contiene solo lettere, numeri, trattino &quot;-&quot; e trattino basso &quot;_&quot;. Non sono consentiti spazi. Deve essere univoco.
* **mktoName:** Stringa. Questo è il nome visualizzato che verrà visualizzato in Email Editor 2.0. Si consiglia di utilizzare un nome descrittivo.

Attributi opzionali

* **mktoImgClass:** Stringa. Il valore qui verrà aggiunto all’attributo class della miniatura video `<img>` all’interno del div.

Esempio:

`<pre data-theme="Confluence"><div class="mktoVideo" id="productVideo" mktoName="Product Announcement Video"></div></pre>`

## Variabili {#variables}

Le variabili sono come token. Le definisci innanzitutto all’interno della `<head>` sezione del modello e-mail utilizzando `<meta>` , quindi utilizzali il numero di volte desiderato in tutto il modello. Poiché sono definiti nel modello, l’utente finale sarà in grado di modificare i propri valori in base alle proprie regole. È possibile definire una variabile come locale o globale nell’ambito. Se utilizzi una variabile all’interno di un &quot;modulo&quot; (vedi di seguito) e un utente finale duplica tale modulo, le variabili locali avranno valori indipendenti, mentre le variabili globali si applicheranno a entrambi i moduli.

## Stringa {#string}

Se specifichi una variabile come stringa, l’utente finale sarà in grado di immettere testo all’interno di una casella di testo nell’editor e-mail. Specificare una variabile String utilizzando `<meta>` con class=&quot;mktoString&quot;

Attributi richiesti

* **id:** Come si fa riferimento alla variabile all’interno del modello e-mail.
* **mktoName:** Stringa. Questo è il nome visualizzato che verrà visualizzato in Email Editor 2.0. Si consiglia di utilizzare un nome descrittivo.

Attributi opzionali

* **allowHTML:** Booleano. Controlla se il valore della variabile è di tipo HTML-escape. Predefinito su False se omesso.
* **default**: Valore predefinito per la stringa. Vuoto se omesso.
* **mktoModuleScope**: Booleano. Controlla se la variabile è locale (true) o globale (false) quando viene utilizzata in un modulo. Predefinito su False se omesso.

Esempio di dichiarazione:

`<pre data-theme="Confluence"><meta class="mktoString" id="textHeader" mktoName="Text Header" default="Edit Me"></pre>`

Esempio di utilizzo:

`<pre data-theme="Confluence">${textHeader}</pre>`

## Elenco {#list}

Se specifichi una variabile come elenco, l’utente finale sarà in grado di scegliere da un set di valori definito nell’editor e-mail. Specifica una variabile di elenco utilizzando `<meta>` con class=&quot;mktoList&quot;

Attributi richiesti

* **id**: Come si fa riferimento alla variabile all’interno del modello e-mail.
* **mktoName:** Stringa. Questo è il nome visualizzato che verrà visualizzato in Email Editor 2.0. Si consiglia di utilizzare un nome descrittivo.
* **valori:** Elenco di valori separati da virgole. Deve avere almeno una stringa.

Attributi opzionali

* **predefinito:** Valore predefinito del menu a discesa di selezione. Se omesso, verrà utilizzato il primo valore dell&#39;attributo &quot;values&quot;.
* **mktoModuleScope**: Booleano. Controlla se la variabile è locale (true) o globale (false) quando viene utilizzata in un modulo. Predefinito su False se omesso.

Esempio di dichiarazione:

`<pre data-theme="Confluence"><meta class="mktoList" id="textFontFamily" mktoName="Main Text Font Family" values="Arial,Verdana,Times New Roman"></pre>`

Esempio di utilizzo:

`<pre data-theme="Confluence">${textFontFamily}</pre>`

## Numero {#number}

Se specifichi una variabile come numero, l’utente finale sarà in grado di inserire un numero nell’editor e-mail. Specifica una variabile Number utilizzando `<meta>` con class=&quot;mktoNumber&quot;

Attributi richiesti

* **id**: Come si fa riferimento alla variabile all’interno del modello e-mail.
* **mktoName**: Stringa. Questo è il nome visualizzato che verrà visualizzato in Email Editor 2.0. Si consiglia di utilizzare un nome descrittivo.
* **predefinito:** Valore numerico predefinito per la variabile .

Attributi opzionali

* **min** Valore minimo accettato.
* **max:** Valore massimo accettato.
* **unità:** Unità da aggiungere al valore numerico (ad esempio: px, pt, em, ecc.) quando vengono visualizzati nell’editor e-mail e nel codice risultante.
* **passo:** Quante unità la variabile numero dovrebbe aumentare/diminuire di (0.1, 1, 10, ecc.). Se omesso, verrà impostato automaticamente su 1.
* **mktoModuleScope**: Booleano. Controlla se la variabile è locale (true) o globale (false) quando viene utilizzata in un modulo. Predefinito su False se omesso.

Esempio di dichiarazione:

`<pre data-theme="Confluence"><meta class="mktoNumber" id="textFontSize" mktoName="Main Text Font Size" default="12" min="8" max="18" units="px" step="1"> </pre>`

Esempio di utilizzo:

`<pre data-theme="Confluence">${textFontSize}</pre>`

## Colore {#color}

Se specifichi una variabile come Colore, l’utente finale sarà in grado di immettere un valore di colore esadecimale o scegliere un colore dal selettore colore all’interno dell’editor e-mail. È possibile specificare una variabile di colore utilizzando `<meta>` con class=&quot;mktoColor&quot;

Attributi richiesti

* **id**: Come si fa riferimento alla variabile all’interno del modello e-mail.
* **mktoName**: Stringa. Questo è il nome visualizzato che verrà visualizzato in Email Editor 2.0. Si consiglia di utilizzare un nome descrittivo.

Attributi opzionali

* **predefinito:** Valore predefinito per il colore. Codice a colori esadecimale a 6 cifre. Ex: #ffffff.
* **mktoModuleScope**: Booleano. Controlla se la variabile è locale (true) o globale (false) quando viene utilizzata in un modulo. Predefinito su False se omesso.

Esempio di dichiarazione:

`<pre data-theme="Confluence"><meta class="mktoColor" id="textColor" mktoName="Main Text Color" default="#FFFFFF"></pre>`

Esempio di utilizzo:

`<pre data-theme="Confluence">${textColor}</pre>`

## Booleano {#boolean}

Se specifichi una variabile come booleana, l’utente finale sarà in grado di attivare/disattivare l’opzione all’interno dell’editor e-mail. Specifica una variabile booleana utilizzando `<meta>` con class=&quot;mktoBoolean&quot;

Attributi richiesti

* **id**: Come si fa riferimento alla variabile all’interno del modello e-mail.
* **mktoName**: Stringa. Questo è il nome visualizzato che verrà visualizzato in Email Editor 2.0. Si consiglia di utilizzare un nome descrittivo.

Attributi opzionali

* **predefinito:** Valore booleano che determina lo stato predefinito dell&#39;interruttore di attivazione/disattivazione. False se omesso.
* **false_value:** Valore da inserire quando l&#39;interruttore è in posizione OFF. False se omesso.
* **true_value:** Valore da inserire quando l’interruttore è in posizione ON. True se omesso.
* **nome_valore_falso:** L’interfaccia utente viene visualizzata quando è in posizione OFF. False se omesso.
* **nome_valore_vero:** Interfaccia utente visualizzata nell’interruttore quando è attivata. True se omesso.
* **mktoModuleScope**: Booleano. Controlla se la variabile è locale (true) o globale (false) quando viene utilizzata in un modulo. Predefinito su False se omesso.

Esempio di dichiarazione:

`<pre data-theme="Confluence"><meta class="mktoBoolean" id="showFooter" mktoName="Show Footer BG?" default="false" false_value="transparent" true_value="black" false_value_name="NO" true_value_name="YES"></pre>`

Esempio di utilizzo:

`<pre data-theme="Confluence">${showFooter}</pre>`

## Blocco HTML {#html-block}

Se specifichi una variabile come blocco di HTML, l’utente finale sarà in grado di inserire testo HTML letterale dall’interno dell’editor e-mail. È possibile specificare una variabile Blocco di HTML utilizzando `<meta>` con class=&quot;mktoHTML&quot;

Attributi richiesti

* **id**: Come si fa riferimento alla variabile all’interno del modello e-mail.
* **mktoName**: Stringa. Questo è il nome visualizzato che verrà visualizzato in Email Editor 2.0. Si consiglia di utilizzare un nome descrittivo.

Attributi opzionali

* **predefinito:** Valore codificato di HTML da utilizzare come contenuto predefinito del blocco.
* **mktoModuleScope**: Booleano. Controlla se la variabile è locale (true) o globale (false) quando viene utilizzata in un modulo. Predefinito su False se omesso.

Esempio di dichiarazione:

`<pre data-theme="Confluence"><meta class="mktoHTML" id="trackingPixel" mktoName="Add Tracking Pixel"></pre>`

Esempio di utilizzo:

`<pre data-theme="Confluence">${trackingPixel}</pre>`

## Variabile immagine {#image-variable}

Se specifichi una variabile come immagine, l’utente finale sarà in grado di scegliere un’immagine dal selettore immagini all’interno dell’editor e-mail. L’URL immagine selezionato sarà il valore della variabile . Specifica una variabile immagine utilizzando `<meta>` con class=&quot;mktoImg&quot;

Attributi richiesti

* **id**: Come si fa riferimento alla variabile all’interno del modello e-mail.
* **mktoName**: Stringa. Questo è il nome visualizzato che verrà visualizzato in Email Editor 2.0. Si consiglia di utilizzare un nome descrittivo.

Attributi opzionali

* **predefinito:** URL immagine predefinito per l’elemento.
* **mktoModuleScope**: Booleano. Controlla se la variabile è locale (true) o globale (false) quando viene utilizzata in un modulo. Predefinito su False se omesso.

Esempio di dichiarazione:

`<pre data-theme="Confluence"><meta class="mktoImg" id="heroBackgroundImage" mktoName="Hero Background Image" default="https://www.company.com/image.jpg"></pre>`

Esempio di utilizzo:

`<pre data-theme="Confluence">${heroBackgroundImage}</pre>`

## Moduli {#modules}

I moduli sono sezioni di modelli definite a livello di modello che verranno visualizzate per consentire agli utenti finali di inserire nell’e-mail. Poiché questi moduli sono già stati creati, puoi assicurarti che interagiscano con il resto del contenuto delle e-mail in modo gradevole (in modo pienamente reattivo). È possibile inserire un modulo solo in un contenitore.

>[!IMPORTANT]
>
>Quando un messaggio e-mail viene generato da un modello e-mail che contiene componenti modulo definiti, tutte le modifiche apportate ai moduli del modello verranno **not** venga inviato a tale e-mail.

**Per contenitori di tipo `<table>`, `<tbody>`, `<thead>`oppure `<tfoot>`:**

Specificato utilizzando `<tr>` con class=&quot;mktoModule&quot;

**Per contenitori di tipo `<td>`:**

Specificato utilizzando `<table>` con class=&quot;mktoModule&quot;

Attributi richiesti

* **id**: Come si fa riferimento al modulo all’interno del modello e-mail.
* **mktoName**: Stringa. Questo è il nome visualizzato che verrà visualizzato in Email Editor 2.0. Si consiglia di utilizzare un nome descrittivo.

Attributi opzionali

* **mktoActive:** Determina se questo modulo viene visualizzato nell’elenco dei moduli all’interno dell’editor e-mail. Predefinito su true. Se false, il modulo non può essere aggiunto da un utente finale a un&#39;e-mail.
* **mktoAddByDefault:** Determina se questo modulo si troverà nell’area di lavoro di un nuovo messaggio e-mail che utilizza questo modello al momento della creazione. Predefinito su true (se mktoActive è false, questo valore viene ignorato).

>[!NOTE]
>
>I valori delle classi contenenti la sintassi Marketo (ad esempio mktoModule, mktoContainer, mktoText) fanno distinzione tra maiuscole e minuscole. I nomi degli attributi personalizzati (ad esempio mktoimgwidth, mktoname) non lo sono.

## Contenitori {#containers}

Un contenitore contiene Moduli e definisce dove possono essere posizionati. Quando gli utenti finali riordinano e inseriscono moduli nella loro e-mail, il contenitore controlla dove possono andare.

**Specificato utilizzando `<table>`, `<tbody>`, `<thead>`, `<tfoot>` o `<td>` con class=&quot;mktoContainer&quot;**

Attributi richiesti

**id**: Come si fa riferimento al modulo all’interno del modello e-mail.

>[!CAUTION]
>
>I contenitori possono contenere solo moduli - se è presente altro, il contenitore è considerato non valido! È consentito un solo contenitore per modello.
