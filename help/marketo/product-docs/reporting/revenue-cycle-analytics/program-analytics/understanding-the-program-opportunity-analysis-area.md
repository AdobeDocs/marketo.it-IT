---
unique-page-id: 2951877
description: Informazioni sull’area di analisi delle opportunità del programma - Documentazione di Marketo - Documentazione del prodotto
title: Informazioni sull’area di analisi delle opportunità del programma
exl-id: 6105df93-b3de-4929-85e3-fd328372bd24
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '896'
ht-degree: 0%

---

# Informazioni sull’area di analisi delle opportunità del programma {#understanding-the-program-opportunity-analysis-area}

## Panoramica {#overview}

L’area Analisi opportunità programma consente di analizzare l’efficacia dei singoli programmi o di visualizzare un riepilogo dei risultati per canale del programma.

**Esempio di domande aziendali a cui è possibile rispondere utilizzando questa area di analisi:**:

Quante opportunità sono state associate a un determinato programma e quante ne abbiamo vinte?

![](assets/one-1.png)

A quanto ammontano i ricavi generati da un determinato programma o canale?

![](assets/two-1.png)

Qual è il ricavo da investire per un determinato programma o canale?

![](assets/three-1.png)

Quali opportunità ha influenzato un determinato programma?

![](assets/four-1.png)

## Misure di attribuzione analisi opportunità programma (punti blu) {#program-opportunity-analysis-attribution-measures-blue-dots}

Le misure disponibili per l&#39;analisi sono in genere numeri e sono rappresentate da punti blu. I Dimension sono attributi che forniscono viste diverse delle misure e sono rappresentati da punti gialli.

Tutte le misure (punti blu) si riferiscono all’attribuzione: il &quot;merito&quot; per l’acquisizione di lead o per il successo di vendita associato a un lead.

![](assets/six.five.png) ![](assets/seven-1.png)

Esistono tre tipi di misure:

* Misure relative all’acquisizione, che ottengono l’attribuzione del primo contatto (FT).
* Misure relative al successo, che ricevono l’attribuzione multi-touch (MT).
* Varie misure relative al programma, tra cui il numero medio di contatti di marketing prima della creazione o della chiusura delle opportunità.

## Acquisizione e misure di successo {#acquisition-and-success-related-measures}

Le misure relative all’acquisizione danno credito al programma attraverso il quale vengono ottenute per la prima volta le informazioni di contatto di un lead. Un lead non deve raggiungere il successo in un programma per l&#39;acquisizione di crediti da aggiudicare.

Il valore dell’acquisizione di un determinato lead cambia nel tempo. È pari a zero finché il lead non effettua un acquisto. Può quindi aumentare con acquisti aggiuntivi.

Le misure di successo attribuiscono un merito a tutti i programmi che contribuiscono ai progressi di un lead verso un acquisto.

Come per l’acquisizione, il valore del contributo alle vendite effettuate a un lead cambia nel tempo ed è pari a zero finché il lead non effettua un acquisto.

<table> 
 <tbody> 
  <tr> 
   <th>Misura di attribuzione - Correlata all’opportunità (FT o MT)*</th> 
   <th>Descrizione</th> 
  </tr> 
  <tr> 
   <td>Costo dell’opportunità</td> 
   <td>La parte del costo del programma che ha influenzato l’opportunità. Il costo può essere suddiviso se sono coinvolti più lead.</td> 
  </tr> 
  <tr> 
   <td>Opportunità create</td> 
   <td>La porzione di credito ricevuta dal programma per aver influenzato la creazione dell’opportunità. Può essere una frazione se sono coinvolti più lead.</td> 
  </tr> 
  <tr> 
   <td>Opportunità acquisite</td> 
   <td>La porzione di credito ricevuta dal programma per aver influenzato l’opportunità acquisita. Può essere una frazione se sono coinvolti più lead.</td> 
  </tr> 
  <tr> 
   <td>Pipeline creata</td> 
   <td>La parte di credito (in valore monetario) ricevuta dal programma per influenzare la creazione dell’opportunità. Può essere una frazione se sono coinvolti più lead.</td> 
  </tr> 
  <tr> 
   <td>Pipeline creata - Ancora aperta</td> 
   <td>La parte di credito (in valore monetario) ricevuta dal programma per influenzare la creazione dell’opportunità attualmente aperta. Può essere una frazione se sono coinvolti più lead.</td> 
  </tr> 
  <tr> 
   <td>Ricavi previsti</td> 
   <td>La parte di credito (in valore monetario) ricevuta dal programma per influenzare la creazione dell’opportunità. Ricavi previsti è la probabilità di opportunità moltiplicata per il valore di opportunità. Può essere una frazione se sono coinvolti più lead.</td> 
  </tr> 
  <tr> 
   <td>Ricavi - Investimento</td> 
   <td>Si tratta del rapporto tra la parte di credito (in valore monetario) ricevuta dal programma per influenzare le opportunità realizzate e il costo del programma.</td> 
  </tr> 
  <tr> 
   <td>Ricavi ottenuti</td> 
   <td>La parte di credito (in valore monetario) ricevuta dal programma per influenzare l’opportunità acquisita. Può essere una frazione se sono coinvolti più lead.</td> 
  </tr> 
 </tbody> 
