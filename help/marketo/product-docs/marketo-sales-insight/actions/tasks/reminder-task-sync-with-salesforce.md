---
description: Sincronizzazione attività promemoria con Salesforce - Documenti Marketo - Documentazione del prodotto
title: Sincronizzazione attività promemoria con Salesforce
exl-id: 11aa6ab5-5489-4c20-a64d-2fd6fe29506f
source-git-commit: 02354356949aef7aa8836d4753ec538b7819a65a
workflow-type: tm+mt
source-wordcount: '586'
ht-degree: 0%

---

# Sincronizzazione attività promemoria con Salesforce {#reminder-task-sync-with-salesforce}

>[!NOTE]
>
>Per informazioni su come attivare l&#39;estrazione di Sincronizzazione attività [Sincronizza attività/promemoria di Sales Insight con le attività Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md#sync-sales-insight-actions-tasks-reminders-to-salesforce-tasks).

Una volta abilitate le impostazioni di sincronizzazione delle attività, gli utenti vedranno le loro attività promemoria sincronizzate bidirezionalmente con Salesforce. Ciò significa che gli utenti possono gestire le attività dalle azioni Salesforce o Sales Insight e avere la certezza che i sistemi rimarranno allineati.

## Sincronizzazione campi attività promemoria {#reminder-task-field-sync}

![](assets/reminder-task-sync-with-salesforce-1.png)

Di seguito è riportato un elenco dei campi delle attività promemoria nelle azioni di approfondimento sulle vendite e dei corrispondenti campi Salesforce supportati tramite la sincronizzazione bidirezionale delle attività.

<table>
 <tr>
  <th>Campo attività Azioni approfondimento vendite</th>
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
  <td><p>Mostra lo stato dell'attività. Le attività Azioni approfondimento vendite hanno due stati che corrispondono a due dei valori nella lista di selezione dello stato delle attività di Salesforce.</p>
  <p>Aperto in Azioni approfondimento vendite = Non avviato in Salesforce.</p>
  <p>Completa in Azioni approfondimento vendite = Completato in Salesforce.</p>
  <p>Gli altri valori di stato in Salesforce non verranno sincronizzati con le azioni di approfondimento sulle vendite.</p></td>
 </tr>
 <tr>
  <td>Priorità</td>
  <td>Priorità</td>
  <td><p>La priorità delle azioni Sales Insight può essere Normal (Normale) o High (Alta), che corrisponde ai valori di priorità Normal (Normale) e High (Alta) in Salesforce.</p>
  <p>Il valore a bassa priorità in Salesforce non verrà sincronizzato con le azioni di approfondimento sulle vendite.</p></td>
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

## Sincronizzazione delle attività di Sales Insight con Salesforce per la prima volta {#syncing-sales-insight-actions-tasks-with-salesforce-for-the-first-time}

Quando attivi per la prima volta la sincronizzazione tra le azioni di approfondimento sulle vendite e le attività di Salesforce, importiamo le attività di Salesforce. Lo faremo **non** trasferisci a Salesforce tutte le attività correnti presenti in Azioni approfondimenti vendite. Per ridurre l’ingombro e i duplicati, le uniche attività sincronizzate dalle azioni di approfondimento sulle vendite in Salesforce sono le attività create *dopo* sincronizzi le azioni di Sales Insight con SFDC.

Ecco cosa accade quando si sincronizzano le azioni Sales Insight e le attività SFDC:

* Non appena si fa clic su Salva durante la sincronizzazione delle attività, queste vengono sincronizzate. Inizialmente questo richiederà del tempo.

* Tutti i promemoria aggiornati o creati nelle ultime 24 ore verranno inseriti da SFDC in Sales Insight Actions. La sincronizzazione è basata sulla data di scadenza e tutte queste attività verranno sincronizzate nel back-end, ma in Centro comandi verranno visualizzate solo le attività in scadenza oggi e domani.

* Se la sincronizzazione è stata attivata in precedenza ed è stata eliminata qualsiasi attività in SFDC, qualsiasi elemento eliminato negli ultimi 15 giorni verrà eliminato da Centro comandi.

* Sincronizzeremo costantemente le attività tra Sales Insight Actions e SFDC, purché la sincronizzazione sia abilitata.

Dopo la sincronizzazione iniziale, tutte le attività create, modificate, completate o eliminate in Azioni approfondimenti vendite verranno sincronizzate con l’elenco delle attività in Salesforce. E qualsiasi cosa creata, modificata, completata o eliminata in Salesforce aggiornerà l’elenco delle attività in Azioni approfondimento vendite.

Per attivare questa sincronizzazione, seleziona la casella di sincronizzazione nel [Pagina Impostazioni](https://toutapp.com/login) nell’applicazione web.

>[!NOTE]
>
>Il campo oggetto di un’attività può essere aggiornato in Azioni approfondimento vendite e tale aggiornamento verrà sincronizzato nel campo oggetto Salesforce per l’attività sincronizzata corrispondente, se utilizzi `{{activity_subject}}` campo dinamico nel tuo [Personalizzazione dettagli attività](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md) impostazioni. Al contrario, eventuali aggiornamenti apportati al campo dell’oggetto in Salesforce _non_ sincronizza con il campo Oggetto attività promemoria azioni approfondimenti vendite.
