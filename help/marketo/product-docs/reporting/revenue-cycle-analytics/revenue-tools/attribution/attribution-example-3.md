---
unique-page-id: 7514149
description: Attribution Example 3 - Documentazione Marketo - Documentazione del prodotto
title: Attribution, esempio 3
exl-id: d8ca63a2-58de-4cde-b915-ff7f2e6468d9
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 0%

---

# Attribution, esempio 3 {#attribution-example}

Leggere lo scenario seguente e cercare di determinare i numeri che dovrebbero essere nella griglia.

* 11 aprile | Download Steve (contenuto) - successo
* 22 aprile | L&#39;opportunità è creata per $3.000 (Sia Steve che Jason hanno ruoli)
* 25 aprile | Jason partecipa (Webinar) - successo
* 30 aprile | Opportunità chiusa

| Metrica di attribuzione | (Contenuto) | (Webinar) |
|---|---|---|
| (MT) Opty Created | `<pre>1</pre>` | `<pre>0</pre>` |
| (MT) Pipeline creata | `<pre>$3,000</pre>` | `<pre>$0</pre>` |
| (MT) Vincita | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (MT) Entrate vinte | `<pre>$1,500</pre>` | `<pre>$1,500</pre>` |

**Mostra risposte**

>[!NOTE]
>
>**Spiegazione**
>
>Ricorda la regola di attribuzione n. 3. Jason ha avuto successo di programma DOPO la creazione della povertà. Pertanto, il webinar non può ottenere credito per la creazione dell&#39;opportunità. Ha vinto solo il credito per l&#39;Opty.
>
>Pertanto, (Contenuto) ha ottenuto il 100% del credito per la creazione e la pipeline di Opty, ma solo il 50% del credito per la partecipazione ha vinto.

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
>* [Attribution, esempio 4](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)

