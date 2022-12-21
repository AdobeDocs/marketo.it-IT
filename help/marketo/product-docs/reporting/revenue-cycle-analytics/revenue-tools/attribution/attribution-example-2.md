---
unique-page-id: 7514146
description: Attribution Example 2 - Documentazione Marketo - Documentazione del prodotto
title: Attribution, esempio 2
exl-id: 8f00abb5-85f8-4f05-874e-57aa6442548c
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 0%

---

# Attribution, esempio 2 {#attribution-example}

Leggere lo scenario seguente e cercare di determinare i numeri che dovrebbero essere nella griglia.

* 11 aprile | Bill è acquisito da (Tradeshow)
* 15 aprile | Joan è acquisita da (Webinar)
* 22 aprile | (Opportunità 1) creata per $6.000
* 24 aprile | (Opportunità 2) creata per $ 10.000
* 25 aprile | Bill e Joan sono associati ai ruoli **ENTRAMBI** Ottici
* 29 aprile | (Opportunità 1) è chiuso

| Nome del programma | (Presentazione) | (Webinar) |
|---|---|---|
| (FT) Opty Created | `<pre>1</pre>` | `<pre>1</pre>` |
| (FT) Pipeline creata | `<pre>$8,000</pre>` | `<pre>$8,000</pre>` |
| (FT) Opty Won | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (FT) Entrate vinte | `<pre>$3,000</pre>` | `<pre>$3,000</pre>` |

**Mostra risposte**

>[!NOTE]
>
>**Spiegazione**
>
>Perché sia Bill che Joan sono stati associati a ruoli **ENTRAMBI** le opportunità, il sistema (secondo le regole) suddivide il credito in modo uniforme tra loro.
>
>La pipeline creata per ciascun programma ($8.000) è la metà del totale ($16.000) disponibile per il credito.

>[!NOTE]
>
>**Regole di attribuzione**
>
>1. Il credito è suddiviso in modo uniforme
>1. Non puoi dare più credito di quanto guadagnato
>1. Non puoi dare credito a qualcosa che è successo in passato


Prova tutti gli esempi e sarai un professionista di attribuzione!

>[!MORELIKETHIS]
>
>* [Attribution, esempio 1](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-1.md)
>* [Attribution, esempio 3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)
>* [Attribution, esempio 4](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)

