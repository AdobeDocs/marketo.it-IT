---
description: Dashboard delle metriche di osservabilità della sincronizzazione di Salesforce - Documentazione di Marketo - Documentazione del prodotto
title: Dashboard delle metriche di osservabilità sincronizzazione di Salesforce
hide: true
hidefromtoc: true
feature: Reporting
source-git-commit: 2457f0f51c6365c29a040e908678e81517327de5
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 0%

---

# Metriche backlog di sincronizzazione Salesforce  {#salesforce-sync-backlog-metrics}

Esamina le prestazioni di sincronizzazione effettive e sincronizza i backlog con questo dashboard.

## Throughput di sincronizzazione e backlog {#sync-throughput-and-backlog}

1. In Marketo Engage, vai all’area Amministratore.

   SCHERMATA

1. Seleziona Salesforce.

   SCHERMATA

Le statistiche riflettono la velocità effettiva e lo stato del backlog per ogni tipo di oggetto sincronizzato nelle ultime 24 ore. I tipi di oggetto includono tutti gli oggetti sincronizzati, tra cui: lead, contatto, account, opportunità, campagna, utente e oggetti personalizzati. Le statistiche della velocità effettiva vengono aggiornate automaticamente ogni 15 minuti, ma puoi aggiornare manualmente utilizzando l’icona di aggiornamento. Il backlog viene recuperato ogni ora.

>[!NOTE]
>
>Le statistiche vengono aggiornate su base continua, non per giorno di calendario.

SCHERMATA

<table><thead>
  <tr>
    <th>Campo</th>
    <th>Descrizione</th>
  </tr></thead>
<tbody>
  <tr>
    <td>Numero massimo di record sincronizzati/ora</td>
    <td>Numero massimo di record sincronizzati all'ora (throughput massimo) osservato nelle ultime 24 ore per il tipo di oggetto. Il periodo di 24 ore ruota con il tempo, non con il giorno di calendario.</td>
  </tr>
  <tr>
    <td>Record minimi sincronizzati / ora</td>
    <td>Numero minimo di record sincronizzati all'ora (velocità effettiva minima) osservati nelle ultime 24 ore per il tipo di oggetto. Il periodo di 24 ore ruota con il tempo, non con il giorno di calendario.</td>
  </tr>
  <tr>
    <td>Media record sincronizzati/ora</td>
    <td>Numero medio di record sincronizzati all'ora (velocità effettiva minima) osservati nelle ultime 24 ore per il tipo di oggetto. Il periodo di 24 ore ruota con il tempo, non con il giorno di calendario. Questo viene calcolato come numero totale di record sincronizzati nelle ultime 24 ore.</td>
  </tr>
  <tr>
    <td>Sincronizza backlog</td>
    <td>Il backlog dei record in attesa di sincronizzazione per il tipo di oggetto. È la somma totale della sincronizzazione in sospeso del backlog in entrambe le direzioni (da Salesforce a Marketo Engage e viceversa). Il backlog da Salesforce viene ottenuto utilizzando una chiamata API a Salesforce e il backlog da Marketo Engage viene calcolato utilizzando le statistiche ottenute dal log dei dati di modifica. Questo viene calcolato ogni ora. I due campi successivi di questa tabella indicano rispettivamente quando è stato calcolato l'ultimo backlog e la pianificazione successiva per il calcolo.</td>
  </tr>
  <tr>
    <td>Backlog stimato (tempo)</td>
    <td>Stima del tempo necessario per sincronizzare il backlog per tipo di oggetto. Calcolato come backlog di sincronizzazione/media dei record sincronizzati all'ora.</td>
  </tr>
  <tr>
    <td>Ultimo recupero backlog</td>
    <td>Ora dell'ultimo calcolo del backlog.</td>
  </tr>
  <tr>
    <td>Recupero successivo backlog</td>
    <td>Ora del successivo calcolo del backlog.</td>
  </tr>
  <tr>
    <td>Stato backlog</td>
    <td>Questo mostra se il backlog è cresciuto nelle ultime 6 ore. Se il backlog corrente è maggiore del backlog registrato 6 ore fa, viene dedotto "In crescita". In caso contrario, verrà visualizzato come 'Normale'. Questo serve a mostrare se il throughput di sincronizzazione sta raggiungendo il backlog.</td>
  </tr>
</tbody></table>

## Tendenza backlog {#backlog-trend}

La tendenza dell’arretrato riflette le variazioni degli arretrati registrati negli ultimi 5 giorni. Il backlog viene visualizzato in un intervallo di tempo di 4 ore distribuito su 5 giorni. Pertanto, il grafico mostrerà 6 intervalli al giorno per 5 giorni, che equivalgono a 30 intervalli.

Il backlog si osserva a un particolare intervallo di 4 ore sull’asse x. Questo valore si riferisce a tutti gli oggetti sincronizzati. Totale del backlog in Salesforce e nel Marketo Engage in attesa di sincronizzazione.

SCHERMATA
