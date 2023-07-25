---
unique-page-id: 11371040
description: Sintassi del modello e-mail - Documentazione di Marketo - Documentazione del prodotto
title: Sintassi del modello e-mail
exl-id: 84d6c0a8-1108-4b7e-8b4f-ac0682c6bdbb
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '2423'
ht-degree: 0%

---

# Sintassi del modello e-mail {#email-template-syntax}

Nella nuova esperienza E-mail 2.0 di Marketo, i modelli e-mail sono composti da qualsiasi combinazione di elementi, variabili, moduli o contenitori. Ciascuno viene definito aggiungendo una sintassi specifica di Marketo al HTML. I precedenti modelli di e-mail (v1.0) sono supportati in Editor e-mail 2.0; tuttavia, non includeranno tutte le funzioni del nuovo editor.

La sintassi delle e-mail di Marketo funziona solo nei modelli e nelle singole e-mail; funziona **non** funziona se incorporata in snippet o token Rich Text.

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

Se si definisce un&#39;area come Testo formattato, gli utenti potranno modificarne il contenuto [utilizzo dell’editor Rich Text di Marketo](/help/marketo/product-docs/email-marketing/general/understanding-the-email-editor/using-the-rich-text-editor.md). Esistono due modi per definire un elemento Rich Text all’interno di un modello e-mail: mktEditable e mktoText. Nota: un elemento Rich Text può sempre essere convertito in uno snippet dall’interno dell’editor e-mail.

### Opzione 1 - Modificabile {#option-mkteditable}

Poiché Email Editor 2.0 è compatibile con le versioni precedenti, alcuni vecchi modelli di e-mail possono specificare elementi in formato Rich Text aggiungendo class=&quot;mktEditable&quot; a qualsiasi elemento HTML. Questo è ancora supportato e l’ID dell’elemento sarà utilizzato come nome visualizzato all’interno dell’editor e-mail.

Attributi richiesti

* **classe**: &quot;mktEditable&quot;.
* **id**: stringa ID. Contiene solo lettere, numeri, trattini &quot;-&quot; e trattini bassi &quot;_&quot;. Non sono consentiti spazi. Deve essere univoco.

Attributi facoltativi

* **mktoName** : stringa. Questo è il nome visualizzato in Email Editor 2.0. Si consiglia di utilizzare un nome descrittivo.

Valore predefinito

Il contenuto all’interno dell’elemento HTML (se fornito) con class=&quot;mktEditable&quot; verrà utilizzato come valore predefinito per l’elemento Rich Text.

Esempio:

`<pre data-theme="Confluence"><div class="mktEditable" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div></pre>`

### Opzione 2: mktoText {#option-mktotext}

Si consiglia di specificare gli elementi Rich Text utilizzando la sintassi class=&quot;mktoText&quot;. In questo modo viene sempre fornito un nome visualizzato corretto per l’elemento.

Attributi richiesti

* **classe**: &quot;mktoText&quot;
* **id**: stringa ID. Contiene solo lettere, numeri, trattini &quot;-&quot; e trattini bassi &quot;_&quot;. Non sono consentiti spazi. Deve essere univoco.
* **mktoName** : stringa. Questo è il nome visualizzato in Email Editor 2.0. Si consiglia di utilizzare un nome descrittivo.

Valore predefinito

Il contenuto all’interno dell’elemento HTML (se fornito) con class=&quot;mktoText&quot; verrà utilizzato come valore predefinito per l’elemento Rich Text.

Esempio:

`<pre data-theme="Confluence"><div class="mktoText" id="exampleText" mktoName="Main Body Text"> Optionally add default text for the editable text area. </div></pre>`

## Immagini {#images}

Sono disponibili due opzioni per definire gli elementi immagine modificabili. È possibile utilizzare una delle seguenti opzioni `<div>`, che specifica un contenitore in cui `<img>` verrà inserito in, o un `<img>` tag. Se desideri che l’utente finale selezioni semplicemente un’immagine che restituirà l’URL dell’immagine (anziché il DOM), consulta &quot;variabili immagine&quot; nella sezione seguente. Le due opzioni seguenti inseriranno un HTML `<img>` elemento.

### Opzione 1 - Utilizzare un `<div>` {#option-use-a-div}

Attributi richiesti

* **classe:** &quot;mktoImg&quot;
* **id:** Stringa ID. Contiene solo lettere, numeri, trattini &quot;-&quot; e trattini bassi &quot;_&quot;. Non sono consentiti spazi. Deve essere univoco.
* **mktoName:** Stringa. Questo è il nome visualizzato in Email Editor 2.0. Si consiglia di utilizzare un nome descrittivo.

