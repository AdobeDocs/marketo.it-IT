---
unique-page-id: 1147114
description: Informazioni sui token in un programma - Documenti Marketo - Documentazione del prodotto
title: Informazioni sui token personali in un programma
exl-id: 01b42272-c419-4cd5-ad30-87413ceb2032
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# Informazioni sui token personali in un programma {#understanding-my-tokens-in-a-program}

Un token è una variabile che puoi utilizzare nelle e-mail, nelle pagine di destinazione e nelle campagne intelligenti per semplificare la tua vita.

Oltre ai token personali, puoi anche utilizzare uno qualsiasi dei token incorporati nei tuoi programmi. Consulta la [Panoramica dei token](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md).

## Token {#my-tokens} personali

I miei token sono variabili personalizzate che chiunque può creare. Vengono [creati](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md) nelle cartelle o nei programmi delle campagne.

I miei token vengono visualizzati in questo modo: `{{my.Name Of Token}}`

Esempi:

* `{{my.Event Date}}`
* `{{my.Webinar Speaker}}`

<table> 
 <thead> 
  <tr> 
   <th>Tipo di token</th> 
   <th>Descrizione</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>File di calendario <img alt="—" src="assets/image2014-9-25-16-3a44-3a19.png" data-linked-resource-id="3083230" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>Utilizza questo token per <a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/create-a-calendar-event-ics-file.md">aggiungere un file evento calendario (.i</a><a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/create-a-calendar-event-ics-file.md">cs)</a> alle e-mail e alle pagine di destinazione.</td> 
  </tr> 
  <tr> 
   <td><p>Data <img alt="—" src="assets/image2014-9-25-16-3a44-3a47.png" data-linked-resource-id="3083231" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></p></td> 
   <td>Questo token contiene un valore data. La data viene visualizzata come giorno/mese dell’anno (ad esempio, 2016-05-23).</td> 
  </tr> 
  <tr> 
   <td>Script e-mail <img alt="—" src="assets/image2014-9-25-16-3a45-3a4.png" data-linked-resource-id="3083232" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>Utilizza questo token per eseguire uno script Velocity nelle e-mail. Ulteriori informazioni <a href="https://developers.marketo.com/documentation/email-scripting/" title="Segui collegamento" rel="nofollow">qui</a>. </td> 
  </tr> 
  <tr> 
   <td>Numero<span> <img alt="—" src="assets/image2014-9-25-16-3a45-3a25.png" data-linked-resource-id="3083233" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></span></td> 
   <td>Qualsiasi numero intero. Può anche essere negativo.</td> 
  </tr> 
  <tr> 
   <td>Rich Text <img alt="—" src="assets/image2014-9-25-16-3a46-3a22.png" data-linked-resource-id="3083234" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>Questo è HTML. Utilizzalo nelle e-mail e nelle pagine di destinazione.</td> 
  </tr> 
  <tr> 
   <td>Punteggio <img alt="—" src="assets/image2014-9-25-16-3a46-3a39.png" data-linked-resource-id="3083235" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>Utilizza questo token nel <a href="/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md">passaggio di flusso del punteggio di modifica</a>. </td> 
  </tr> 
  <tr> 
   <td colspan="1">Campagna SFDC <img alt="—" src="assets/sfdc-campaign-icon.jpg" data-linked-resource-id="11379761" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114" title="—"></td> 
   <td colspan="1">Utilizza questo token per consentire l’aggiunta di lead che diventano parte di un programma Marketo a qualsiasi campagna SFDC.</td> 
  </tr> 
  <tr> 
   <td>Testo <img alt="—" src="assets/image2014-9-25-16-3a46-3a54.png" data-linked-resource-id="3083236" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>Solo un po' di testo. Usarlo quando l'HTML è troppo costoso. Il limite di dimensione per i token di testo è di 524.288 caratteri (UTF-8) o 2 MB.</td> 
  </tr> 
 </tbody> 
</table>

>[!CAUTION]
>
>I miei token non verranno risolti quando invii un’e-mail da Sales Insight in Microsoft Dynamics o Salesforce; verranno compilati solo i token standard (Lead, Azienda, ecc.). Tuttavia, i valori predefiniti per i token _funzioneranno_.

## Nidificazione dei token {#nesting-tokens}

Quando si crea un nuovo token, è possibile farvi riferimento da altri oggetti nella struttura. Esiste una struttura di denominazione per la creazione del token per una gestione semplice.

* **Token locale:** il token è stato creato direttamente nel programma o nella cartella.
* **Token ereditato:** il token è stato creato nella struttura in un punto qualsiasi di un programma o cartella di livello superiore.
* **Token ignorato:** il token è stato ereditato e quindi un utente ha fatto un&#39;eccezione in questo programma o cartella.

È possibile creare variabili globali e quindi sostituirle ai livelli inferiori nella struttura.

Lo spostamento di programmi e cartelle influisce anche sui token. Controlla sempre se i riferimenti non sono interrotti durante lo spostamento.

>[!NOTE]
>
>Se l’e-mail inviata da un programma di coinvolgimento è un’e-mail figlia di un programma predefinito (non locale per il programma di coinvolgimento), tutti i token utente utilizzati nell’e-mail vengono risolti dal programma predefinito in cui risiede l’e-mail figlio.

>[!MORELIKETHIS]
>
>* [Panoramica dei token](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md)
>* [Gestione dei token personali](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md)

