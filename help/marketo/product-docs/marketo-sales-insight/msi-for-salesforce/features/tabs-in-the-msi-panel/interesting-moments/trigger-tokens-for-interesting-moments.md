---
unique-page-id: 1146999
description: Token di attivazione per i momenti di interesse - Documentazione di Marketo - Documentazione del prodotto
title: Attiva token per momenti di interesse
exl-id: 666a6eed-c432-4088-b4f1-54c996eca64c
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 0%

---

# Attiva token per momenti di interesse {#trigger-tokens-for-interesting-moments}

>[!PREREQUISITES]
>
>Scopri come utilizzare la [Passaggio flusso momento di interesse](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md).

## Token disponibili {#available-tokens}

Estrai [Panoramica dei token](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) per vedere tutti i token si può mettere in un momento interessante.

## Attiva token {#trigger-tokens}

In base al trigger utilizzato in una campagna intelligente, sono disponibili token di trigger aggiuntivi.

* `{{trigger.Trigger Name}}` che è sempre il trigger effettivo. Ad esempio: fa clic su Collega nell’e-mail.
* `{{trigger.Name}}` è il nome della risorsa che ha attivato la campagna. Ad esempio: Collegamento clic sulla pagina web è l’URL stesso, oggetto per i trigger Salesforce, ecc.
* Sono disponibili trigger aggiuntivi in base ai vincoli elencati di seguito.

**Trigger e-mail**

<table style="table-layout:auto"> 
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
   <td>Clic sul collegamento nell’e-mail</td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
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
   <td>Notifica di mancato recapito e-mail grave</td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
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
   <td>Mancato recapito e-mail non permanenti</td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
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
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
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
   <td>Apre l’e-mail</td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
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
   <td>Ricevuto Inoltra a e-mail amico</td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
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
   <td>Inoltro a e-mail amico</td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="spunta"></td>
  </tr> 
  <tr> 
   <td>Annulla iscrizione all’e-mail</td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
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

<table style="table-layout:auto"> 
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
   <td>Clic sul collegamento nell’e-mail di vendita</td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>E-Mail Di Vendita Inviata</td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Apre l'e-mail di vendita</td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>E-mail di vendita non recapitate</td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
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
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><br></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
    <tr> 
   <td>L’opportunità è aggiornata</td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
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
   <td>Modifiche proprietario</td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
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
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
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
   <td>Persona eliminata da SFDC</td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
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
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
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
   <td>Rimosso dall’opportunità</td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
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
   <td>Rimosso da Campagna SFDC</td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
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
   <td>Attività registrata</td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
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
   <td>L'attività è aggiornata</td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
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
   <td>Aggiunto all’opportunità</td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
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
   <td>Aggiunta a Campagna SFDC</td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
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
   <td>Stato modificato nella campagna SFDC</td> 
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

**Trigger Sales Connect**

<table style="table-layout:auto"> 
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
   <td>Clic sul collegamento nell’e-mail di vendita</td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>E-Mail Di Vendita Inviata</td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Apre l'e-mail di vendita</td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>E-mail di vendita non recapitate</td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
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
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><br></td>
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Aggiunto alla campagna di vendita</td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
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
   <td>Modifiche proprietario</td> 
   <td>Viene Rimosso Dalla Campagna Di Vendita</td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
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
   <td>Chiamata di vendita ricevuta</td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
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

<table style="table-layout:auto"> 
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
   <td>Compila modulo</td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Pagina Web Visite</td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><br></td>
  </tr> 
  <tr> 
   <td>Clic sul collegamento sulla pagina web</td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.png" alt="spunta"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td>
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Se non ha un assegno ![(segno di spunta)](assets/check.png) quindi restituirebbe una stringa vuota (niente) nel momento interessante.

&#42;Il trigger **Pagina Web Visite** dispone di alcuni token aggiuntivi:

* `{{trigger.Referrer}}`
* `{{trigger.Search Engine}}`
* `{{trigger.Search Query}}`

>[!TIP]
>
>Metti sempre alla prova i tuoi momenti interessanti per assicurarti che vengano riprodotti nel modo in cui desideri.
>
>Inoltre, assicurati che sia interessante per il venditore, non solo per te!
