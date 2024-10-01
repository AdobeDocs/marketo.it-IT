---
description: Metriche backlog di sincronizzazione Salesforce - Documentazione Marketo - Documentazione del prodotto
title: Metriche backlog di sincronizzazione Salesforce
hide: true
hidefromtoc: true
feature: Reporting
source-git-commit: a9ed4a7e2247a26b376bde64bb1cfd6db2833822
workflow-type: tm+mt
source-wordcount: '840'
ht-degree: 0%

---

# Metriche backlog di sincronizzazione Salesforce  {#salesforce-sync-backlog-metrics}

Il backlog di sincronizzazione rappresenta i record in attesa di sincronizzazione da Salesforce a Marketo Engage e viceversa. Assicurando che il backlog rimanga sotto controllo, le sincronizzazioni saranno regolari e tempestive.

>[!NOTE]
>
>Il backlog copre i numeri di post-aggiornamenti di sincronizzazione in sospeso su entrambi i lati e non quelli eseguiti da passaggi del flusso di sincronizzazione come i passaggi del flusso [Sincronizza persona in SFDC](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/sync-person-to-sfdc.md){target="_blank"} o [Sincronizza persona in Microsoft](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/microsoft-dynamics-flow-actions/sync-person-to-microsoft.md){target="_blank"}.

## Come accedere {#how-to-access}

1. In Marketo Engage, vai all&#39;area **Amministratore**.

   SCHERMATA

1. Seleziona **Salesforce**.

   SCHERMATA

## Tendenza backlog di sincronizzazione {#sync-backlog-trend}

La tendenza dell’arretrato riflette le variazioni degli arretrati registrati negli ultimi 5 giorni. Il backlog viene visualizzato in un intervallo di tempo di 4 ore distribuito su 5 giorni. Pertanto, il grafico mostrerà 6 intervalli al giorno per 5 giorni, che equivalgono a 30 intervalli.

Il backlog si osserva a un particolare intervallo di 4 ore sull’asse x. Questo valore si riferisce a tutti gli oggetti sincronizzati. Totale del backlog in Salesforce e nel Marketo Engage in attesa di sincronizzazione.

SCHERMATA

## Throughput di sincronizzazione e backlog {#sync-throughput-and-backlog}

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
    <td>Stima del tempo necessario per sincronizzare il backlog per tipo di oggetto. Calcolato come 'Backlog sincronizzato/Media record sincronizzati all'ora'.</td>
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

## Cause dei backlog di sincronizzazione {#what-causes-sync-backlogs}

Sia che l&#39;aggiornamento venga eseguito sul lato Marketo Engage o sul lato CRM, verrà attivata la risincronizzazione del record per aggiornare le informazioni sull&#39;altro lato tramite il normale ciclo di sincronizzazione tra il Marketo Engage e il sistema CRM. Ogni volta che si aggiorna un record in Salesforce, viene generato un timestamp di modifica del sistema, denominato &#39;SysModStamp&#39;. In questo modo viene accodata una modifica alla sincronizzazione.

Quando si esegue una grande quantità di aggiornamenti (ad esempio, se si modifica il valore di un campo), molti record vengono modificati, creando nuovi SysModStamps. Un numero elevato di aggiornamenti dei record persona deve quindi essere risincronizzato tra il Marketo Engage e il CRM, a volte creando un backlog momentaneo.

## Procedure consigliate per la gestione dei backlog di sincronizzazione {#best-practices-for-managing-sync-backlogs}

**Campi sincronizzati**: verificare che i campi sincronizzati siano solo quelli da sincronizzare. Le modifiche apportate ai campi aumentano il backlog di sincronizzazione e i campi con priorità inferiore potrebbero arrestare o rallentare la sincronizzazione di campi più importanti. Rivolgiti al [Supporto Marketo Engage](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} per rimuovere i campi sincronizzati.

**Campi sensibili**: alcuni campi sono soggetti ad aggiornamenti frequenti (ad esempio campi di valuta soggetti a modifiche). Controlla se è necessario sincronizzarli o se i campi devono essere progettati in modo diverso.

**Oggetti personalizzati**: rivedi periodicamente gli oggetti personalizzati in sincronia e rimuovi quelli che non devono più essere sincronizzati.

**Attività**: verifica se sono presenti attività sincronizzate che è possibile rimuovere dalla sincronizzazione.

**Pianifica aggiornamenti in blocco durante le ore non critiche**: controlla i modelli di sincronizzazione dei dati per identificare i periodi non critici. Verifica se è possibile pianificare aggiornamenti in blocco durante questi periodi non critici.

Se segui tutte le best practice di cui sopra e stai ancora riscontrando backlog significativi, contatta il [Supporto Marketo Engage](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.
