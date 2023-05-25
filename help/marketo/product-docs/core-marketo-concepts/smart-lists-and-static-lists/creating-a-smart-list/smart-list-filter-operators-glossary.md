---
unique-page-id: 557312
description: Glossario degli operatori di filtri per elenchi avanzati - Documentazione di Marketo - Documentazione del prodotto
title: Glossario degli operatori di filtro elenchi avanzati
exl-id: 5a370482-f214-4909-bb49-801c1a36b153
source-git-commit: 5ffb1a1931ccbc945ba535f72898a1b73154e47a
workflow-type: tm+mt
source-wordcount: '605'
ht-degree: 11%

---

# Glossario degli operatori di filtro elenchi avanzati {#smart-list-filter-operators-glossary}

Un operatore fa parte dell’elenco avanzato, che consente di ottenere specifiche. Ti consente di descrivere il filtro o l’attivatore in un linguaggio semplice. Gli operatori disponibili sono diversi per ogni tipo di campo.

Di seguito è riportato un glossario che descrive ogni insieme di operatori.

## Campi data {#date-fields}

![](assets/image2014-9-10-17-3a15-3a47.png)

Quando scegli un operatore, il lato destro cambia in modo dinamico.

| Operatore | Lato destro | Descrizione |
|---|---|---|
| è | Data singola | Corrispondenza data esatta |
| non è | Data singola | Qualsiasi data ECCETTO quella specificata |
| tra | Due campi data | Qualsiasi data compresa tra due date specificate |
| nel passato | Input lingua naturale&#42; | Vedi il diagramma seguente |
| nel passato prima di | Input lingua naturale&#42; | Vedi il diagramma seguente |
| nel futuro | Input lingua naturale&#42; | Vedi il diagramma seguente |
| nel futuro dopo | Input lingua naturale&#42; | Vedi il diagramma seguente |
| nell’intervallo temporale | Predefiniti (ultimo trimestre, ieri, ecc.) | Definito nell’elenco a discesa |
| dopo | Data singola | Tutti i record dopo la data specificata |
| prima di | Data singola | Tutti i record prima di quello specificato |
| il o dopo il | Data singola | Come &quot;dopo&quot; ma inclusivo |
| entro | Data singola | Come &quot;prima&quot; ma inclusivo |
| è vuoto | Nessuna | Tutti i record senza data |
| non è vuoto | Nessuna | Tutti i record con qualsiasi data |

&#42; L&#39;input del linguaggio naturale è figo. Di seguito sono riportati alcuni dei pattern che è possibile immettere:

* 1 ora
* 82 giorni
* 3 settimane
* 14 mesi
* 1 anno

Basta digitare il numero e l&#39;unità e funzionerà!

>[!NOTE]
>
>&quot;Nel passato&quot; **fa** includi il giorno (fino all’ora, non dopo) in cui hai creato l’elenco avanzato.

>[!CAUTION]
>
>Quando crei un elenco avanzato utilizzando un filtro per campo data (ad esempio, Data di nascita, Data di creazione SFDC) e utilizzi i vincoli **prima di**, **il o prima del**, o **in passato prima di**, l’elenco avanzato includerà anche le persone che non hanno valore in detto campo data.

Utilizza il diagramma seguente per comprendere la differenza tra gli operatori di data.

![](assets/image2014-9-10-17-3a15-3a58.png)

>[!NOTE]
>
>**Esempio**
>
>I campi data possono diventare complessi quando si lavora con eventi passati e futuri. Ecco un paio di esempi.
>
>**In passato prima di**
>
>Per la tua nuova promozione, utilizza questo operatore per inviare e-mail solo a persone che non si sono abbonate o hanno rinnovato il servizio entro un anno o non sono mai state abbonate.
>
>**In futuro dopo**
>
>Se vuoi vedere clienti che sono pronti per il rinnovo entro 90 giorni, Puoi utilizzare due filtri separati. Prima utilizzare &quot;In futuro dopo 90 giorni&quot; e seconda, &quot;In futuro 91 giorni&quot;. In questo modo chiunque abbia una data compresa tra 90 giorni.

## Campi stringa {#string-fields}

![](assets/image2014-9-10-17-3a16-3a6.png)

| Operatore | Descrizione |
|---|---|
| è | Corrispondenza esatta (senza distinzione maiuscole/minuscole) |
| non è | Qualsiasi cosa TRANNE la corrispondenza esatta |
| inizia con | Prime lettere di corrispondenza stringa |
| non inizia con | Le prime lettere della stringa NON corrispondono |
| contiene | Tutte le lettere insieme nella corrispondenza delle stringhe (ad esempio: california, fortune, quindi) |
| non contiene | Nessuna corrispondenza tra lettere nella stringa. (retro di &quot;contiene&quot;) |
| è vuoto | Record privi di valore (NULL) |
| non è vuoto | Record con qualsiasi valore |

>[!TIP]
>
>Utilizza operatori positivi rispetto a negativi. I filtri &quot;Non è&quot; devono cercare l’intero set di dati nella tua istanza, il che può richiedere molto tempo. I filtri &quot;is&quot; positivi possono sfruttare algoritmi di ricerca più efficaci.

## Campi interi {#integer-fields}

![](assets/image2014-9-10-17-3a16-3a14.png)

<table> 
 <thead> 
  <tr> 
   <th colspan="1" rowspan="1">Operatore</th> 
   <th colspan="1" rowspan="1">Descrizione</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td colspan="1" rowspan="1">è</td> 
   <td colspan="1" rowspan="1">Il numero esatto corrisponde ( = 0 restituirà entrambi i lead con 0 <em>e</em> NULL)</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">non è</td> 
   <td colspan="1" rowspan="1">Qualsiasi cosa TRANNE il numero esatto corrisponde</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">tra</td> 
   <td colspan="1" rowspan="1">Definisci due valori per trovare tutti nel mezzo (inclusi)</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">maggiore di</td> 
   <td colspan="1" rowspan="1">Sopra il valore specificato</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">minore di</td> 
   <td colspan="1" rowspan="1">Minore del valore specificato</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">almeno</td> 
   <td colspan="1" rowspan="1">Al di sopra del valore specificato (incluso)</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">al massimo</td> 
   <td colspan="1" rowspan="1">Minore del valore specificato (incluso)</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">è vuoto</td> 
   <td colspan="1" rowspan="1">Record privi di valore (NULL): zero è un numero, è <em>non</em> NULL</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">non è vuoto</td> 
   <td colspan="1" rowspan="1">Record con QUALSIASI valore (incluso zero)</td> 
  </tr> 
 </tbody> 
</table>

Come potete vedere, questi operatori facilitano l&#39;uso del linguaggio Marketo con fluenza!
