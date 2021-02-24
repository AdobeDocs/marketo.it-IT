---
unique-page-id: 7514126
description: Attribuzione Esempio 1 - Documenti Marketo - Documentazione prodotto
title: Esempio di attribuzione 1
translation-type: tm+mt
source-git-commit: fa4ab03b98ac922e10c6daf3647dc460c12244d3
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 0%

---


# Esempio di attribuzione 1 {#attribution-example}

Leggere lo scenario seguente e cercare di determinare i numeri che dovrebbero essere nella griglia.

* 11 aprile | Fred è acquisito da (Tradeshow)
* 15 aprile | Partecipanti Margo (webinar) - successo
* 22 aprile | Fred è associato (ruolo) all&#39;opportunità
* 22 aprile | L&#39;opportunità viene creata per $3.000

| Nome programma | (Presentazione) | (webinar) |
|---|---|---|
| (FT) Opzione creata | `<pre>1</pre>` | `<pre>0</pre>` |
| (FT) Pipeline creata | `<pre>$3,000</pre>` | `<pre>$0</pre>` |
| (FT) Opty Won | `<pre>0</pre>` | `<pre>0</pre>` |
| (FT) Entrate vinte | `<pre>0</pre>` | `<pre>0</pre>` |

**Mostra risposte**

>[!NOTE]
>
>**Spiegazione**
>
>Primo, capire che alcuni tipi sono CONTI e altri sono VALUTA. L&#39;opzione Creato è un conteggio, un numero intero. La tubazione è una valuta. In Marketo, la valuta sarà conforme alle impostazioni internazionali dell&#39;amministratore.
>
>Il motivo per cui il Salone ha ricevuto tutti i crediti è perché Margo non era associato a un ruolo nell&#39;opportunità. Nessun ruolo, nessun credito.

>[!NOTE]
>
>**Regole di attribuzione**
>
>1. Il credito è suddiviso in modo uniforme
>1. Non puoi dare più credito di quanto hai guadagnato
>1. Non si può dare credito a qualcosa che è successo in passato


Prova tutti gli esempi e sarai un professionista di attribuzione!

>[!MORELIKETHIS]
>
>* [Attribuzione Esempio 2](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-2.md)
>* [Esempio di attribuzione 3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)
>* [Esempio di attribuzione 4](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)

