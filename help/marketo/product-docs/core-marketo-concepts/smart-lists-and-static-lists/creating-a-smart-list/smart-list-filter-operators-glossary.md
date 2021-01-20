---
unique-page-id: 557312
description: Smart List Filtri Operatori Glossario - Marketo Docs - Documentazione del prodotto
title: Glossario degli operatori di filtri per elenchi avanzati
translation-type: tm+mt
source-git-commit: 5b9f48c98464c79bcdca2e335f6a4a2edce98ce4
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---


# Glossario degli operatori di filtri per elenchi avanzati {#smart-list-filter-operators-glossary}

Un operatore è una parte dell&#39;elenco smart che consente di ottenere informazioni specifiche. Consente di descrivere il filtro o l’attivatore in un linguaggio semplice. Gli operatori disponibili sono diversi per ciascun tipo di campo.

Questo è un glossario che descrive ogni insieme di operatori.

## Campi data {#date-fields}

![](assets/image2014-9-10-17-3a15-3a47.png)

Quando si sceglie un operatore, il lato destro cambia in modo dinamico.

| Operatore | Lato destro | Descrizione |
|---|---|---|
| is | Data singola | Corrispondenza data esatta |
| is not | Data singola | Qualsiasi data TRANNE quella specificata |
| tra | Due campi data | Qualsiasi data che include e tra due date specificate |
| in passato | Input lingua naturale* | Vedere il diagramma seguente |
| in passato | Input lingua naturale* | Vedere il diagramma seguente |
| in futuro | Input lingua naturale* | Vedere il diagramma seguente |
| in futuro | Input lingua naturale* | Vedere il diagramma seguente |
| nel tempo | Predefiniti (ultimo trimestre, ieri ecc.) | Definito in elenco di selezione |
| after | Data singola | Tutti i record dopo la data specificata |
| before | Data singola | Tutti i record prima di quello specificato |
| o dopo | Data singola | Come &quot;after&quot; ma incluso |
| o prima | Data singola | Come &quot;prima&quot; ma incluso |
| è vuoto | None | Tutti i record senza data |
| non è vuoto | None | Tutti i record con qualsiasi data |

* L&#39;input in lingua naturale è fantastico. Di seguito sono riportati alcuni dei pattern che è possibile inserire:

* 1 ora
* 82 giorni
* 3 settimane
* 14 mesi
* 1 anno

Basta digitare il numero e l&#39;unità insieme e funzionerà!

>[!NOTE]
>
>&quot;In passato&quot; **fa** include il giorno (fino all&#39;ora, non dopo) in cui si crea l&#39;elenco smart.

>[!CAUTION]
>
>Quando si crea un elenco avanzato utilizzando un filtro di campo data (ad esempio, Data di nascita, Data di creazione SFDC) e si utilizzano i vincoli **before** o **on o precedenti**, l&#39;elenco smart list includerà anche le persone che non hanno alcun valore in tale campo data.

Usare il diagramma seguente per comprendere la differenza tra gli operatori data.

![](assets/image2014-9-10-17-3a15-3a58.png)

>[!NOTE]
>
>**Esempio**
>
>I campi data possono diventare difficili quando si lavora con eventi passati e futuri. Ecco un paio di esempi.
>
>**In passato**
>
>Per la nuova promozione, utilizza questo operatore per inviare e-mail solo a persone che non hanno sottoscritto o rinnovato il servizio entro un anno o che non sono mai state sottoscritte.
>
>**In futuro**
>
>Supponiamo di voler vedere i clienti che saranno rinnovati entro 90 giorni. Vengono utilizzati due filtri separati. Primo utilizzo &quot;In futuro dopo 90 giorni&quot;, e secondo, &quot;In futuro 91 giorni.&quot; Questo catturerebbe chiunque abbia una data di 90 giorni da ora.

## Campi stringa {#string-fields}

![](assets/image2014-9-10-17-3a16-3a6.png)

| Operatore | Descrizione |
|---|---|
| is | Corrispondenza esatta (senza distinzione tra maiuscole e minuscole) |
| is not | Eccetto la corrispondenza esatta |
| inizia con | Prime lettere della corrispondenza stringa |
| non inizia con | Le prime lettere della stringa NON corrispondono |
| contains | Tutte le lettere nella corrispondenza stringa (esempio: California, fortuna, quindi) |
| not contains | Nessuna corrispondenza nella corrispondenza stringa. (al contrario di &quot;contains&quot;) |
| è vuoto | Record senza valore (NULL) |
| non è vuoto | Record con valore ANY |

>[!TIP]
>
>Utilizzate operatori positivi rispetto a operatori negativi. I filtri &quot;Non è&quot; devono cercare l&#39;intero set di dati nell&#39;istanza, il che può richiedere molto tempo. I filtri &quot;is&quot; positivi possono sfruttare algoritmi di ricerca più efficaci.

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
   <td colspan="1" rowspan="1">is</td> 
   <td colspan="1" rowspan="1">Corrispondenza numero esatta ( = 0 restituisce entrambi i lead con 0 <em>e</em> NULL)</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">is not</td> 
   <td colspan="1" rowspan="1">Qualsiasi valore ECCETTO numero esatto corrispondente</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">tra</td> 
   <td colspan="1" rowspan="1">Definite due valori per trovare tutti gli utenti intermedi (incluso)</td> 
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
   <td colspan="1" rowspan="1">Sopra il valore specificato (incluso)</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">al massimo</td> 
   <td colspan="1" rowspan="1">Minore del valore specificato (incluso)</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">è vuoto</td> 
   <td colspan="1" rowspan="1">Record senza valore (NULL) - zero è un numero, è <em>not</em> NULL</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">non è vuoto</td> 
   <td colspan="1" rowspan="1">Record con valore ANY (incluso zero)</td> 
  </tr> 
 </tbody> 
</table>

Come potete vedere, questi operatori rendono facile parlare Marketo-ese con fluenza!
