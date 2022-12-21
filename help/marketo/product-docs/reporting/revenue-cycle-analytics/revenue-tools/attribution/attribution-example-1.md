---
unique-page-id: 7514126
description: Attribution Example 1 - Documentazione Marketo - Documentazione del prodotto
title: Attribution, esempio 1
exl-id: 851cbad3-0f6d-4ea0-857f-8b15337c7540
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 0%

---

# Attribution, esempio 1 {#attribution-example}

Leggere lo scenario seguente e cercare di determinare i numeri che dovrebbero essere nella griglia.

* 11 aprile | Fred è acquisito da (Tradeshow)
* 15 aprile | Margo partecipa (Webinar) - successo
* 22 aprile | Fred è associato (ruolo) all&#39;opportunità
* 22 aprile | L&#39;opportunità viene creata per $3.000

| Nome del programma | (Presentazione) | (Webinar) |
|---|---|---|
| (FT) Opty Created | `<pre>1</pre>` | `<pre>0</pre>` |
| (FT) Pipeline creata | `<pre>$3,000</pre>` | `<pre>$0</pre>` |
| (FT) Opty Won | `<pre>0</pre>` | `<pre>0</pre>` |
| (FT) Entrate vinte | `<pre>0</pre>` | `<pre>0</pre>` |

**Mostra risposte**

>[!NOTE]
>
>**Spiegazione**
>
>Primo, capire che alcuni tipi sono CONTI e altri sono VALUTA. Opty Created è un conteggio, un numero intero. La pipeline è una valuta. In Marketo, la valuta sarà conforme alle impostazioni internazionali dell&#39;amministratore.
>
>Il motivo per cui il Tradeshow ha ricevuto tutto il credito è perché Margo non era associato a un ruolo nell&#39;opportunità. Nessun ruolo, nessun credito.

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
>* [Attribution, esempio 2](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-2.md)
>* [Attribution, esempio 3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)
>* [Attribution, esempio 4](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)

