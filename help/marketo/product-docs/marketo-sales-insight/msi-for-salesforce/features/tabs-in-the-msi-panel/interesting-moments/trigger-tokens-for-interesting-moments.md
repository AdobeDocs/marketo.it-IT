---
unique-page-id: 1146999
description: Token di attivazione per i momenti interessanti - Documenti Marketo - Documentazione del prodotto
title: Token di attivazione per i momenti interessanti
exl-id: 666a6eed-c432-4088-b4f1-54c996eca64c
translation-type: tm+mt
source-git-commit: 20a3bee9973340d7b772532d1be31fe745e5ffd7
workflow-type: tm+mt
source-wordcount: '437'
ht-degree: 0%

---

# Token di attivazione per i momenti interessanti {#trigger-tokens-for-interesting-moments}

>[!PREREQUISITES]
>
>Scopri come utilizzare il [passaggio Interessante del flusso di momenti](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md).

## Token disponibili {#available-tokens}

Consulta [Panoramica dei token](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) per vedere tutti i token che puoi inserire in un momento interessante.

## Token di attivazione {#trigger-tokens}

In base al trigger utilizzato in una campagna intelligente, sono disponibili ulteriori token trigger.

* `{{trigger.Trigger Name}}` che è sempre il trigger effettivo stesso. Ad esempio: Fai clic su Collega in E-mail.
* `{{trigger.Name}}` è il nome della risorsa che ha attivato la campagna. Ad esempio: Clic Link sulla pagina web è l’URL stesso, l’oggetto per i trigger Salesforce, ecc.
* Sono disponibili altri trigger basati sui vincoli elencati di seguito.

**Attivatori e-mail**

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col>
  <col>
  <col>
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th><br></th> 
   <th><code>{{trigger.Trigger Name}}</code></th> 
   <th><code>{{trigger.Name}}</code></th> 
   <th><code>{{trigger.Link}}</code></th> 
   <th><code>{{trigger.Subject}}</code></th> 
   <th><code>{{trigger.Category}}</code></th> 
   <th><code>{{trigger.Details}}</code></th> 
   <th><code>{{trigger.Web Page}}</code></th> 
   <th><code>{{trigger.Client IP Address}}</code></th> 
   <th><code>{{trigger.Sent By}}</code></th> 
   <th><code>{{trigger.Received By}}</code></th> 
   <th><code>{{trigger.Referrer}}</code></th>
   <th><code>{{trigger.Search Engine}}</code></th>
   <th><code>{{trigger.Search Query}}</code></th>
   <th><code>{{trigger.Browser}}</code></th>
  </tr> 
  <tr> 
   <td>Clic su Collega in e-mail</td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>E-mail rimbalzata dura</td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Soft rimbalzi e-mail</td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>E-Mail Consegnata</td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Apre e-mail</td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
    <tr> 
   <td>Inoltra a Amico e-mail ricevuto</td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
    <tr> 
   <td>Inviato a Amico e-mail</td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td>
  </tr> 
  <tr> 
   <td>Annulla l’abbonamento a un’e-mail</td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
 </tbody> 
</table>

**Trigger Salesforce**

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col>
  <col>
  <col>
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th><br></th> 
   <th><code>{{trigger.Trigger Name}}</code></th> 
   <th><code>{{trigger.Name}}</code></th> 
   <th><code>{{trigger.Link}}</code></th> 
   <th><code>{{trigger.Subject}}</code></th> 
   <th><code>{{trigger.Category}}</code></th> 
   <th><code>{{trigger.Details}}</code></th> 
   <th><code>{{trigger.Web Page}}</code></th> 
   <th><code>{{trigger.Client IP Address}}</code></th> 
   <th><code>{{trigger.Sent By}}</code></th> 
   <th><code>{{trigger.Received By}}</code></th> 
   <th><code>{{trigger.Referrer}}</code></th>
   <th><code>{{trigger.Search Engine}}</code></th>
   <th><code>{{trigger.Search Query}}</code></th>
   <th><code>{{trigger.Browser}}</code></th>
  </tr> 
  <tr> 
   <td>Clic Link nell'e-mail di vendita</td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Invia e-mail di vendita</td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Apre l'e-mail di vendita</td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Saldi e-mail di vendita</td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>E-mail di vendita ricevuta</td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
    <tr> 
   <td>Opportunità aggiornata</td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
    <tr> 
   <td>Modifiche al proprietario</td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>La persona viene convertita</td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>La persona viene cancellata dall'SFDC</td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Persona sincronizzata con SFDC</td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Rimosso dall'opportunità</td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Rimosso dalla campagna SFDC</td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>L’attività viene registrata</td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>L’attività è stata aggiornata</td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Aggiunto a Opportunità</td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Aggiunto alla campagna SFDC</td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Lo stato viene modificato nella campagna SFDC</td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
 </tbody> 
