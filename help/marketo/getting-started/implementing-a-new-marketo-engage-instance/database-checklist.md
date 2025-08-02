---
description: Imposta la sezione Database per la nuova istanza di Marketo Engage.
title: Best practice per le nuove istanze - Elenco di controllo del database
feature: Getting Started
exl-id: 996ea2db-a00c-48e5-97a8-00f869c261b1
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 2%

---

# Best practice per le nuove istanze: elenco di controllo del database {#new-instance-best-practices-database-checklist}

Nella sezione Database sono disponibili gli attributi chiave delle persone presenti nell&#39;istanza. Scopri i passaggi necessari per spostarti tra i diversi elenchi e segmentazioni nel tuo database e come gestire i record di persone.

Ricordati di [scaricare le liste di controllo](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx) e tenere traccia dell&#39;avanzamento.

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
    <li>Esaminare il numero totale di persone e persone commerciabili nel <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/database-dashboard.html?lang=it" target="_blank">database Marketo Engage</a>.</li></td>
  </tr>
  <tr>
    <td>INSERISCO NELL'ELENCO BLOCCATI DI</td>
    <td><li>Definisci i criteri di inserisce nell'elenco Bloccati dei. Prendi in considerazione l'aggiunta dei domini della concorrenza al tuo <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.html?lang=it" target="_blank">inserisco nell'elenco Bloccati di</a> per impedire loro di ricevere le tue e-mail.</li></td>
  </tr>
  <tr>
    <td>Marketing sospeso</td>
    <td><li>Definisci i criteri di <a href="https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/email-marketing/deliverability/understanding-unsubscribe#marketing-suspended" target="_blank">Marketing sospeso</a>.</li></td>
  </tr>
  <tr>
    <td>Indirizzi e-mail non recapitati </td>
    <td><li>Definisci i criteri per gli indirizzi e-mail non recapitati.</li>
    <li>Rivedi le persone nella categoria "E-mail non valida" e determina se le e-mail devono essere <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/hard-and-soft-bounces-in-email.html?lang=it" target="_blank">reimpostate manualmente</a>.</li></td>
  </tr>
  <tr>
    <td>Possibili duplicati</td>
    <td><li>Rivedi Persone nell’elenco Possibili duplicati.</li>
    <li>Definisci la strategia di gestione dei duplicati per determinare se <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.html?lang=it" target="_blank">unire manualmente le persone</a>.</li>
    <li>Se hai un'integrazione CRM, definisci un processo e un account per <a href="https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people#effect-in-salesforce" target="_blank">l'effetto dell'unione di lead nel CRM</a>.</li></td>
  </tr>
  <tr>
    <td>Nessun programma di acquisizione</td>
    <td><li>Stabilisci campagne nei modelli di programma che impostano un programma di acquisizione, soprattutto se utilizzi moduli globali.</li></td>
  </tr>
  <tr>
    <td>Persone non abbonate</td>
    <td><li>Rivedi i criteri per <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/understanding-unsubscribe.html?lang=it" target="_blank">Utenti non iscritti</a>.</li></td>
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
    <th style="width:21%">Area</th>
    <th style="width:79%">Elementi azione</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Segmentazione</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.html?lang=it" target="_blank">Crea segmentazioni</a> in base alle tue esigenze aziendali. Ogni abbonamento è limitato a 20 segmentazioni e 100 segmenti all’interno di ogni segmentazione.</li></td>
  </tr>
</tbody>
</table>
