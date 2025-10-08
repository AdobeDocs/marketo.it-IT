---
title: Progettare contenuti accessibili
description: Scopri come progettare contenuti accessibili per le e-mail in Adobe Marketo Engage.
feature: Email Designer
role: User
level: Beginner, Intermediate
keywords: e-mail, progettazione, accessibilità
source-git-commit: 5adfebfd8f9f0cdaebb1eb86a68c136d46298446
workflow-type: tm+mt
source-wordcount: '1359'
ht-degree: 0%

---

# Progettare contenuti accessibili {#accessible-content}

L&#39;[atto europeo sull&#39;accessibilità](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A32019L0882){target="_blank"} è una direttiva intesa a migliorare il mercato interno dei prodotti e dei servizi accessibili eliminando gli ostacoli causati da norme nazionali divergenti tra gli Stati membri.

Questo regolamento stabilisce che tutte le comunicazioni digitali, inclusi e-mail, newsletter, PDF e contenuti scaricabili, devono essere accessibili. Durante la creazione di contenuti per i destinatari, è quindi necessario seguire linee guida specifiche, ad esempio utilizzare font accessibili e formati leggibili e fornire testo alternativo per le immagini.

Marketo Engage Email Designer consente di conformarsi facilmente a questa direttiva, in base alle linee guida WCAG (Web Content Accessibility Guidelines) 2.1, livello AA. Di seguito sono elencate le best practice per la progettazione di contenuti accessibili con Marketo Engage.

>[!NOTE]
>
>In questa pagina puoi rendere il contenuto accessibile a tutti i destinatari in modo che le persone con disabilità possano leggere, comprendere e interagire con le e-mail progettate in Marketo Engage.

## Assicurare la leggibilità del testo {#text-readability}

Sfrutta la scheda **[!UICONTROL Styles]** del componente **[!UICONTROL Text]** per garantire la leggibilità del testo, ad esempio l&#39;utilizzo di un contrasto cromatico appropriato e di font semplici.

<!--![](assets/accessible-text-styles.png){width="80%"}-->

Per i font e il testo, attenetevi alle seguenti linee guida:

**Selezione carattere**

* Utilizza font sans-serif come Arial, Verdana, Tahoma, Helvetica o Open Sans.
* Evita font serif, corsivi o decorativi nel contenuto del corpo.
* Attenersi a un set di caratteri limitato per coerenza e fallback (ad esempio: `font-family: Arial, Helvetica, sans-serif;`).

**Dimensione font**

* Assicurati che la dimensione minima del font per il corpo del testo sia 16 px.
* Utilizza la gerarchia corretta per le intestazioni.

**Contrasto colore**

* Mantenere un rapporto di contrasto di almeno 4,5:1 tra testo e sfondo.
* Per il testo di grandi dimensioni (≥24 px o 18 px in grassetto), assicurati di ottenere un contrasto di almeno 3:1.
* Evitare il testo grigio chiaro o pastello su sfondi bianchi.
* Non fare affidamento solo sul colore per trasmettere il significato. Usa sottolineature, icone, ecc.

**Accessibilità testo**

* Evitare il testo nelle immagini.
* Non utilizzare tutte le maiuscole nel corpo del testo.
* Assicurati che il testo possa essere ingrandito fino al 200% senza interrompere il layout.

## Garantire l’accessibilità visiva {#visual-accessibility}

* Evitare di utilizzare indicatori di solo colore per informazioni importanti.
* Utilizza etichette di testo o icone per maggiore chiarezza.
* Ottimizza la progettazione per layout mobili e reattivi, garantendo pulsanti grandi e spaziati correttamente.
* Esegui regolarmente test tra dispositivi e dimensioni dello schermo per mantenere l’accessibilità.

In Marketo Engage, le dimensioni e la spaziatura dei diversi elementi del contenuto possono essere ulteriormente migliorate utilizzando i parametri e gli attributi di stile dal riquadro E-mail Designer **[!UICONTROL Styles]**.

Ad esempio, è possibile aggiornare lo sfondo o modificare i margini, la spaziatura interna e l&#39;allineamento per migliorare l&#39;accessibilità visiva.