</table>

_&#42;(FT) = First-Touch Attribution, utilizzato per le misure di acquisizione dei lead; (MT) = Multi-Touch Attribution, utilizzato per le misure di successo dei lead_

Di seguito è riportato uno scenario che descrive come vengono calcolate le unità di opportunità quando sono presenti due programmi che hanno generato lead, ma tali lead hanno portato a un’opportunità dallo stesso account.

**Programma 1**

* Genera un lead: Lead 1
* Il lead 1 proviene dal conto 1

**Programma 2**

* Genera un altro lead: Lead 2
* Lead 2 proviene anche dall&#39;account 1

**Account 1**

* Genera un&#39;opportunità: opportunità 1

Marketo attribuisce il merito in modo appropriato senza il doppio conteggio delle opportunità tra i programmi. In questo caso, ogni programma riceve 0,5 unità di opportunità. In altre parole, ogni programma riceve la metà del credito per l’opportunità generata. Inoltre, metà dei ricavi associati all’opportunità viene assegnata a ciascun programma.

## Misure Varie Connesse Al Programma {#miscellaneous-program-related-measures}

Le altre misure disponibili riflettono i risultati complessivi del programma.

<table> 
 <tbody> 
  <tr> 
   <th>Misura di attribuzione: correlata al programma</th> 
   <th>Descrizione</th> 
  </tr> 
  <tr> 
   <td>N. di opportunità associate al programma</td> 
   <td><p>Il numero totale di opportunità che hanno assegnato qualsiasi tipo di credito di attribuzione a un programma. Le opportunità possono essere influenzate da uno o più lead e da uno o più programmi.</p></td> 
  </tr> 
  <tr> 
   <td>Numero medio di successi per opportunità chiusa</td> 
   <td>Numero medio di successi del programma prima della chiusura dell’opportunità. <br></td> 
  </tr> 
  <tr> 
   <td>Numero medio di successi per opportunità creata</td> 
   <td>Numero medio di programmi riusciti prima della creazione dell’opportunità.</td> 
  </tr> 
  <tr> 
   <td>Nuovi nomi</td> 
   <td>Numero totale di nuovi nomi, ovvero nuovi lead, acquisiti dal programma.</td> 
  </tr> 
  <tr> 
   <td>Costo programma</td> 
   <td>Costo totale del programma.</td> 
  </tr> 
  <tr> 
   <td>Completato (totale)</td> 
   <td>Numero totale di membri del programma che hanno raggiunto il successo.</td> 
  </tr> 
 </tbody> 
</table>

## Dimension di analisi delle opportunità del programma (punti gialli) {#program-opportunity-analysis-dimensions-yellow-dots}

Mentre le misure (punti blu) vengono calcolate e richiedono un certo pensiero e una spiegazione da utilizzare, le dimensioni (punti gialli) sono descrittive. Di seguito sono riportate le dimensioni disponibili.

<table> 
 <tbody> 
  <tr> 
   <th>Categoria</th> 
   <th>Etichetta visualizzazione</th> 
  </tr> 
  <tr> 
   <td>Attributi di opportunità</td> 
   <td>Opportunità chiusa<br>Nome opportunità*<br>Nome del proprietario dell’opportunità<br>Fase dell’opportunità<br>Tipo di opportunità</td> 
  </tr> 
  <tr> 
   <td>Intervallo temporale dell’opportunità</td> 
   <td>Opportunità chiusa anno/trimestre/mese<br>Opportunità creata anno/trimestre/mese</td> 
  </tr> 
  <tr> 
   <td>Attributi del programma</td> 
   <td>Canale del programma<br>Nome del programma</td> 
  </tr> 
  <tr> 
   <td>Intervallo temporale costi programma</td> 
   <td>Costo anno/trimestre/mese</td> 
  </tr> 
 </tbody> 
</table>

*&#42;Tutte le opportunità che hanno assegnato qualsiasi tipo di merito di attribuzione a un programma. Le opportunità possono essere influenzate da uno o più lead e da uno o più programmi.*

>[!MORELIKETHIS]
>
>[Creare un rapporto di Gestione ricavi](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-explorer/create-a-revenue-explorer-report.md)
