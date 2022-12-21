---
unique-page-id: 7514151
description: Attribution Example 4 - Documentazione Marketo - Documentazione del prodotto
title: Attribution, esempio 4
exl-id: 98cd7401-3bc7-40a1-b88d-7174a3027d4e
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 0%

---

# Attribution, esempio 4 {#attribution-example}

Leggere lo scenario seguente e cercare di determinare i numeri che dovrebbero essere nella griglia.

* 11 aprile | E-Book scaricabile da Michelle (Contenuto) - Successo
* 15 aprile | Partecipa John (Webinar) - Successo
* 22 aprile | (Opportunità 1) creata per $3.000
* 24 aprile | (Opportunità 2) creata per $5.000
* 25 aprile | John e Michelle sono associati a **entrambi** Ottici
* 29 aprile | [Opt 1] è chiuso

| Nome del programma | (Contenuto) | (Webinar) |
|---|---|---|
|  | (Opty 1) | (Opty 2) | (Opty 1) | (Opty 2) |
| (MT) Opty Created | `<pre>0.5</pre>` | `<pre>0.5</pre>` | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (MT) Pipeline creata | `<pre>$1,500</pre>` | `<pre>$2,500</pre>` | `<pre>$1,500</pre>` | `<pre>$2,500</pre>` |
| (MT) Vincita | `<pre>0.5</pre>` | `<pre>0</pre>` | `<pre>0.5</pre>` | `<pre>0</pre>` |
| (MT) Entrate vinte | `<pre>$1,500</pre>` | `<pre>$0</pre>` | `<pre>$1,500</pre>` | `<pre>$0</pre>` |

**Mostra risposte**

>[!NOTE]
>
>**Spiegazione**
>
>Quando si hanno più opportunità e più persone con successo del programma, è necessario dividere il credito tra le persone e i programmi. Tuttavia, si noti che il credito per le opportunità 1 e 2 non è combinato. Ciascuna è una distinta valutazione del credito.
>
>Quando sono coinvolte più persone, Marketo calcola automaticamente le frazioni di un&#39;opportunità per dare credito.

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
>* [Attribution, esempio 2](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-2.md)
>* [Attribution, esempio 3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)