Attributi facoltativi

* **mktoImgClass:** Stringa. Il valore qui verrà aggiunto all’attributo class del `<img>` all&#39;interno del div.
* **mktoImgSrc:** Da utilizzare come valore predefinito per l&#39;immagine inserita in questo div. Se viene omesso, viene utilizzato un segnaposto.
* **mktoImgLink:** Indicare che `<img>` deve essere circondato da un `<a>` con questo URL di destinazione. L’utente può modificarlo nell’Editor e-mail.
* **mktoImgLinkTarget:** Indicare che `<a>` dall&#39;attributo mktoImgLink deve utilizzare questa destinazione. Non produce alcun effetto se non si utilizza anche mktoImgLink.
* **mktoImgWidth:** Utilizzato come larghezza sul racchiuso `<img>`.
* **mktoImgHeight:** Utilizzato come altezza sul racchiuso `<img>`.
* **mktoLockImgSize:** Utilizzato per sbloccare il `<img>` proprietà height e width dell&#39;elemento in modo che l&#39;utente finale possa modificare il valore (se omesso, il valore predefinito è true).
* **mktoLockImgStyle:** Utilizzato per bloccare `<img>` proprietà style dell&#39;elemento (il valore predefinito è false).

Valore predefinito (facoltativo)

**`<img>`**: da utilizzare come `<img>` l&#39;elemento in cui verrà inserita l&#39;immagine. Utile se desideri aggiungere all’immagine uno stile in linea. Ricorda di includere circostante `<a> </a>` , in modo che, se l’utente aggiunge un collegamento, il tuo stile non venga rimosso.

Esempio:

`<pre data-theme="Confluence"><div class="mktoImg" id="exampleImg" mktoName="Example Image" mktoImgLink="https://www.marketo.com"> <a><img style="border:10px solid red;"></a> </div></pre>`

### Opzione 2 - Utilizzare un \&lt;img> {#option-use-an-img}

>[!NOTE]
>
>Questa opzione non consente agli utenti finali di aggiungere un collegamento alla propria immagine. Utilizza l’opzione 1 se è importante per il modello.

Attributi richiesti

* **classe:** &quot;mktoImg&quot;
* **id:** Stringa ID. Contiene solo lettere, numeri, trattini &quot;-&quot; e trattini bassi &quot;_&quot;. Non sono consentiti spazi. Deve essere univoco.
* **mktoName:** Stringa. Questo è il nome visualizzato in Email Editor 2.0. Si consiglia di utilizzare un nome descrittivo.  Valore predefinito (facoltativo)
* **src:** Da utilizzare come valore predefinito per l&#39;immagine. Se viene omesso, viene utilizzato un segnaposto.
* **mktoLockImgSize:** Utilizzato per sbloccare il `<img>` proprietà height e width dell&#39;elemento in modo che l&#39;utente finale possa modificare il valore (se omesso, il valore predefinito è true).
* **mktoLockImgStyle:** Utilizzato per bloccare `<img>` proprietà style dell&#39;elemento (il valore predefinito è false).

Esempio:
`<pre data-theme="Confluence"><img class="mktoImg" id="exampleImg" mktoName="Example Image"></pre>`

## Snippet {#snippets}

Se si definisce un&#39;area come frammento, gli utenti finali potranno scegliere quale approvato [Frammento](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-snippet-to-an-email.md)si desidera inserire in questa area. Sebbene gli elementi Rich Text possano essere convertiti in snippet dall’editor e-mail, quando definisci un’area specifica come Snippet non può essere convertita in Rich Text. È possibile specificare un&#39;area Snippet utilizzando una `<div>` con class=&quot;mktoSnippet&quot;

Attributi richiesti

* **id:** Stringa ID. Contiene solo lettere, numeri, trattini &quot;-&quot; e trattini bassi &quot;_&quot;. Non sono consentiti spazi. Deve essere univoco.
* **mktoName:** Stringa. Questo è il nome visualizzato in Email Editor 2.0. Si consiglia di utilizzare un nome descrittivo.

Valore predefinito (facoltativo)

**mktoDefaultSnippetId**: ID numerico dello snippet di Marketo che deve essere visualizzato per impostazione predefinita (funziona solo se uno snippet con tale ID esiste ed è approvato in tale area di lavoro).

Esempio:

`<pre data-theme="Confluence"><div class="mktoSnippet" id="unsubscribeFooter" mktoName="Unsubscribe Footer" mktoDefaultSnippetId="12"></div></pre>`

## Video {#video}

Se definisci un’area geografica come video, gli utenti finali potranno inserire un URL YouTube o Vimeo da visualizzare come immagine in miniatura (con il pulsante &quot;play&quot;) all’interno dell’e-mail. È possibile specificare un&#39;area Video utilizzando una `<div>` con class=&quot;mktoVideo&quot;

Attributi richiesti

* **id:** Stringa ID. Contiene solo lettere, numeri, trattini &quot;-&quot; e trattini bassi &quot;_&quot;. Non sono consentiti spazi. Deve essere univoco.
* **mktoName:** Stringa. Questo è il nome visualizzato in Email Editor 2.0. Si consiglia di utilizzare un nome descrittivo.

Attributi facoltativi

* **mktoImgClass:** Stringa. Il valore qui verrà aggiunto all’attributo class della miniatura video `<img>` all&#39;interno del div.

Esempio:

`<pre data-theme="Confluence"><div class="mktoVideo" id="productVideo" mktoName="Product Announcement Video"></div></pre>`

## Variabili {#variables}

Le variabili sono simili ai token. Puoi prima definirli all’interno del `<head>` sezione del modello e-mail tramite `<meta>` e utilizzarli tutte le volte che si desidera in tutto il modello. Poiché sono definiti nel modello, l’utente finale sarà in grado di modificare i propri valori in base alle proprie regole. Tieni presente che puoi definire una variabile come locale o globale nell’ambito. Se utilizzi una variabile all’interno di un &quot;modulo&quot; (vedi sotto) e un utente finale duplica tale modulo, le variabili locali avranno valori indipendenti, mentre le variabili globali saranno applicabili a entrambi i moduli.

## Stringa {#string}

Se specifichi una variabile come stringa, l’utente finale potrà immettere il testo all’interno di una casella di testo nell’editor e-mail. È possibile specificare una variabile String utilizzando `<meta>` con class=&quot;mktoString&quot;

Attributi richiesti

* **id:** Come fare riferimento alla variabile all’interno del modello e-mail.
* **mktoName:** Stringa. Questo è il nome visualizzato in Email Editor 2.0. Si consiglia di utilizzare un nome descrittivo.

Attributi facoltativi

* **allowHTML:** Booleano. Controlla se il valore della variabile è con escape per HTML. Se omesso, il valore predefinito è False.
* **predefinito**: valore predefinito per la stringa. Vuoto se omesso.
* **mktoModuleScope**: booleano. Controlla se la variabile è locale (true) o globale (false) quando viene utilizzata in un modulo. Se omesso, il valore predefinito è False.

Esempio di dichiarazione:

`<pre data-theme="Confluence"><meta class="mktoString" id="textHeader" mktoName="Text Header" default="Edit Me"></pre>`

Esempio di utilizzo:

`<pre data-theme="Confluence">${textHeader}</pre>`

## Elenco {#list}

Se specifichi una variabile come Elenco, l’utente finale potrà scegliere da un set di valori definito nell’editor e-mail. È possibile specificare una variabile elenco utilizzando `<meta>` con class=&quot;mktoList&quot;

Attributi richiesti

* **id**: come fai riferimento alla variabile all’interno del modello e-mail.
* **mktoName:** Stringa. Questo è il nome visualizzato in Email Editor 2.0. Si consiglia di utilizzare un nome descrittivo.
* **valori:** Elenco di valori separato da virgole. Deve essere presente almeno una stringa.

Attributi facoltativi

* **impostazione predefinita:** Valore predefinito del menu a discesa di selezione. Se omesso, viene utilizzato il primo valore dell’attributo &quot;values&quot;.
* **mktoModuleScope**: booleano. Controlla se la variabile è locale (true) o globale (false) quando viene utilizzata in un modulo. Se omesso, il valore predefinito è False.

Esempio di dichiarazione:

`<pre data-theme="Confluence"><meta class="mktoList" id="textFontFamily" mktoName="Main Text Font Family" values="Arial,Verdana,Times New Roman"></pre>`

Esempio di utilizzo:

`<pre data-theme="Confluence">${textFontFamily}</pre>`

## Numero {#number}

Se specifichi una variabile come Numero, l’utente finale potrà immettere un numero nell’editor e-mail. È possibile specificare una variabile Numerica utilizzando `<meta>` con class=&quot;mktoNumber&quot;

