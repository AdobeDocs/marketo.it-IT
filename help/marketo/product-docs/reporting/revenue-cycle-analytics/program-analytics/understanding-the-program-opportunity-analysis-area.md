---
unique-page-id: 2951877
description: Informazioni sull'area di analisi delle opportunità del programma - Documenti Marketo - Documentazione del prodotto
title: Informazioni sull'area di analisi delle opportunità del programma
translation-type: tm+mt
source-git-commit: cb7df3dd38275837f8ab05ce846c2c68ab78462f
workflow-type: tm+mt
source-wordcount: '896'
ht-degree: 0%

---


# Informazioni sull&#39;area di analisi delle opportunità del programma {#understanding-the-program-opportunity-analysis-area}

## Panoramica {#overview}

L&#39;area Analisi opportunità del programma consente di analizzare l&#39;efficacia dei singoli programmi o di visualizzare i risultati riepilogati per canale del programma.

**Di seguito sono riportati alcuni esempi di domande aziendali a cui puoi rispondere utilizzando questa area di analisi**:

Quante opportunità sono state associate a un determinato programma e quante di queste abbiamo vinto?

![](assets/one-1.png)

Quanti ricavi ha contribuito un determinato programma o canale?

![](assets/two-1.png)

Qual è il mio gettito sugli investimenti per un determinato programma o canale?

![](assets/three-1.png)

Quali opportunità ha influenzato un determinato programma?

![](assets/four-1.png)

## Misure di attribuzione analisi opportunità programma (punti blu) {#program-opportunity-analysis-attribution-measures-blue-dots}

Le misure disponibili per l&#39;analisi sono generalmente numeri e sono rappresentate da punti blu. I Dimension sono attributi che forniscono diverse viste delle misure e sono rappresentati da punti gialli.

Tutte le misure (puntini blu) si riferiscono all&#39;attribuzione - il &quot;credito&quot; per l&#39;acquisizione principale o per il successo delle vendite associato a un lead.

![](assets/six.five.png) ![](assets/seven-1.png)

Esistono tre tipi di misure:

* Misure relative all&#39;acquisizione, che ottengono l&#39;attribuzione &quot;first-touch&quot; (FT).
* Misure relative al successo, che ricevono l’attribuzione multi-touch (MT).
* Varie misure relative al programma, compreso il numero medio di contatti di marketing prima che vengano create o chiuse opportunità.

## Misure relative all&#39;acquisizione e al successo {#acquisition-and-success-related-measures}

Le misure relative all’acquisizione danno credito al programma attraverso il quale vengono prima ottenute le informazioni di contatto del lead. Un lead non deve raggiungere il successo in un programma di acquisizione del credito da aggiudicare.

Il valore dell’acquisizione di un dato lead cambia nel tempo. È pari a zero finché il lead non effettua un acquisto. Può quindi aumentare con acquisti aggiuntivi.

Le misure relative al successo danno credito a tutti i programmi che contribuiscono al progresso di un lead verso l’acquisto.

Come nel caso dell&#39;acquisizione, il valore del contributo alle vendite effettuate a un cambiamento lead nel tempo è pari a zero fino a quando l&#39;acquisto non viene effettuato dal lead.

<table> 
 <tbody> 
  <tr> 
   <th>Misura di attribuzione - Opportunità correlate (FT o MT)*</th> 
   <th>Descrizione</th> 
  </tr> 
  <tr> 
   <td>Costo dell'opportunità</td> 
   <td>La parte del costo del programma che ha influenzato l'opportunità. Il costo può essere suddiviso in caso di più lead.</td> 
  </tr> 
  <tr> 
   <td>Opportunità create</td> 
   <td>La parte di credito ricevuta dal programma per influenzare la creazione dell'opportunità. Può trattarsi di una frazione se sono coinvolti più lead.</td> 
  </tr> 
  <tr> 
   <td>Opportunità conquistate</td> 
   <td>La parte di credito ricevuta dal programma per influenzare l'opportunità di vincita. Può trattarsi di una frazione se sono coinvolti più lead.</td> 
  </tr> 
  <tr> 
   <td>Pipeline creata</td> 
   <td>La quota di credito (in valore monetario) ricevuta dal programma per influenzare la creazione dell'opportunità. Può trattarsi di una frazione se sono coinvolti più lead.</td> 
  </tr> 
  <tr> 
   <td>Pipeline creata - Still Open</td> 
   <td>La quota di credito (in valore monetario) ricevuta per influenzare la creazione dell'opportunità attualmente aperta. Può trattarsi di una frazione se sono coinvolti più lead.</td> 
  </tr> 
  <tr> 
   <td>Entrate previste</td> 
   <td>La quota di credito (in valore monetario) ricevuta dal programma per influenzare la creazione dell'opportunità. Entrate previste è la probabilità di opportunità moltiplicata per il valore dell'opportunità. Può trattarsi di una frazione se sono coinvolti più lead.</td> 
  </tr> 
  <tr> 
   <td>Entrate Da Investimento</td> 
   <td>Questo è il rapporto tra la quota di credito (in valore monetario) ricevuta dal programma per influenzare le opportunità e il costo del programma.</td> 
  </tr> 
  <tr> 
   <td>Entrate</td> 
   <td>La quota di credito (in valore monetario) ricevuta dal programma per influenzare le opportunità di vincita. Può trattarsi di una frazione se sono coinvolti più lead.</td> 
  </tr> 
 </tbody> 