</table>

**Trigger di Sales Connect**

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col>
  <col>
  <col>
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th><br></th> 
   <th><code>{{trigger.Trigger Name}}</code></th> 
   <th><code>{{trigger.Name}}</code></th> 
   <th><code>{{trigger.Link}}</code></th> 
   <th><code>{{trigger.Subject}}</code></th> 
   <th><code>{{trigger.Category}}</code></th> 
   <th><code>{{trigger.Details}}</code></th> 
   <th><code>{{trigger.Web Page}}</code></th> 
   <th><code>{{trigger.Client IP Address}}</code></th> 
   <th><code>{{trigger.Sent By}}</code></th> 
   <th><code>{{trigger.Received By}}</code></th> 
   <th><code>{{trigger.Referrer}}</code></th>
   <th><code>{{trigger.Search Engine}}</code></th>
   <th><code>{{trigger.Search Query}}</code></th>
   <th><code>{{trigger.Browser}}</code></th>
  </tr> 
  <tr> 
   <td>Clic Link nell'e-mail di vendita</td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Invia e-mail di vendita</td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Apre l'e-mail di vendita</td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Saldi e-mail di vendita</td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>E-mail di vendita ricevuta</td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>È stato aggiunto alla campagna di vendita</td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr>
   <td>Modifiche al proprietario</td> 
   <td>È Rimosso Dalla Campagna Di Vendita</td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Chiamata alle vendite ricevute</td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
 </tbody> 
</table>

**Varie**

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col> 
  <col>
  <col>
  <col>
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th><br></th> 
   <th><code>{{trigger.Trigger Name}}</code></th> 
   <th><code>{{trigger.Name}}</code></th> 
   <th><code>{{trigger.Link}}</code></th> 
   <th><code>{{trigger.Subject}}</code></th> 
   <th><code>{{trigger.Category}}</code></th> 
   <th><code>{{trigger.Details}}</code></th> 
   <th><code>{{trigger.Web Page}}</code></th> 
   <th><code>{{trigger.Client IP Address}}</code></th> 
   <th><code>{{trigger.Sent By}}</code></th> 
   <th><code>{{trigger.Received By}}</code></th> 
   <th><code>{{trigger.Referrer}}</code></th>
   <th><code>{{trigger.Search Engine}}</code></th>
   <th><code>{{trigger.Search Query}}</code></th>
   <th><code>{{trigger.Browser}}</code></th>
  </tr> 
  <tr> 
   <td>Riempie il modulo</td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Pagina Web Visite</td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Clic sul link sulla pagina Web</td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(segno di spunta)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Se non ha un segno di spunta ![(tick)](assets/check.svg) restituirà una stringa vuota (niente) nel momento interessante.

*Il trigger **Visita pagina Web** dispone di alcuni token aggiuntivi:

* `{{trigger.Referrer}}`
* `{{trigger.Search Engine}}`
* `{{trigger.Search Query}}`

>[!TIP]
>
>Testa sempre i tuoi momenti interessanti per assicurarti che rendano il modo in cui intendi.
>
>Inoltre, assicurati che sia interessante per il Venditore, non solo per te. ![(rosa)](assets/wink.svg)>
