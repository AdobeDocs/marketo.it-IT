---
unique-page-id: 7514149
description: Esempio di attribuzione 3 - Documentazione di Marketo - Documentazione del prodotto
title: Esempio di attribuzione 3
exl-id: d8ca63a2-58de-4cde-b915-ff7f2e6468d9
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 0%

---

# Esempio di attribuzione 3 {#attribution-example}

Leggi lo scenario seguente e prova a determinare i numeri che devono essere presenti nella griglia.

* 11 aprile | Download di Steve (contenuto) - operazione riuscita
* Aprile 22 | L’opportunità è stata creata per 3.000 dollari (sia Steve che Jason hanno un ruolo)
* Aprile 25 | Jason partecipa (webinar) - operazione riuscita
* Aprile 30 | Opportunità chiusa

| Metrica di attribuzione | (Contenuto) | (Webinar) |
|---|---|---|
| (MT) Opty creato | `<pre>1</pre>` | `<pre>0</pre>` |
| (MT) Pipeline creata | `<pre>$3,000</pre>` | `<pre>$0</pre>` |
| (MT) Opty Won | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (MT) Entrate realizzate | `<pre>$1,500</pre>` | `<pre>$1,500</pre>` |

**Mostra risposte**

>[!NOTE]
>
>**Spiegazione**
>
>Ricorda #3. regola di attribuzione Jason ha avuto successo nel programma DOPO la creazione dell’opzione. Pertanto, al webinar non viene attribuito il merito per la creazione dell’opportunità. Solo il merito per l&#39;opzione vinta.
>
>Pertanto, (Contenuto) ha il 100% di credito per la creazione e la pipeline dell’opzione, ma solo il 50% di credito per l’opzione vinta.

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
>* [Esempio di attribuzione 4](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)
