---
unique-page-id: 7514126
description: Esempio di attribuzione 1 - Documentazione di Marketo - Documentazione del prodotto
title: Esempio di attribuzione 1
exl-id: 851cbad3-0f6d-4ea0-857f-8b15337c7540
feature: Reporting, Revenue Cycle Analytics
source-git-commit: d20a9bb584f69282eefae3704ce4be2179b29d0b
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 0%

---

# Esempio di attribuzione 1 {#attribution-example}

Leggi lo scenario seguente e prova a determinare i numeri che devono essere presenti nella griglia.

* 11 aprile | Fred è acquisita da (fiera)
* Aprile 15 | Partecipazione a Margo (webinar) - operazione riuscita
* Aprile 22 | Fred è associato (ruolo) all’opportunità
* Aprile 22 | Opportunità creata per 3.000 dollari

| Nome del programma | (fiera) | (Webinar) |
|---|---|---|
| (FT) Opzione creata | `<pre>1</pre>` | `<pre>0</pre>` |
| Pipeline (FT) creata | `<pre>$3,000</pre>` | `<pre>$0</pre>` |
| (FT) Opty Won | `<pre>0</pre>` | `<pre>0</pre>` |
| (FT) Entrate realizzate | `<pre>0</pre>` | `<pre>0</pre>` |

**Mostra risposte**

>[!NOTE]
>
>**Spiegazione**
>
>Il primo è capire che alcuni tipi sono CONTEGGI e altri sono VALUTA. L&#39;opzione creata è un conteggio, un numero intero. La pipeline è una valuta. In Marketo, la valuta sarà conforme alle impostazioni locali dell&#39;amministratore.
>
>Il motivo per cui il Tradeshow ha ricevuto tutto il merito è perché Margo non era associato a un ruolo nell&#39;opportunità. Nessun ruolo, nessun credito.

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
>* [Esempio di attribuzione 2](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-2.md)
>* [Esempio di attribuzione 3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)
>* [Esempio di attribuzione 4](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)
