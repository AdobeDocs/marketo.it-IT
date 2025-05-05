---
unique-page-id: 1147114
description: Informazioni sui token in un programma - Documentazione di Marketo - Documentazione del prodotto
title: Informazioni sui token in un programma
exl-id: 01b42272-c419-4cd5-ad30-87413ceb2032
feature: Tokens
source-git-commit: f21d9356f00f8ea50819b591d15ca06d61256d8b
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 1%

---

# Informazioni sui token in un programma {#understanding-my-tokens-in-a-program}

Un token è una variabile che puoi utilizzare nelle e-mail, nelle pagine di destinazione e nelle campagne avanzate per semplificare la tua vita.

Oltre a I miei token, nei programmi puoi utilizzare anche qualsiasi token incorporato. Controlla la [panoramica dei token](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md){target="_blank"}.

## I miei token  {#my-tokens}

I miei token sono variabili personalizzate che chiunque può creare. Localmente, sono [create](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md){target="_blank"} nelle cartelle o nei programmi della campagna.

I miei token sono visualizzati così: `{{my.Name Of Token}}`

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
   <td>Usa questo token per <a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/create-a-calendar-event-ics-file.md">aggiungere un file evento calendario (.i</a><a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/create-a-calendar-event-ics-file.md">cs)</a> alle e-mail e alle pagine di destinazione.</td> 
  </tr> 
  <tr> 
   <td><p>Data <img alt="--" src="assets/image2014-9-25-16-3a44-3a47.png" data-linked-resource-id="3083231" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></p></td> 
   <td>Questo token contiene un valore di data. La data viene visualizzata come anno-mese-giorno (ad esempio, 2016-05-23).</td> 
  </tr> 
  <tr> 
   <td>Script e-mail <img alt="--" src="assets/image2014-9-25-16-3a45-3a4.png" data-linked-resource-id="3083232" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>Utilizza questo token per eseguire uno script Velocity nelle e-mail. Ulteriori informazioni <a href="https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/email-scripting" title="Segui collegamento" rel="nofollow">qui</a>. </td> 
  </tr> 
  <tr> 
   <td>Numero <span> <img alt="--" src="assets/image2014-9-25-16-3a45-3a25.png" data-linked-resource-id="3083233" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></span></td> 
   <td>Qualsiasi numero intero. Può anche essere negativo.</td> 
  </tr> 
  <tr> 
   <td>Rich Text <img alt="--" src="assets/image2014-9-25-16-3a46-3a22.png" data-linked-resource-id="3083234" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>Questo è HTML. Utilizzalo nelle e-mail e nelle pagine di destinazione.</td> 
  </tr> 
  <tr> 
   <td>Punteggio <img alt="--" src="assets/image2014-9-25-16-3a46-3a39.png" data-linked-resource-id="3083235" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>Usa questo token nel <a href="/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md">passaggio del flusso del punteggio di modifica</a>. </td> 
  </tr> 
  <tr> 
   <td colspan="1">SFDC Campaign <img alt="--" src="assets/sfdc-campaign-icon.jpg" data-linked-resource-id="11379761" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114" title="--"></td> 
   <td colspan="1">Utilizza questo token per consentire ai lead che entrano a far parte di un programma Marketo di essere aggiunti anche a qualsiasi campagna SFDC venga aggiunta.</td> 
  </tr> 
  <tr> 
   <td>Testo <img alt="--" src="assets/image2014-9-25-16-3a46-3a54.png" data-linked-resource-id="3083236" data-linked-resource-type="attachment" data-base-url="https://docs.marketo.com" data-linked-resource-container-id="1147114"></td> 
   <td>Solo un testo. Utilizzalo quando HTML è sovraccarico. Il limite di dimensione per i token di testo è di 524.288 caratteri (UTF-8) o 2 MB.</td> 
  </tr> 
 </tbody> 
</table>

>[!CAUTION]
>
>I miei token non vengono risolti quando invii un’e-mail da Sales Insight su Microsoft Dynamics o Salesforce; verranno compilati solo i token standard (lead, società, ecc.). I valori predefiniti per i token _funzioneranno_.

## Nidificazione dei token {#nesting-tokens}

Quando crei un nuovo token, altri oggetti nella struttura possono farvi riferimento. Esiste una struttura di denominazione per la posizione in cui il token è stato creato per una gestione semplice.

* **Token locale:** Il token è stato creato direttamente in tale programma o cartella.
* **Token ereditato:** Il token è stato creato nella struttura in un programma o in una cartella di livello superiore.
* **Token ignorato:** Il token è stato ereditato e quindi un utente ha fatto un&#39;eccezione in questo programma o cartella.

Puoi creare variabili globali e quindi sostituirle ai livelli più bassi nella struttura.

Lo spostamento di programmi e cartelle influisce anche sui token. Verificare sempre che i riferimenti non siano interrotti durante lo spostamento.

>[!NOTE]
>
>Se l’e-mail inviata da un programma di coinvolgimento è un’e-mail figlio di un programma predefinito (non locale al programma di coinvolgimento), tutti i Token personali utilizzati nell’e-mail vengono risolti dal programma predefinito in cui si trova l’e-mail figlio.

>[!MORELIKETHIS]
>
>* [Panoramica dei token](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md){target="_blank"}
>* [Gestione dei token](/help/marketo/product-docs/core-marketo-concepts/programs/tokens/managing-my-tokens.md){target="_blank"}