<!--![](assets/accessible-styles.png){width="80%"}-->

Marketo Engage Email Designer consente di visualizzare in anteprima e ottimizzare il design per diversi dispositivi e dimensioni di schermo. In qualsiasi momento è possibile **[!UICONTROL Switch to live view]** per verificare come il contenuto potrebbe essere riprodotto su dispositivi di varie dimensioni.

<!--![](assets/accessible-live-view.png){width="80%"}-->

>[!CAUTION]
>
>La visualizzazione live è un’anteprima generica progettata per confrontare il modo in cui il contenuto potrebbe essere riprodotto tra varie dimensioni di dispositivo. Il rendering finale può variare a seconda del client e-mail del destinatario.

## Usa testo alternativo per le immagini {#alt-text}

Utilizzare il componente **[!UICONTROL Image]** per fornire testo alternativo per le immagini.

<!--![](assets/accessible-alt-text.png){width="90%"}-->

* Descrivi lo scopo dell’immagine in modo conciso e contestuale.
* Evita frasi ridondanti come &quot;Immagine di ...&quot; e utilizza testo alternativo vuoto per le immagini decorative.
* Per le icone con significato, fornisci etichette significative e per le immagini complesse, utilizza un breve testo alternativo più una descrizione più lunga altrove.

## Usa formato leggibile {#readable-format}

Utilizza la struttura e i componenti di contenuto rilevanti di E-mail Designer, nonché le opzioni nel riquadro **[!UICONTROL Styles]**, per organizzare il contenuto in modo chiaro, logico e conciso, accessibile a tutti.

<!--![](assets/accessible-components.png){width="100%"}-->

* Utilizza HTML semantico e strutturato con intestazioni, paragrafi, elenchi e tabelle corretti.
* Assicurati che il contenuto segua un flusso logico da sinistra a destra e dall’alto al basso.
* Utilizza un linguaggio chiaro e conciso.
* Fornire formati alternativi per PDF e infografiche.
* Consenti il ridimensionamento e il riversamento del testo e assicurati che la composizione tipografica sia leggibile con un contrasto del colore adeguato in tutti i formati.

## Garantire la leggibilità dei contenuti {#readability}

Per essere leggibile, il contenuto deve essere chiaro, ben strutturato e utilizzabile da tutti, comprese le persone con difficoltà visive, cognitive o di lettura e quelle che utilizzano tecnologie per l’accessibilità. Alcuni punti da considerare durante la creazione di contenuto accessibile includono:

* Mantieni le frasi a un massimo di 20 parole.
* Modifica la tua copia in modo che sia diretta e concisa.
* Utilizza la voce attiva per semplificare la struttura della frase.
* Evita di usare parole gergali, gergali o regionali che alcuni potrebbero non conoscere.

