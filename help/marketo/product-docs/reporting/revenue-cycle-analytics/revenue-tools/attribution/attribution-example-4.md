---
unique-page-id: 7514151
description: Esempio di attribuzione 4 - Documentazione di Marketo - Documentazione del prodotto
title: Esempio di attribuzione 4
exl-id: 98cd7401-3bc7-40a1-b88d-7174a3027d4e
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 0%

---

# Esempio di attribuzione 4 {#attribution-example}

Leggi lo scenario seguente e prova a determinare i numeri che devono essere presenti nella griglia.

* 11 aprile | Michelle scarica l&#39;e-Book (Contenuto) - Successo
* Aprile 15 | John partecipa (webinar) - Operazione riuscita
* Aprile 22 | (Opportunità 1) creato per $ 3.000
* Aprile 24 | (Opportunità 2) creato per $5.000
* Aprile 25 | John e Michelle sono associati a **entrambi** Opti
* Aprile 29 | [Opzione 1] è Closed-Won

| Nome del programma | (Contenuto) | (Webinar) |
|---|---|---|
|   | (Opzione 1) | (Opzione 2) | (Opzione 1) | (Opzione 2) |
| (MT) Opty creato | `<pre>0.5</pre>` | `<pre>0.5</pre>` | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (MT) Pipeline creata | `<pre>$1,500</pre>` | `<pre>$2,500</pre>` | `<pre>$1,500</pre>` | `<pre>$2,500</pre>` |
| (MT) Opty Won | `<pre>0.5</pre>` | `<pre>0</pre>` | `<pre>0.5</pre>` | `<pre>0</pre>` |
| (MT) Entrate realizzate | `<pre>$1,500</pre>` | `<pre>$0</pre>` | `<pre>$1,500</pre>` | `<pre>$0</pre>` |

**Mostra risposte**

>[!NOTE]
>
>**Spiegazione**
>
>Quando si hanno più opportunità e più persone con successo del programma, è necessario dividere il credito tra le persone e i programmi. Tuttavia, si noti che il credito per l&#39;opportunità 1 e 2 non sono combinati. Ciascuno di essi è una valutazione del merito di credito distinta.
>
>Quando sono coinvolte più persone, Marketo calcolerà automaticamente le frazioni di un&#39;opportunità di dare credito per.

>[!NOTE]
>
>**Regole di attribuzione**
>
>1. Il credito viene suddiviso in modo uniforme
>1. Non puoi dare più credito di quello che hai guadagnato
>1. Non puoi dare credito a qualcosa che è successo nel passato

Prova tutti gli esempi e sarai un professionista dell’attribuzione.

>[!MORELIKETHIS]
>
>* [Esempio di attribuzione 1](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-1.md)
>* [Esempio di attribuzione 2](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-2.md)
>* [Esempio di attribuzione 3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)
