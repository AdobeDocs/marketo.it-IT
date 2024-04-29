---
description: Impostare la sezione Database per la nuova istanza di Marketo Engage.
title: Best practice per le nuove istanze - Elenco di controllo del database
hide: true
hidefromtoc: true
feature: Getting Started
source-git-commit: 47446db902f85e1b4a910d0924efc5beb82bffbe
workflow-type: tm+mt
source-wordcount: '302'
ht-degree: 2%

---

# Best practice per le nuove istanze: elenco di controllo del database {#new-instance-best-practices-database-checklist}

La sezione Database fornisce un’istantanea degli attributi chiave relativi alle persone nell’istanza. Scopri i passaggi necessari per spostarti tra i diversi elenchi e segmentazioni nel tuo database e come gestire i record di persone.

Ricordati di scaricare le liste di controllo [LINK] e tieni traccia dei tuoi progressi.

## Elenchi smart di sistema {#system-smart-lists}

<table>
<thead>
  <tr>
    <th style="width:20%">Area</th>
    <th style="width:80%">Elementi azione</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Tutte le persone</td>
    <td><li>Determina come implementare una sincronizzazione 1:1 con il tuo sistema CRM o come applicare i filtri per limitare chi si sposta da un sistema all’altro e quando.</li> 
    <li>Rivedi il numero totale di persone e persone commerciabili nel tuo <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/database-dashboard.html" target="_blank">database di Marketo Engage</a>.</li></td>
  </tr>
  <tr>
    <td>INSERISCO NELL'ELENCO BLOCCATI DI</td>
    <td><li>Definisci i criteri di inserisce nell'elenco Bloccati dei. Valuta l’aggiunta di domini della concorrenza al <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.html" target="_blank">INSERISCO NELL'ELENCO BLOCCATI DI</a> per evitare che ricevano le e-mail.</li></td>
  </tr>
  <tr>
    <td>Marketing sospeso</td>
    <td><li>Definisci <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/understanding-unsubscribe.html#marketing-suspended" target="_blank">Marketing sospeso</a> criteri.</li></td>
  </tr>
  <tr>
    <td>Indirizzi e-mail non recapitati </td>
    <td><li>Definisci i criteri per gli indirizzi e-mail non recapitati.</li>
    <li>Rivedi le persone nella categoria E-mail non valida e se le e-mail devono essere <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/hard-and-soft-bounces-in-email.html" target="_blank">ripristina manualmente</a>.</li></td>
  </tr>
  <tr>
    <td>Possibili duplicati</td>
    <td><li>Rivedi Persone nell’elenco Possibili duplicati.</li> 
    <li>Definire la strategia di gestione dei duplicati per determinare se si desidera <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.html" target="_blank">unisci persone manualmente</a>.</li>  
    <li>Se disponi di un’integrazione CRM, definisci un processo e un account per <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.html#effect-in-salesforce" target="_blank">l’effetto dell’unione di lead nel CRM</a>.</li></td>
  </tr>
  <tr>
    <td>Nessun programma di acquisizione</td>
    <td><li>Stabilisci campagne nei modelli di programma che impostano un programma di acquisizione, soprattutto se utilizzi moduli globali.</li></td>
  </tr>
  <tr>
    <td>Persone non abbonate</td>
    <td><li>Rivedi i criteri per <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/understanding-unsubscribe.html" target="_blank">Persone non abbonate</a>.</li></td>
  </tr>
</tbody>
</table>

## Raggruppa elenchi avanzati {#group-smart-lists}

<table>
<thead>
  <tr>
    <th style="width:20%">Area</th>
    <th style="width:80%">Elementi azione</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Raggruppa elenchi avanzati</td>
    <td><li>Presta attenzione alla creazione di elenchi avanzati di gruppo in modo che non siano presenti elenchi duplicati.</li>
    <li>Tenere traccia degli elenchi principali nel database.</li></td>
  </tr>
</tbody>
</table>

## Segmentazione {#segmentation}

<table>
<thead>
  <tr>
    <th style="width:20%">Area</th>
    <th style="width:80%">Elementi azione</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Segmentazione</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.html" target="_blank">Creare segmentazioni</a> in base alle esigenze aziendali. Ogni abbonamento è limitato a 20 segmentazioni e 100 segmenti all’interno di ogni segmentazione.</li></td>
  </tr>
</tbody>
</table>
