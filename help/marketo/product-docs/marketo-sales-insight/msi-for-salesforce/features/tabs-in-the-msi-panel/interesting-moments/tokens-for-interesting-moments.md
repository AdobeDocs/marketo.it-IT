---
unique-page-id: 1146999
description: Token per momenti interessanti - Documenti Marketo - Documentazione prodotto
title: Token per momenti interessanti
translation-type: tm+mt
source-git-commit: 972cf9769ac751d9abfd5665975703dcd07930f0
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---


# Token per momenti interessanti {#tokens-for-interesting-moments}

>[!PREREQUISITES]
>
>Scopri come utilizzare il passaggio [Interessante Flusso di Momenti](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md).

## Token disponibili {#available-tokens}

Controlla [Tokens Overview](/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/tokens-overview.md) per vedere tutti i token che puoi inserire in un momento interessante.

## Token trigger {#trigger-tokens}

In base all&#39;attivatore utilizzato in una campagna intelligente, sono disponibili altri Token trigger.

* `{{trigger.Trigger Name}}` che è sempre il trigger effettivo stesso. Ad esempio: Fate clic su Collega in E-mail.
* `{{trigger.Name}}` è il nome della risorsa che ha attivato la campagna. Ad esempio: Fate clic su Collega nella pagina Web è l’URL stesso, l’oggetto per le attivazioni Salesforce, ecc.
* Ulteriori attivatori sono disponibili in base ai vincoli elencati di seguito:

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
  </tr> 
  <tr> 
   <td>Fate clic su Collega nell’e-mail</td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
  </tr> 
  <tr> 
   <td>Punti e-mail rigidi</td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
  </tr> 
  <tr> 
   <td>Soft punteggi e-mail</td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
  </tr> 
  <tr> 
   <td>E-mail inviata</td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
  </tr> 
  <tr> 
   <td>Apre E-Mail</td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
  </tr> 
  <tr> 
   <td>Annulla sottoscrizione da e-mail</td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><br></td> 
   <td><br></td> 
  </tr> 
  <tr> 
   <td>Fai clic su Collega nell'e-mail di vendita</td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><br></td> 
  </tr> 
  <tr> 
   <td>E-mail di vendita inviata</td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><br></td> 
  </tr> 
  <tr> 
   <td>Apre l'e-mail di vendita</td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><br></td> 
  </tr> 
  <tr> 
   <td>E-mail di vendita ricevuta</td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
  </tr> 
  <tr> 
   <td colspan="1">Messaggio e-mail di vendita troncato</td> 
   <td colspan="1"><img src="assets/check.svg" alt="(tick)"></td> 
   <td colspan="1"><img src="assets/check.svg" alt="(tick)"></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
  </tr> 
  <tr> 
   <td>Compilazione modulo</td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><br></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><img src="assets/check.svg" alt="(tick)"></td> 
   <td><br></td> 
   <td><p><br></p></td> 
  </tr> 
  <tr> 
   <td colspan="1">Visita pagina Web*</td> 
   <td colspan="1"><img src="assets/check.svg" alt="(tick)"></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><img src="assets/check.svg" alt="(tick)"></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
   <td colspan="1"><br></td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Se non ha un segno di spunta ![(tick)](assets/check.svg), nel momento interessante restituirà una stringa vuota (niente).

*L&#39;attivatore **Visita pagina Web** dispone di alcuni token aggiuntivi:

* `{{trigger.Referrer}}`
* `{{trigger.Search Engine}}`
* `{{trigger.Search Query}}`

>[!TIP]
>
>Prova sempre i tuoi momenti interessanti per assicurarti che siano il modo in cui intendi.
>
>Inoltre, accertati che sia interessante per il Sales Person, non solo per te. ![(wink)](assets/wink.svg)>