Attributi richiesti

* **id**: come fai riferimento alla variabile all’interno del modello e-mail.
* **mktoName**: stringa. Questo è il nome visualizzato in Email Editor 2.0. Si consiglia di utilizzare un nome descrittivo.
* **impostazione predefinita:** Valore numerico predefinito per la variabile.

Attributi facoltativi

* **min.:** Valore minimo accettato.
* **max:** Valore massimo accettato.
* **unità:** Unità da aggiungere al valore numerico (es: px, pt, em, ecc.) quando viene visualizzato nell’Editor e-mail e nel codice risultante.
* **passaggio:** Quante unità la variabile numerica deve aumentare/diminuire di (0,1, 1, 10, ecc.). Se omesso, il valore predefinito è 1.
* **mktoModuleScope**: booleano. Controlla se la variabile è locale (true) o globale (false) quando viene utilizzata in un modulo. Se omesso, il valore predefinito è False.

Esempio di dichiarazione:

`<pre data-theme="Confluence"><meta class="mktoNumber" id="textFontSize" mktoName="Main Text Font Size" default="12" min="8" max="18" units="px" step="1"> </pre>`

Esempio di utilizzo:

`<pre data-theme="Confluence">${textFontSize}</pre>`

## Colore {#color}

Se specifichi una variabile come Colore, l’utente finale potrà immettere un valore di colore esadecimale o scegliere un colore dal selettore colore all’interno dell’editor e-mail. È possibile specificare una variabile Colore utilizzando `<meta>` con class=&quot;mktoColor&quot;

Attributi richiesti

* **id**: come fai riferimento alla variabile all’interno del modello e-mail.
* **mktoName**: stringa. Questo è il nome visualizzato in Email Editor 2.0. Si consiglia di utilizzare un nome descrittivo.

Attributi facoltativi

* **impostazione predefinita:** Valore predefinito per il colore. Codice colore esadecimale a 6 cifre. Esempio: #ffffff.
* **mktoModuleScope**: booleano. Controlla se la variabile è locale (true) o globale (false) quando viene utilizzata in un modulo. Se omesso, il valore predefinito è False.

Esempio di dichiarazione:

`<pre data-theme="Confluence"><meta class="mktoColor" id="textColor" mktoName="Main Text Color" default="#FFFFFF"></pre>`

Esempio di utilizzo:

`<pre data-theme="Confluence">${textColor}</pre>`

## Booleano {#boolean}

Se specifichi una variabile come booleano, l’utente finale potrà attivare/disattivare l’opzione nell’editor e-mail. È possibile specificare una variabile booleana utilizzando `<meta>` con class=&quot;mktoBoolean&quot;

Attributi richiesti

* **id**: come fai riferimento alla variabile all’interno del modello e-mail.
* **mktoName**: stringa. Questo è il nome visualizzato in Email Editor 2.0. Si consiglia di utilizzare un nome descrittivo.

Attributi facoltativi

* **impostazione predefinita:** Valore booleano che determina lo stato predefinito dell’interruttore di attivazione. False se omesso.
* **false_value:** Valore da inserire quando l’interruttore è in posizione OFF. False se omesso.
* **true_value:** Valore da inserire quando l&#39;interruttore è in posizione ON. True se omesso.
* **nome_valore_falso:** L’interfaccia utente visualizzata in attiva/disattiva quando è in posizione OFF. False se omesso.
* **true_value_name:** L&#39;interfaccia utente visualizzata in attiva/disattiva. True se omesso.
* **mktoModuleScope**: booleano. Controlla se la variabile è locale (true) o globale (false) quando viene utilizzata in un modulo. Se omesso, il valore predefinito è False.

Esempio di dichiarazione:

`<pre data-theme="Confluence"><meta class="mktoBoolean" id="showFooter" mktoName="Show Footer BG?" default="false" false_value="transparent" true_value="black" false_value_name="NO" true_value_name="YES"></pre>`

Esempio di utilizzo:

`<pre data-theme="Confluence">${showFooter}</pre>`

## Blocco HTML {#html-block}

Se specifichi una variabile come HTML Block (Blocco di HTML), l’utente finale potrà inserire testo letterale nell’editor e-mail. È possibile specificare una variabile HTML Block utilizzando `<meta>` con class=&quot;mktoHTML&quot;

Attributi richiesti