Per valutare la leggibilità delle e-mail, puoi utilizzare il popolare [test di facilità di lettura Flesch](https://support.microsoft.com/en-us/office/get-your-document-s-readability-and-level-statistics-85b4969e-e80a-4777-8dd3-f7fc3c8b3fd2){target="_blank"}, disponibile in Microsoft Word, che calcola la facilità di lettura dei contenuti su una scala da 0 a 100.

## Verifica il contenuto {#test}

Per verificare l’accessibilità dei contenuti, puoi utilizzare le funzionalità di test fornite da Marketo Engage. Non sono progettate specificamente per verificare se il contenuto è completamente accessibile, ma possono fornire un primo livello di verifica.

* Visualizza l’anteprima del contenuto utilizzando i profili di test.

* Utilizza l&#39;opzione [Rendering di e-mail](/help/marketo/product-docs/email-marketing/email-designer/test-email-rendering.md){target="_blank"} che sfrutta Litmus per simulare le progettazioni tra i principali client e-mail (Apple Mail, Gmail, Outlook) e vedere se testo, colori e immagini rendono accessibili i contenuti. <!--Litmus includes accessibility testing-->

* Invia bozze per testare il rendering del contenuto prima di inviarlo al pubblico reale.

<!--![](assets/accessible-simulate.png){width="90%"}-->

Per eseguire il check-in in modo più coerente se il contenuto è accessibile in modo affidabile, cerca strumenti esterni specifici come:

* Il [Verifica contrasto WebAim](https://webaim.org/resources/contrastchecker/){target="_blank"} e lo strumento di valutazione dell&#39;accessibilità Web [WAVE](https://wave.webaim.org/){target="_blank"} per valutare il contrasto e la conformità;

* Tecnologie per l&#39;accessibilità, come gli assistenti vocali (ad esempio: [NVDA](https://www.nvaccess.org/download/){target="_blank"} o [VoiceOver](https://support.apple.com/en-ie/guide/iphone/iph3e2e415f/ios){target="_blank"} su iPhone), per visualizzare le e-mail dal punto di vista degli utenti ipovedenti.

## Usa modalità scura {#dark-mode}

[Modalità scura](/help/marketo/product-docs/email-marketing/email-designer/dark-mode.md){target="_blank"} migliora l&#39;accessibilità visiva per gli utenti con sensibilità alla luce o problemi di vista, per una migliore esperienza di visualizzazione.

<!--![](assets/accessible-dark-mode.png){width="90%"}-->

Alcune best practice per la progettazione di contenuti in modalità scura includono:

* Utilizzo di PNG o SVG trasparenti
* Impostazione di metatag e CSS appropriati
* Fornire uno stile di fallback accessibile se la modalità scura non è supportata.

Assicurati che il rendering delle e-mail venga eseguito correttamente in modalità scura, sottoponendo a test tutto il contenuto delle e-mail e gli elementi dell’interfaccia utente sia in modalità chiara che scura.

## Utilizzare attributi specifici per l&#39;accessibilità {#attributes}

### Attributi della lingua {#language}

Durante la creazione delle progettazioni, includere gli attributi `lang` (lingua) e `dir` (direzione del testo) nel corpo del contenuto. Questi attributi consentono alle tecnologie per l’accessibilità (come gli assistenti vocali) di interpretare e presentare il contenuto in modo appropriato.

* L&#39;attributo `lang` indica la lingua dell&#39;e-mail per le tecnologie per l&#39;accessibilità, garantendo che le parole vengano pronunciate correttamente.

  +++Esempi

  Esempio di inglese:

  ```
  <body lang="en">
  ```

  Esempio di francese:

  ```
  <body lang="fr">
  ```

  +++

* L&#39;attributo `dir` specifica la direzione del testo. La maggior parte delle lingue, tra cui l&#39;inglese e il francese, sono lette da sinistra a destra (ltr), mentre le lingue come l&#39;arabo e l&#39;ebraico sono lette da destra a sinistra (rtl).

  +++Esempi

  Esempio di inglese (da sinistra a destra):

  ```html
  <body lang="en" dir="ltr">
  ```

  Esempio di arabo (da destra a sinistra):

  ```html
  <body lang="ar" dir="rtl">
  ```

  +++

Gli assistenti vocali si basano sull&#39;attributo `lang` per applicare le regole di pronuncia corrette, mentre la direzione del testo garantisce un flusso di contenuto naturale per le lingue da sinistra a destra o da destra a sinistra. Senza questi attributi, gli utenti potrebbero riscontrare un ordine di lettura confuso o una pronuncia errata. Racchiudi sempre il corpo dell&#39;e-mail con gli attributi `lang` e `dir` appropriati.

>[!TIP]
>
>Se l&#39;e-mail contiene più lingue, assegnare gli attributi della lingua appropriati a sezioni specifiche (ad esempio `<table>` o `<td>` blocchi) per garantire che ogni parte sia letta correttamente.

### Tabelle {#tables}

Nel contenuto di HTML, le tabelle vengono spesso utilizzate per il layout. Per impostazione predefinita, gli assistenti vocali trattano ogni `<table>` come una tabella dati, annunciando righe, colonne e struttura. Questo può creare confusione se la tabella viene utilizzata solo per la formattazione.

Aggiungi `role="presentation"` (o `role="none"`) alle tabelle layout per garantire che le tecnologie per l&#39;accessibilità saltino la struttura e si concentrino solo sul contenuto effettivo.

+++Esempio: tabella layout (con `role="presentation"`)

```html
<table role="presentation" border="0" cellpadding="0" cellspacing="0" width="100%"> 
  <tr> 
    <td align="center"> 
      <h1>Hello World</h1> 
      <p>Welcome to our newsletter</p> 
    </td> 
  </tr> 
</table>
```

Gli assistenti vocali leggono:
&quot;Hello World. Benvenuto nella nostra newsletter.&quot; _(Nessuna menzione di righe, colonne o tabelle)_

+++

+++Esempio - Tabella dati (senza `role="presentation"`)

```html
<table border="1" cellpadding="5" cellspacing="0">
  <tr>
    <th scope="col">Name</th>
    <th scope="col">Score</th>
  </tr>
  <tr> 
    <td>Peter</td>
    <td>19</td>
  </tr>
  <tr>
    <td>Parker</td>
    <td>62</td>
  </tr>
</table>
```

Gli assistenti vocali leggono:
&quot;Tabella con 2 colonne e 3 righe.&quot;

&quot;Nome, Peter. Punteggio, 19.&quot;

&quot;Nome, Parker. Punteggio 62.&quot;

+++

>[!TIP]
>
>Utilizza `role="presentation"` esclusivamente per le tabelle layout. Per le tabelle dati, mantenere la struttura semantica `<table>` in modo che gli assistenti vocali possano annunciare correttamente le intestazioni e le relazioni.

### Testo per i collegamenti {#links}

Gli assistenti vocali leggono i collegamenti utilizzando il testo. Se un collegamento è etichettato solo come &quot;Fai clic qui&quot; o &quot;Ulteriori informazioni&quot;, gli utenti delle tecnologie per l’accessibilità non conosceranno la destinazione. Per garantire l’accessibilità, è necessario un testo descrittivo che indichi chiaramente la destinazione o l’azione.

Utilizza E-mail Designer per aggiungere un collegamento al contenuto e modificare l’etichetta in modo che sia distinguibile (visibile) e descrittiva (chiaro in merito allo scopo). Evita etichette vaghe come &quot;qui&quot; o &quot;altro&quot;.

<!--![](assets/accessible-link.png){width="70%"}-->

+++Esempio - Collegamento valido (descrittivo): 

```
<p>Learn more in the  
<a href="https://adobe.com/release-notes">August release notes</a>. 
</p>
```

Gli assistenti vocali leggono:
&quot;Link, note sulla versione di agosto&quot;.

+++

+++Esempio: collegamento non valido (non descrittivo)

```
<p>Learn more about our new features.  
  <a href="https://adobe.com/release-notes">Click here</a>. 
</p>
```

Gli assistenti vocali leggono:
&quot;Link, fai clic qui.&quot; *(nessun contesto fuori ordine di lettura)*

+++

<!--for Landing Pages-->

<!--## Provide keyboard navigation and focus support {#keyboard}

Providing keyboard navigation and focus support allows people who cannot use a mouse to fully access and interact with content. It also improves overall usability by giving all users a clear and consistent way to move through information.

* Focus via keyboard
    * Ensure all interactive elements (such as buttons, checkboxes, links) have `tabindex="0"` so they are included in the natural tab order. 
    * Allow navigation using the Tab and arrow keys (↑ ↓ ← →), which should visibly highlight the focused element. 
* Custom focus styling 
    * Apply clear and distinguishable styles for focusing on actionable elements: 
        +++Example (CSS)

        ```
        [tabindex="0"] : focus { 
        outline: 2px solid #00AEEF;  /* Cyan border */ 
        background-color: #20CEFF;   /* Optional background */ 
        }
        ```
        
        +++

    * Ensure that focus indicators meet the WCAG 2.2 focus appearance standards, including: 
        * Minimum area: 2 CSS pixel thick outline.
        * Contrast ratio: ≥ 3:1 between focused and unfocused state. 

* Keyboard activation support 
    * Ensure checkboxes and buttons respond to the Enter and Space keys. 
    * Validate the interaction using the keyboard alone: 
        * Enter or Space should toggle checkboxes.
        * Enter or Space should trigger the buttons.-->
