---
solution: Marketo Engage
product: marketo
title: Frammenti personalizzabili
description: Scopri come personalizzare i frammenti rendendo modificabili alcuni campi. Creare frammenti riutilizzabili flessibili in E-mail Designer.
level: Beginner, Intermediate
feature: Email Designer
role: User
exl-id: 3e0232c7-13bd-49e2-b7c7-cd389b5f0704
TQID: https://experienceleague.adobe.com/SCmyn9QUECmvQgVltKknlvLuvL15Tz3LYorBFYB1hqI
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
  - id: e8ccd51f-da0d-4e3b-939b-e30d5ebb1ea5
topic_v2:
  - id: e0eb8757-182f-49f3-94a4-1587d16f5094
source-git-commit: fdc003d7aed05d85687427d9455bb806eb33d0b2
workflow-type: tm+mt
source-wordcount: 1398
ht-degree: 0%

---

# Frammenti personalizzabili {#customizable-fragments}

Quando i frammenti vengono utilizzati in un’e-mail o in un modello e-mail, vengono bloccati per impostazione predefinita a causa dell’ereditarietà, il che significa che eventuali modifiche apportate a un frammento vengono propagate automaticamente a tutte le risorse in cui viene utilizzato. Con i frammenti personalizzabili, campi specifici all’interno di un frammento possono essere definiti come modificabili quando il frammento viene aggiunto a un’e-mail o a un modello e-mail. Ad esempio, se disponi di un frammento con un banner, del testo e un pulsante, puoi designare come modificabili alcuni campi, ad esempio l’URL di destinazione dell’immagine o del pulsante.

I frammenti personalizzabili consentono di gestire e personalizzare il contenuto senza creare blocchi di contenuto completamente nuovi o interrompere l’ereditarietà dei frammenti. Le modifiche apportate a livello di frammento vengono comunque propagate, consentendo al contempo la personalizzazione a livello di e-mail o modello e-mail.

I frammenti visivi e di espressione possono essere contrassegnati come personalizzabili.

## Aggiungere campi modificabili nei frammenti visivi {#visual}

Per rendere modificabili parti di un frammento visivo, effettua le seguenti operazioni:

>[!NOTE]
>
>I campi modificabili possono essere aggiunti ai componenti **image**, **text** e **button**. Per i componenti di **HTML**, i campi modificabili vengono aggiunti utilizzando l&#39;editor di personalizzazione, in modo simile ai frammenti di espressione. [Scopri i campi modificabili nei componenti HTML nei frammenti](#editable-html)

1. Apri la schermata di modifica del contenuto del frammento.

1. Seleziona il componente nel frammento in cui desideri configurare i campi modificabili.

1. Il riquadro delle proprietà del componente viene visualizzato sul lato destro. Selezionare la scheda **[!UICONTROL Editable fields]**, quindi attivare/disattivare l&#39;opzione **[!UICONTROL Enable edition]**.

1. Tutti i campi che possono essere modificati per il componente selezionato sono elencati nel riquadro. I campi disponibili per la modifica dipendono dal tipo di componente selezionato.

   Nell’esempio seguente, l’URL del pulsante &quot;Fai clic qui&quot; è configurato come modificabile.

   ![](assets/fragment-param-enable.png){width="800" zoomable="yes"}

1. Fare clic su **[!UICONTROL Overview]** per controllare tutti i campi modificabili e i relativi valori predefiniti.

   In questo esempio, il campo URL del pulsante viene visualizzato con il valore predefinito definito nel componente. Gli utenti possono personalizzare questo valore dopo aver aggiunto il frammento al loro contenuto.

   ![](assets/fragment-param-preview.png){width="800" zoomable="yes"}

1. Al termine, salva le modifiche.

Dopo aver aggiunto il frammento a un messaggio e-mail, gli utenti possono personalizzare tutti i campi modificabili configurati nel frammento.

## Componenti HTML modificabili nei frammenti {#editable-html}

All’interno di un componente HTML, è possibile modificare i seguenti tipi di elementi:

