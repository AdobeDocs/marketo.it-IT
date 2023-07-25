---
unique-page-id: 7514146
description: Esempio di attribuzione 2 - Documentazione di Marketo - Documentazione del prodotto
title: Esempio di attribuzione 2
exl-id: 8f00abb5-85f8-4f05-874e-57aa6442548c
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 0%

---

# Esempio di attribuzione 2 {#attribution-example}

Leggi lo scenario seguente e prova a determinare i numeri che devono essere presenti nella griglia.

* 11 aprile | Fatturazione acquisita da (fiera)
* Aprile 15 | Giovanna è acquisita da (webinar)
* Aprile 22 | (Opportunità 1) creato per 6.000 dollari
* Aprile 24 | (Opportunità 2) creato per $ 10.000
* Aprile 25 | Bill e Joan sono associati a ruoli **ENTRAMBI** Opti
* Aprile 29 | (Opportunità 1) è un&#39;opportunità acquisita

| Nome del programma | (fiera) | (Webinar) |
|---|---|---|
| (FT) Opzione creata | `<pre>1</pre>` | `<pre>1</pre>` |
| Pipeline (FT) creata | `<pre>$8,000</pre>` | `<pre>$8,000</pre>` |
| (FT) Opty Won | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (FT) Entrate realizzate | `<pre>$3,000</pre>` | `<pre>$3,000</pre>` |

**Mostra risposte**

>[!NOTE]
>
>**Spiegazione**
>
>Perché sia Bill che Joan erano associati a ruoli **ENTRAMBI** opportunità, il sistema (secondo le regole) ripartisce il credito in modo uniforme tra loro.
>
>La pipeline creata per ciascun programma (8.000 dollari) è la metà del totale (16.000 dollari) disponibile da attribuire come credito.

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
>* [Esempio di attribuzione 3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)
>* [Esempio di attribuzione 4](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)
