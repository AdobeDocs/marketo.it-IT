---
unique-page-id: 557312
description: Glossario degli operatori di filtri di elenchi avanzati - Documenti Marketo - Documentazione del prodotto
title: Glossario degli operatori di filtri di elenchi avanzati
exl-id: 5a370482-f214-4909-bb49-801c1a36b153
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# Glossario degli operatori di filtri di elenchi avanzati {#smart-list-filter-operators-glossary}

Un operatore è una parte dell’elenco avanzato che consente di ottenere informazioni specifiche. Ti consente di descrivere il filtro o l’attivatore in un linguaggio semplice. Gli operatori disponibili sono diversi per ciascun tipo di campo.

Ecco un glossario che descrive ogni set di operatori.

## Campi data {#date-fields}

![](assets/image2014-9-10-17-3a15-3a47.png)

Quando scegli un operatore, il lato destro cambia dinamicamente.

| Operatore | Lato destro | Descrizione |
|---|---|---|
| è | Data singola | Corrispondenza data esatta |
| non | Data singola | Qualsiasi data tranne quella specificata |
| tra | Due campi data | Qualsiasi data che include e tra due date specificate |
| in passato | Input lingua naturale* | Vedi il diagramma seguente |
| in passato | Input lingua naturale* | Vedi il diagramma seguente |
| in futuro | Input lingua naturale* | Vedi il diagramma seguente |
| in futuro | Input lingua naturale* | Vedi il diagramma seguente |
| in tempo | Predefiniti (ultimo trimestre, ieri ecc.) | Definito in elenco a discesa |
| dopo | Data singola | Tutti i record dopo la data specificata |
| prima | Data singola | Tutti i record precedenti a quello specificato |
| o dopo | Data singola | Come &quot;dopo&quot; ma inclusivo |
| o prima | Data singola | Come &quot;prima&quot; ma inclusivo |
| è vuoto | Nessuno | Tutti i record senza data |
| non è vuoto | Nessuno | Tutti i record con qualsiasi data |

* L&#39;input del linguaggio naturale è fresco. Di seguito sono riportati alcuni dei pattern che è possibile immettere:

* 1 ora
* 82 giorni
* 3 settimane
* 14 mesi
* 1 anno

Basta digitare il numero e l&#39;unità insieme e funzionerà!

>[!NOTE]
>
>&quot;In passato&quot; **does** include il giorno (fino all&#39;ora e non dopo) in cui hai creato il tuo elenco smart.

>[!CAUTION]
>
>Quando crei un elenco avanzato utilizzando un filtro per campi data (ad esempio Data di nascita, Data creazione DSC) e utilizzi i vincoli **before** o **on o before** , l’elenco avanzato includerà anche le persone che non hanno alcun valore in tale campo data.

Utilizza il diagramma seguente per comprendere la differenza tra gli operatori data.

![](assets/image2014-9-10-17-3a15-3a58.png)

>[!NOTE]
>
>**Esempio**
>
>I campi data possono diventare difficili quando si lavora con eventi passati e futuri. Ecco un paio di esempi.
>
>**In passato**
>
>Per la nuova promozione, utilizza questo operatore per inviare e-mail solo a persone che non si sono abbonate o rinnovate il servizio entro un anno o che non sono mai state abbonate.
>
>**In futuro dopo**
>
>Supponiamo di voler vedere i clienti in fase di rinnovo entro 90 giorni. Dovresti utilizzare due filtri separati. Primo utilizzo &quot;In futuro dopo 90 giorni&quot;, e secondo, &quot;In futuro 91 giorni.&quot; Questo catturerebbe chiunque abbia un appuntamento tra 90 giorni.

## Campi stringa {#string-fields}

![](assets/image2014-9-10-17-3a16-3a6.png)

| Operatore | Descrizione |
|---|---|
| è | Corrispondenza esatta (senza distinzione tra maiuscole e minuscole) |
| non | Qualsiasi tranne la corrispondenza esatta |
| inizia con | Prime lettere di corrispondenza delle stringhe |
| non inizia con | Le prime lettere della stringa NON corrispondono |
| contiene | Qualsiasi lettera insieme nella corrispondenza stringa (esempio: california, fortuna, quindi) |
| non contiene | Nessuna corrispondenza nella corrispondenza stringa. (al contrario di &quot;contiene&quot;) |
| è vuoto | Record senza valore (NULL) |
| non è vuoto | Record con valore ANY |

>[!TIP]
>
>Utilizzare gli operatori positivi rispetto a quelli negativi. I filtri &quot;Non è&quot; devono cercare l’intero set di dati nell’istanza, il che può richiedere molto tempo. I filtri &quot;is&quot; positivi possono sfruttare algoritmi di ricerca più efficaci.

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
   <td colspan="1" rowspan="1">Corrispondenza numero esatta ( = 0 restituisce entrambi i lead con 0 <em>e</em> NULL)</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">non</td> 
   <td colspan="1" rowspan="1">Qualsiasi valore tranne la corrispondenza esatta del numero</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">tra</td> 
   <td colspan="1" rowspan="1">Definisci due valori per trovare tutti nel mezzo (incluso)</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">maggiore di</td> 
   <td colspan="1" rowspan="1">Sopra il</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">inferiore a</td> 
   <td colspan="1" rowspan="1">Minore del valore specificato</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">almeno</td> 
   <td colspan="1" rowspan="1">Sopra il specificato (incluso)</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">al massimo</td> 
   <td colspan="1" rowspan="1">Minore del valore specificato (incluso)</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">è vuoto</td> 
   <td colspan="1" rowspan="1">Record senza valore (NULL) - zero è un numero, ma è <em>not</em> NULL</td> 
  </tr> 
  <tr> 
   <td colspan="1" rowspan="1">non è vuoto</td> 
   <td colspan="1" rowspan="1">Record con valore ANY (incluso zero)</td> 
  </tr> 
 </tbody> 
</table>

Come potete vedere, questi operatori rendono facile parlare Marketo-ese con fluenza!