</table>

_* (FT) = First-Touch Attribution, utilizzata per le misure di acquisizione del lead; (MT) = Attribuzione multi-touch, utilizzata per misure di successo iniziale_

Di seguito è riportato uno scenario che descrive come vengono calcolate le Unità opportunità in presenza di due programmi che hanno generato i lead, ma che hanno portato a un&#39;opportunità dallo stesso account.

**Programma 1**

* Genera un lead: Lead 1
* Il lead 1 proviene dal conto 1

**Programma 2**

* Genera un altro lead: Lead 2
* Il lead 2 proviene anche dal conto 1

**Conto 1**

* Genera un&#39;opportunità: Opportunità 1

Marketo concede il credito in modo appropriato senza il doppio conteggio delle opportunità tra i programmi. Quindi, in questo caso, ogni programma riceve 0,5 Unità Opportunità. In altre parole, ogni programma riceve la metà del credito per l&#39;Opportunità generata. Inoltre, metà delle entrate associate all&#39;opportunità viene assegnata a ciascun programma.

## Varie misure relative ai programmi {#miscellaneous-program-related-measures}

Le altre misure disponibili rispecchiano i risultati complessivi del programma.

<table> 
 <tbody> 
  <tr> 
   <th>Misura di attribuzione - Relativa al programma</th> 
   <th>Descrizione</th> 
  </tr> 
  <tr> 
   <td>Numero di opportunità associate al programma</td> 
   <td><p>Numero di opportunità totali che avevano concesso qualsiasi tipo di credito di attribuzione a un programma. Le opportunità possono essere influenzate da uno o più lead e da uno o più programmi.</p></td> 
  </tr> 
  <tr> 
   <td>Numero medio di successi per opportunità chiusa</td> 
   <td>Numero medio di successi del programma prima della chiusura dell'opportunità. <br></td> 
  </tr> 
  <tr> 
   <td>Numero medio di successi per opportunità creata</td> 
   <td>Numero medio di successi dei programmi prima della creazione dell'opportunità.</td> 
  </tr> 
  <tr> 
   <td>Nuovi nomi</td> 
   <td>Il numero totale di nuovi nomi, ossia nuovi lead, acquisiti dal programma.</td> 
  </tr> 
  <tr> 
   <td>Costo del programma</td> 
   <td>Costo totale del programma.</td> 
  </tr> 
  <tr> 
   <td>Successo (totale)</td> 
   <td>Il numero totale di membri del programma che hanno raggiunto il successo.</td> 
  </tr> 
 </tbody> 
</table>

## Dimension di analisi delle opportunità del programma (punti gialli) {#program-opportunity-analysis-dimensions-yellow-dots}

Mentre le misure (punti blu) vengono calcolate e richiedono riflessione e spiegazioni, le dimensioni (punti gialli) sono descrittive. Ecco le dimensioni disponibili.

<table> 
 <tbody> 
  <tr> 
   <th>Categoria</th> 
   <th>Etichetta visualizzazione</th> 
  </tr> 
  <tr> 
   <td>Attributi opportunità</td> 
   <td>Opportunità chiusa<br>Nome opportunità*<br>Nome proprietario opportunità<br>Stage opportunità<br>Tipo opportunità</td> 
  </tr> 
  <tr> 
   <td>Timeframe opportunità</td> 
   <td>Opportunità chiusa anno/trimestre/mese<br>Opportunità creata anno/trimestre/mese</td> 
  </tr> 
  <tr> 
   <td>Attributi del programma</td> 
   <td>Canale programma<br>Nome programma</td> 
  </tr> 
  <tr> 
   <td>Calendario costi programma</td> 
   <td>Anno costo/trimestre/mese</td> 
  </tr> 
 </tbody> 
</table>

**Tutte le opportunità che hanno concesso un qualsiasi tipo di credito di attribuzione a un programma. Le opportunità possono essere influenzate da uno o più lead e da uno o più programmi.*

>[!MORELIKETHIS]
>
>[Creazione di un rapporto di Esplora entrate](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/create-a-revenue-explorer-report.md)