* Parte di **contenuto di testo** (ad esempio, un titolo o un&#39;etichetta CTA).
* **URL** completo, utilizzato come destinazione di collegamento o come origine immagine. Gli URL parziali non sono supportati; la variabile deve rappresentare l’intero valore URL.
* Valore completo della proprietà **CSS** (ad esempio, un valore di colore, di riempimento o di larghezza). I valori parziali delle proprietà CSS non sono supportati.

Ogni valore della proprietà CSS con parametri deve essere esattamente `{{{varName}}}`: nessun suffisso, nessun testo aggiuntivo, nessuna variabile multipla e nessuna concatenazione all&#39;interno di una singola proprietà.

Per parametrizzare proprietà multilaterali come la spaziatura interna:

* dichiarare ogni lato come una proprietà separata _(consigliato)_, oppure
* dichiarare una singola variabile che contiene il valore di sintassi abbreviata completo.

## Funzionamento dei campi modificabili nei componenti di HTML {#components}

I campi modificabili in un componente HTML vengono creati dichiarando le variabili in linea direttamente all’interno del codice sorgente del componente. Ogni variabile ha un ID univoco e un valore predefinito. Viene quindi fatto riferimento alla variabile ogni volta che il valore modificabile deve essere visualizzato nel markup.

Una volta salvato e pubblicato il frammento, ogni variabile dichiarata nel componente HTML viene automaticamente visualizzata come parametro modificabile quando il frammento viene aggiunto a un messaggio e-mail.

L’autore dell’e-mail può quindi sovrascrivere il valore predefinito di qualsiasi variabile di E-mail Designer (ad esempio, modificando un colore di sfondo, scambiando un URL CTA o aggiornando un titolo) senza modificare il HTML sottostante.

## Riferimento sintassi {#syntax}

I campi modificabili sono definiti e referenziati utilizzando due pattern:

### Dichiarazione di una variabile {#declaring}

Utilizza la dichiarazione in linea per definire una variabile con un ID univoco e un valore predefinito:

```handlebars
{{#inline "variableID"}}default_value{{/inline}}
```

Sostituire `variableID` con un identificatore univoco per il campo modificabile. L’ID deve essere univoco all’interno del componente e non deve contenere spazi.

Sostituire `default_value` con il valore che deve essere utilizzato se l&#39;autore e-mail non lo sostituisce.

### Riferimento a una variabile {#referencing}

Utilizza parentesi graffe triple per fare riferimento alla variabile ovunque il relativo valore dovrebbe apparire nel markup:

```handlebars
{{{variableID}}}
```

È possibile fare riferimento allo stesso ID variabile un numero qualsiasi di volte all’interno di HTML. Tutti i riferimenti verranno risolti in base al valore impostato dall’autore dell’e-mail (o al valore predefinito, se non viene fornita alcuna sostituzione).

### Parametri opzionali {#optional}

La dichiarazione in linea supporta parametri facoltativi che modificano la modalità di presentazione o elaborazione del campo modificabile:

| Azione | Parametro | Esempio |
|---|---|---|
| Dichiara un campo modificabile con un **valore predefinito**. Quando il frammento viene aggiunto a un messaggio e-mail, viene utilizzato questo valore predefinito a meno che l’autore non lo ignori. | Aggiungi il valore predefinito tra i tag in linea. | `{{#inline "editableFieldID"}}default_value{{/inline}}` |
| Definisci una **etichetta** per il campo modificabile. Questa etichetta viene visualizzata in E-mail Designer quando l’autore dell’e-mail modifica i campi del frammento. | `name="title"` | `{{#inline "editableFieldID" name="title"}}default_value{{/inline}}` |
| Dichiara un campo modificabile che contiene una **origine immagine**. | `assetType="image"` | `{{#inline "editableFieldID" assetType="image"}}default_value{{/inline}}` |
| Dichiara un campo modificabile contenente un **URL** che deve essere tracciato. | `assetType="url"` | `{{#inline "editableFieldID" assetType="url"}}default_value{{/inline}}` |

## Aggiunta di campi modificabili a un componente HTML {#adding-editable-fields}

Per rendere modificabili parti di un componente HTML all’interno di un frammento visivo, effettua le seguenti operazioni:

1. Apri il frammento visivo per la modifica in E-mail Designer.
1. Aggiungere un **componente HTML** al frammento dal pannello Componenti oppure selezionare un componente HTML esistente.
1. Con il componente HTML selezionato, fai clic su **Mostra codice sorgente** per aprire la visualizzazione origine di HTML nell&#39;editor di personalizzazione.
1. Nell’editor di personalizzazione, dichiara ogni variabile modificabile utilizzando la sintassi di dichiarazione in linea. Posiziona tutte le dichiarazioni di variabili nella parte superiore del componente per migliorarne la leggibilità e assegna a ciascuna variabile un ID univoco.
1. Fare riferimento a ogni variabile nel markup HTML utilizzando la sintassi `{{{variableID}}}` ovunque debba essere visualizzato il valore modificabile. È possibile fare riferimento più volte alla stessa variabile nello stesso componente.
1. Salva il componente HTML, quindi salva il frammento.
1. Pubblica il frammento per renderlo disponibile nelle e-mail.

## Utilizzo del frammento in un messaggio e-mail {#using-fragment}

Dopo la pubblicazione del frammento, tutte le variabili dichiarate nei suoi componenti HTML vengono visualizzate come parametri modificabili in E-mail Designer.

Per personalizzarli quando si utilizza il frammento in un messaggio e-mail:

1. Apri o crea un’e-mail in Marketo Engage Email Designer.
1. Aggiungi il frammento pubblicato all’area di lavoro dell’e-mail.
1. Seleziona il frammento per aprirne il riquadro delle proprietà. L&#39;elenco dei campi modificabili viene visualizzato nella sezione **Campi modificabili**, con ogni campo etichettato dal relativo ID variabile (o dall&#39;etichetta descrittiva specificata tramite il parametro `name`).
1. Aggiorna il valore di qualsiasi campo modificabile direttamente dal riquadro delle proprietà. La modifica si applica solo all’e-mail corrente; il frammento pubblicato e le altre e-mail che vi fanno riferimento rimangono invariati.
1. Salva l’e-mail.

Il frammento viene riprodotto con i valori personalizzati, ereditando comunque eventuali aggiornamenti strutturali futuri apportati al frammento pubblicato.

### Esempio: frammento semplice con testo, colore e URL modificabili {#example}

L’esempio seguente crea un piccolo banner promozionale con quattro campi modificabili:

* un colore di sfondo
* un testo del titolo
* un’etichetta CTA
* un URL CTA

Dopo aver pubblicato il frammento, un autore e-mail può ignorare uno di questi valori quando aggiunge il frammento a un messaggio e-mail.

**Banner semplice e modificabile**

```html
<!-- Define editable variables -->
{{#inline "bgColor"}}#0057FF{{/inline}}
{{#inline "headlineText"}}Example Headline{{/inline}}
{{#inline "ctaText"}}Learn More{{/inline}}
{{#inline "ctaUrl" assetType="url"}}https://www.example.com{{/inline}}

<!-- Use the variables in the HTML -->
<table width="100%" cellpadding="0" cellspacing="0"
       style="background-color:{{{bgColor}}}; border-radius:8px;" >
  <tr>
    <td style="padding:30px; text-align:center; font-family:Arial,sans-serif;">
      <h2 style="color:#ffffff; font-size:24px; margin:0;">
        {{{headlineText}}}
      </h2>
      <a href="{{{ctaUrl}}}"
         style="display:inline-block; margin-top:16px; padding:12px 28px;
                background:#ffffff; color:{{{bgColor}}};
                font-weight:bold; border-radius:4px; text-decoration:none;">
        {{{ctaText}}}
      </a>
    </td>
  </tr>
</table>
```

In questo esempio:

* Viene fatto riferimento a `bgColor` due volte: una volta per il colore di sfondo della tabella e una volta per il colore del testo di CTA. Entrambi i riferimenti vengono risolti sullo stesso valore, pertanto una singola modifica viene propagata a entrambe le posizioni.
* `ctaUrl` è dichiarato con `assetType="url"`, che indica che il valore deve essere elaborato come URL tracciato.

## Best practice {#best-practices}

* Includi le unità (`px`, `em`, `%`) nel valore predefinito della variabile in modo che la variabile rappresenti un valore CSS completo. Questo evita la concatenazione, che non è supportata.
* Preferisci proprietà CSS lato lungo (`padding-top`, `padding-right`, `padding-bottom`, `padding-left`) rispetto alla scorciatoia quando potrebbe essere necessario modificare ogni lato in modo indipendente.
* Quando un URL deve essere tracciato, dichiaralo con `assetType="url"`.
* Se un campo modificabile contiene un&#39;origine immagine, dichiararlo con `assetType="image"`.
* Verifica il frammento aggiungendolo a una bozza di e-mail e verificando che tutti i campi modificabili siano visualizzati nel riquadro delle proprietà e che vengano risolti correttamente quando vengono sostituiti.

## Aspetti da considerare {#things-to-know}

* I campi modificabili nei componenti di HTML supportano il contenuto full-text, gli URL completi e i valori completi delle proprietà CSS. Gli URL parziali e i valori parziali delle proprietà CSS non possono essere parametrizzati.
* Un singolo valore di proprietà CSS non può combinare una variabile con testo statico aggiuntivo o con un’altra variabile. Ogni valore di proprietà con parametri deve essere esattamente un riferimento di variabile.
* Gli ID delle variabili devono essere univoci all’interno di un componente HTML e non devono contenere spazi.
* I collegamenti di sistema predefiniti, come il collegamento per annullare l’abbonamento e l’URL della pagina speculare, non possono essere trasformati in campi modificabili.

<!--
## Add editable fields in HTML components and expression fragments {#expression}

To make portions of an HTML component or an expression fragment editable, you must use a specific syntax in the expression editor. This involves declaring a _variable_ with a default value that users can override after adding the fragment to their content.

For example, suppose you want to create a fragment to add to your emails, and allow users to customize a specific color used in different locations, such as frames or buttons' background colors. When creating your fragment, you need to declare a variable with a _unique ID_ (e.g., "color"), and call it at the desired locations in the fragment content where you want to apply this color. When adding the fragment to their content, users will be able to customize the color used wherever the variable is referenced.

For HTML components, only specific elements can become editable fields. Expand the section below for more information.

+++Editable elements in HTML components:

The elements below can become editable fields in an HTML component:

* A portion of text
* A full URL for link or image (doesn't work with portion of a URL)
* Entire CSS property (doesn't work with partial property)

For example, in the code below, each element highlighted in red can become a property:

![](assets/fragment-html.png){width="500" zoomable="yes"}

+++
-->

>[!MORELIKETHIS]
>
>[Frammenti](/help/marketo/product-docs/email-marketing/email-designer/fragments.md){target="_blank"}
