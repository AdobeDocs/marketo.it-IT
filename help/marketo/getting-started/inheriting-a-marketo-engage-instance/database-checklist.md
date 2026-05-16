---
description: Elenco di controllo del database delle istanze ereditate - Documentazione di Marketo - Documentazione del prodotto
title: Elenco di controllo del database delle istanze ereditate
feature: Getting Started
exl-id: 278a6a2f-7b68-4003-8727-129e0dc96c12
TQID: https://experienceleague.adobe.com/ssiWj0vQTwU1qBD5fyZ8VHz7RmFjaVxu1dj7J8G-P5U
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: c5f60233-d5ea-4453-a799-0ad258b4d399id: d65b4a73-87a3-4d56-b638-74e74d9939ceid: e64968b2-4ee5-47f9-8cae-0588f184b9ebid: ed6be6bb-75bb-4ea9-9a42-3bcaa65e1bcc
subfeature_v2: id: a1d50dda-6d94-4e16-8c30-5eb7181c4650id: df8eb12b-4f82-491f-acbb-d74012ca5654
topic_v2: id: e0eb8757-182f-49f3-94a4-1587d16f5094id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 423
ht-degree: 7%

---

# Istanza ereditata: elenco di controllo del database {#inherited-instance-database-checklist}

Comprendi il numero totale di persone, persone commerciabili e principali sorgenti di acquisizione persone nel tuo abbonamento. Ricordati di [scaricare le liste di controllo](/help/marketo/getting-started/inheriting-a-marketo-engage-instance/assets/adobe-marketo-engage-inherited-instance-admin-checklist.xlsx) e tenere traccia dell&#39;avanzamento.

## Elenchi smart di sistema {#system-smart-lists}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">Area</th>
   <th>Rivedi focus</th>
  </tr>
  <tr>
   <td>Tutte le persone</td>
   <td><li>Quante persone esistono nel <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/database-dashboard.md" target="_blank">database</a>?</li>
<li>Se il database è quasi pieno, i criteri aziendali consigliano di espandere le dimensioni del database o di eliminare i dati storici?</li>
<li>Il database complessivo è commerciabile almeno all'85%?
<br/> Se il tuo rientra in questa soglia, controlla con maggiore attenzione gli altri elenchi avanzati del sistema (ad Elenco Bloccati, Marketing Sospeso, Duplicati, Annulla iscrizione).</li></td>
  </tr>
  <tr>
   <td>Persone con iscrizione annullata</td>
   <td><li>Quali sono i criteri per <a href="/help/marketo/product-docs/email-marketing/deliverability/understanding-unsubscribe.md#marketing-suspended" target="_blank">utenti non iscritti</a>? Ci sono troppe persone non iscritte?</li>
<li>I metodi di annullamento dell’abbonamento sono in linea con i requisiti sulla privacy dei dati?</li>
<li>La tua preferenza per annullare l’abbonamento è aggiornata? Per quanto tempo i record sono rimasti nel database come non commerciabili?</li></td>
  </tr>
  <tr>
   <td>Marketing sospeso</td>
   <td><li>Quali sono i criteri per <a href="/help/marketo/product-docs/email-marketing/deliverability/durable-unsubscribe.md#marketing-suspended" target="_blank">Marketing sospeso</a>? Ci sono troppe persone che sono sospese dal marketing?</li>
<li>Per quanto tempo i documenti sono rimasti nello stato Marketing Sospeso?</li>
<p>Esempio di caso d’uso Marketing Suspended: record di persone attivamente coinvolte nelle vendite in opportunità in fase avanzata per le quali desideri eliminare le comunicazioni di marketing.</td>
  </tr>
   <tr>
   <td>Elenco Bloccati</td>
   <td><li>Quali sono i criteri per <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/add-person-to-blocklist.md" target="_blank">la inserisce nell'elenco Bloccati dei record</a>? Ci sono troppe persone che sono?</li></td>
  </tr>
  <tr>
   <td>Indirizzi e-mail con mancato recapito</td>
   <td><li>Ci sono molte <a href="/help/marketo/product-docs/email-marketing/deliverability/hard-and-soft-bounces-in-email.md" target="_blank">persone che hanno rimbalzato</a> nel tuo database?
   <br/> In caso affermativo, valutare il motivo.</li></td></li></td>
  </tr>
  <tr>
   <td>Possibili duplicati</td>
   <td><li>Quanti <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/managing-people-in-smart-lists/find-and-merge-duplicate-people.md" target="_blank">record potenzialmente duplicati</a> sono presenti?
   <br/> Eliminarli o unirli.</li></td>
  </tr>
   <tr>
   <td>Nessun programma di acquisizione</td>
   <td><li>Quante persone non dispongono di un <a href="/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-program-membership.md#acquisition-program" target="_blank">programma di acquisizione</a>?
   <br/> Se ce ne sono molti, prova a scoprirne il motivo.</li></td>
  </tr>
 </tbody>
</table>

## Elenchi avanzati {#smart-lists}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">Area</th>
   <th>Rivedi focus</th>
  </tr>
  <tr>
   <td>Elenchi avanzati</td>
   <td><li>Quanti <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/understanding-smart-lists.md" target="_blank">elenchi avanzati</a> sono presenti? Come vengono utilizzati in questa istanza?</li>
   <p><img src="assets/note-icon.png" alt="icona nota"> NOTA: nella sezione Database, gli elenchi smart di gruppo sono generati dall'utente e gli elenchi smart di sistema sono elenchi predefiniti creati da Marketo Engage.
<li>Gli elenchi sono organizzati in una struttura di cartelle coesa?
<br/> Se disponi di elenchi orfani, puoi organizzare la struttura in modo che le risorse siano facili da trovare.</li>
<p><img src="assets/tip-icon.png" alt="icona di suggerimento">SUGGERIMENTO: <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-folders.md#archive-a-folder" target="_blank">Archiviazione</a> degli elenchi avanzati non più necessari per migliorare l'organizzazione e le prestazioni.</td>
  </tr>
 </tbody>
</table>

## Elenchi statici {#static-lists}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">Area</th>
   <th>Rivedi focus</th>
  </tr>
  <tr>
   <td>Elenchi statici</td>
   <td><li>Quanti <a href="/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/understanding-static-lists.md" target="_blank">Elenchi statici</a> sono presenti? Come vengono utilizzati in questa istanza?</li>
   <p><img src="assets/note-icon.png" alt="icona nota"> NOTA: nella sezione Database gli elenchi di gruppi sono elenchi statici.</td>
  </tr>
 </tbody>
</table>

## Segmentazioni {#segmentations}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">Area</th>
   <th>Rivedi focus</th>
  </tr>
  <tr>
   <td>Segmentazioni</td>
   <td><li>Quali <a href="/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md" target="_blank">segmentazioni</a> sono presenti? Come vengono utilizzati?</li>
<li>Troppe persone in <a href="/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/segmentation-order-priority.md" target="_blank">segmenti predefiniti</a>?</li>
<li>Esiste una segmentazione per il pubblico commerciabile?
<br/> In caso contrario, provare a crearne uno.</li></td>
  </tr>
 </tbody>
</table>