* **id**: come fai riferimento alla variabile all’interno del modello e-mail.
* **mktoName**: stringa. Questo è il nome visualizzato in Email Editor 2.0. Si consiglia di utilizzare un nome descrittivo.

Attributi facoltativi

* **impostazione predefinita:** Valore con codifica HTML da utilizzare come contenuto predefinito del blocco.
* **mktoModuleScope**: booleano. Controlla se la variabile è locale (true) o globale (false) quando viene utilizzata in un modulo. Se omesso, il valore predefinito è False.

Esempio di dichiarazione:

`<pre data-theme="Confluence"><meta class="mktoHTML" id="trackingPixel" mktoName="Add Tracking Pixel"></pre>`

Esempio di utilizzo:

`<pre data-theme="Confluence">${trackingPixel}</pre>`

## Variabile immagine {#image-variable}

Se specifichi una variabile come Immagine, l’utente finale potrà scegliere un’immagine dal selettore delle immagini nell’editor e-mail. L’URL immagine selezionato sarà il valore della variabile. È possibile specificare una variabile immagine utilizzando `<meta>` con class=&quot;mktoImg&quot;

Attributi richiesti

* **id**: come fai riferimento alla variabile all’interno del modello e-mail.
* **mktoName**: stringa. Questo è il nome visualizzato in Email Editor 2.0. Si consiglia di utilizzare un nome descrittivo.

Attributi facoltativi

* **impostazione predefinita:** URL immagine predefinito per l’elemento.
* **mktoModuleScope**: booleano. Controlla se la variabile è locale (true) o globale (false) quando viene utilizzata in un modulo. Se omesso, il valore predefinito è False.

Esempio di dichiarazione:

`<pre data-theme="Confluence"><meta class="mktoImg" id="heroBackgroundImage" mktoName="Hero Background Image" default="https://www.company.com/image.jpg"></pre>`

Esempio di utilizzo:

`<pre data-theme="Confluence">${heroBackgroundImage}</pre>`

## Moduli {#modules}

I moduli sono sezioni con modelli definite a livello di modello che verranno visualizzate e inserite dagli utenti finali nelle e-mail. Poiché questi moduli sono stati pregenerati, puoi assicurarti che interagiranno con il resto del contenuto dell’e-mail in modo agevole (in modo completamente reattivo). Puoi inserire un modulo solo in un contenitore.

>[!IMPORTANT]
>
>Quando un’e-mail viene generata da un modello e-mail che contiene componenti modulo definiti, eventuali modifiche apportate ai moduli del modello **non** essere inviato a tale e-mail.

**Per contenitori di tipo `<table>`, `<tbody>`, `<thead>`, o `<tfoot>`:**

Specificato tramite `<tr>` con class=&quot;mktoModule&quot;

**Per contenitori di tipo `<td>`:**

Specificato tramite `<table>` con class=&quot;mktoModule&quot;

Attributi richiesti

* **id**: come fai riferimento al modulo all’interno del modello e-mail.
* **mktoName**: stringa. Questo è il nome visualizzato in Email Editor 2.0. Si consiglia di utilizzare un nome descrittivo.

Attributi facoltativi

* **mktoActive:** Determina se questo modulo viene visualizzato nell’elenco dei moduli all’interno dell’editor e-mail. Impostazione predefinita: true. Se false, il modulo non può essere aggiunto a un’e-mail da un utente finale.
* **mktoAddByDefault:** Determina se questo modulo verrà incluso nell’area di lavoro di una nuova e-mail che utilizza questo modello al momento della creazione. Il valore predefinito è true (se mktoActive è false, questo valore viene ignorato).

>[!NOTE]
>
>I valori delle classi contenenti la sintassi Marketo (ad esempio mktoModule, mktoContainer, mktoText) fanno distinzione tra maiuscole e minuscole. I nomi degli attributi personalizzati (ad esempio mktoimgwidth, mktoname) non sono consentiti.

## Contenitori {#containers}

Un contenitore contiene i Moduli e definisce dove possono essere posizionati. Quando gli utenti finali riordinano e inseriscono moduli nelle e-mail, il contenitore controlla dove possono andare.

**Specificato utilizzando `<table>`, `<tbody>`, `<thead>`, `<tfoot>` o `<td>` con class=&quot;mktoContainer&quot;**

Attributi richiesti

**id**: come fai riferimento al modulo all’interno del modello e-mail.

>[!CAUTION]
>
>I contenitori possono contenere solo moduli: se è presente qualcos’altro, il contenitore viene considerato non valido. È consentito un solo contenitore per modello.
