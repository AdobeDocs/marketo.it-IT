---
description: Sincronizzazione attività promemoria con Salesforce - Documenti Marketo - Documentazione del prodotto
title: Sincronizzazione attività promemoria con Salesforce
exl-id: 4de933db-4626-4845-be70-8ad55d03a18e
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 0%

---

# Sincronizzazione attività promemoria con Salesforce {#reminder-task-sync-with-salesforce}

>[!NOTE]
>
>Per informazioni su come attivare l&#39;estrazione di Sincronizzazione attività [Sincronizza attività/promemoria vendite con attività Salesforce](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/salesforce-sync-settings.md#sync-sales-connect-tasks-reminders-to-salesforce-tasks).

Una volta abilitate le impostazioni di sincronizzazione delle attività, gli utenti vedranno le loro attività promemoria sincronizzate bidirezionalmente con Salesforce. In questo modo gli utenti possono gestire le attività da Salesforce o Sales Connect e avere la certezza che i sistemi rimarranno allineati.

## Sincronizzazione campi attività promemoria {#reminder-task-field-sync}

![](assets/reminder-task-sync-with-salesforce-1.png)

Di seguito è riportato un elenco dei campi delle attività promemoria in Sales Connect e dei corrispondenti campi Salesforce supportati tramite la sincronizzazione bidirezionale delle attività.

<table>
 <tr>
  <th>Campo attività Sales Connect</th>
  <th>Campo attività Salesforce</th>
  <th>Attività Salesforce</th>
 </tr>
 <tr>
  <td>Nome attività</td>
  <td>Campo oggetto</td>
  <td>Un breve campo di riepilogo destinato a mostrare il titolo dell’attività.</td>
 </tr>
 <tr>
  <td>Stato</td>
  <td>Stato attività</td>
  <td><p>Mostra lo stato dell'attività. Le attività Sales Connect hanno due stati che corrispondono a due dei valori nella lista di selezione dello stato delle attività Salesforce.</p>
  <p>Apri in connessione vendite = Non avviato in Salesforce.</p>
  <p>Completato in Sales Connect = Completato in Salesforce.</p>
  <p>Gli altri valori di stato in Salesforce non verranno sincronizzati con Sales Connect.</p></td>
 </tr>
 <tr>
  <td>Priorità</td>
  <td>Priorità</td>
  <td><p>La priorità Sales Connect può essere Normal (Normale) o High (Alta), che corrisponde ai valori di priorità Normal (Normale) e High (Alta) in Salesforce.</p>
  <p>Il valore di priorità bassa in Salesforce non verrà sincronizzato con Sales Connect.</p></td>
 </tr>
 <tr>
  <td>Data di scadenza</td>
  <td>Data di scadenza</td>
  <td>Data di scadenza dell'attività.</td>
 </tr>
 <tr>
  <td>Dettagli</td>
  <td>Commenti</td>
  <td>Mostra informazioni più dettagliate su ciò che doveva essere completato con l'attività promemoria.</td>
 </tr>
</table>

## Sincronizzazione per la prima volta delle attività Sales Connect con Salesforce {#syncing-sales-connect-tasks-with-salesforce-for-the-first-time}

Quando attivi per la prima volta la sincronizzazione tra le attività Sales Connect e Salesforce, le attività Salesforce vengono importate. Lo faremo **non** eseguire il push di tutte le attività correnti disponibili in Sales Connect a Salesforce. Per ridurre il disordine e i duplicati, le uniche attività sincronizzate da Sales Connect a Salesforce sono le attività create *dopo* sincronizzi Sales Connect con SFDC.

Ecco cosa accade quando si sincronizzano le attività Sales Connect e SFDC:

* Non appena si fa clic su Salva durante la sincronizzazione delle attività, queste vengono sincronizzate. Inizialmente questo richiederà del tempo.

* Tutti i promemoria aggiornati o creati nelle ultime 24 ore verranno inseriti da SFDC a Sales Connect. La sincronizzazione è basata sulla data di scadenza e tutte queste attività verranno sincronizzate nel back-end, ma in Centro comandi verranno visualizzate solo le attività in scadenza oggi e domani.

* Se la sincronizzazione è stata attivata in precedenza ed è stata eliminata qualsiasi attività in SFDC, qualsiasi elemento eliminato negli ultimi 15 giorni verrà eliminato da Centro comandi.

* Sincronizzeremo costantemente le attività tra Sales Connect e SFDC, purché la sincronizzazione sia abilitata.

Dopo la sincronizzazione iniziale, tutte le attività create, modificate, completate o eliminate in Sales Connect verranno sincronizzate con l&#39;elenco delle attività in Salesforce. E tutto ciò che viene creato, modificato, completato o eliminato in Salesforce aggiorna l&#39;elenco delle attività in Sales Connect.

Per attivare questa sincronizzazione, seleziona la casella di sincronizzazione nel [Pagina Impostazioni](https://toutapp.com/login) nell’applicazione web.

>[!NOTE]
>
>Il campo oggetto di un&#39;attività può essere aggiornato in Sales Connect e tale aggiornamento verrà sincronizzato nel campo oggetto Salesforce per l&#39;attività sincronizzata corrispondente, se si utilizza `{{activity_subject}}` campo dinamico nel tuo [Personalizzazione dettagli attività](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md) impostazioni. Al contrario, eventuali aggiornamenti apportati al campo dell’oggetto in Salesforce _non_ sincronizzare con il campo Oggetto attività promemoria Sales Connect.
