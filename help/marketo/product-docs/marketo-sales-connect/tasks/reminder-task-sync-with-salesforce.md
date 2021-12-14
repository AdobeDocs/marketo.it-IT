---
description: Sincronizzazione attività promemoria con Salesforce - Documenti Marketo - Documentazione del prodotto
title: Sincronizzazione attività promemoria con Salesforce
hide: true
hidefromtoc: true
exl-id: 4de933db-4626-4845-be70-8ad55d03a18e
source-git-commit: 87f43fb58b5739c0465a1a74fb60cdf5c5f6b759
workflow-type: tm+mt
source-wordcount: '501'
ht-degree: 0%

---

# Sincronizzazione attività promemoria con Salesforce {#reminder-task-sync-with-salesforce}

>[!NOTE]
>
>Per informazioni su come abilitare l’estrazione della sincronizzazione delle attività [Sincronizza attività di vendita/promemoria in attività Salesforce](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/salesforce-sync-settings.md#sync-sales-connect-tasks-reminders-to-salesforce-tasks).

Una volta abilitate le impostazioni di sincronizzazione delle attività, gli utenti vedranno le loro attività di promemoria bidirezionalmente sincronizzate con Salesforce. Ciò significa che gli utenti possono gestire le attività da Salesforce o Sales Connect e avere la certezza che i sistemi rimarranno allineati.

## Sincronizzazione campo attività promemoria {#reminder-task-field-sync}

![](assets/reminder-task-sync-with-salesforce-1.png)

Di seguito è riportato un elenco dei campi attività promemoria in Sales Connect e dei relativi campi Salesforce supportati tramite la sincronizzazione bidirezionale delle attività.

<table>
 <tr>
  <th>Campo attività Sales Connect</th>
  <th>Campo attività Salesforce</th>
  <th>Task Salesforce</th>
 </tr>
 <tr>
  <td>Nome attività</td>
  <td>Campo oggetto</td>
  <td>Breve campo di riepilogo inteso per mostrare il titolo dell’attività.</td>
 </tr>
 <tr>
  <td>Stato</td>
  <td>Stato attività</td>
  <td><p>Mostra lo stato dell'attività. Le attività di vendita Connect hanno due stati che vengono mappati su due valori nella lista di selezione dello stato dell'attività di Salesforce.</p>
  <p>Apri in Sales Connect = Non avviato in Salesforce.</p>
  <p>Completato in Sales Connect = Completato in Salesforce.</p>
  <p>Gli altri valori di stato in Salesforce non verranno sincronizzati con Sales Connect.</p></td>
 </tr>
 <tr>
  <td>Priorità</td>
  <td>Priorità</td>
  <td><p>La priorità di vendita Connect può essere Normale o Alta, che corrisponde ai valori di priorità Normale e Alta in Salesforce.</p>
  <p>Il valore a bassa priorità in Salesforce non verrà sincronizzato con Sales Connect.</p></td>
 </tr>
 <tr>
  <td>Data di scadenza</td>
  <td>Data di scadenza</td>
  <td>Data di scadenza dell'attività.</td>
 </tr>
 <tr>
  <td>Dettagli</td>
  <td>Commenti</td>
  <td>Mostra informazioni più dettagliate su cosa si intendeva completare con l’attività promemoria.</td>
 </tr>
</table>

## Sincronizzazione delle attività di vendita con Salesforce per la prima volta {#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

Quando attivi per la prima volta la sincronizzazione tra le attività di Sales Connect e Salesforce, importiamo le attività di Salesforce. Lo faremo **not** sovrascrivi tutte le attività correnti in Sales Connect to Salesforce. Per ridurre il disordine e i duplicati, le uniche attività che vengono sincronizzate da Sales Connect in Salesforce sono le attività create *dopo* è possibile sincronizzare Sales Connect con SFDC.

Ecco cosa succede quando si sincronizzano le attività di Sales Connect e SFDC:

* Non appena fai clic su salva nella sincronizzazione delle attività, queste iniziano a sincronizzarsi. Inizialmente ci vorrà un po&#39; di tempo.

* Eventuali promemoria aggiornati o creati nelle ultime 24 ore verranno inviati da SFDC a Sales Connect. La sincronizzazione è basata sulla data di scadenza e tutte le attività verranno sincronizzate sul back-end, ma in Command Center verranno visualizzate solo le attività scadute oggi e domani.

* Se la sincronizzazione è stata attivata in precedenza ed elimini eventuali attività in SFDC, tutto ciò che è stato eliminato negli ultimi 15 giorni verrà eliminato dal Centro comandi.

* Le attività verranno sincronizzate costantemente tra Sales Connect e SFDC purché la sincronizzazione sia abilitata.

Dopo la sincronizzazione iniziale, tutte le attività create, modificate, completate o eliminate in Sales Connect verranno sincronizzate nell&#39;elenco delle attività in Salesforce. E qualsiasi cosa creata, modificata, completata o eliminata in Salesforce aggiornerà l&#39;elenco delle attività in Sales Connect.

Per attivare questa sincronizzazione, controlla la casella di sincronizzazione nel tuo [Pagina Impostazioni](https://toutapp.com/login) nell&#39;applicazione web.
