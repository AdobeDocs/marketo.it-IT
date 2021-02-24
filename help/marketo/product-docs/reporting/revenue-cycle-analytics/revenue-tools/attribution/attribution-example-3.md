---
unique-page-id: 7514149
description: Attribuzione Esempio 3 - Documenti Marketo - Documentazione prodotto
title: Esempio di attribuzione 3
translation-type: tm+mt
source-git-commit: fa4ab03b98ac922e10c6daf3647dc460c12244d3
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 0%

---


# Esempio di attribuzione 3 {#attribution-example}

Leggere lo scenario seguente e cercare di determinare i numeri che dovrebbero essere nella griglia.

* 11 aprile | Download Steve (contenuto) - successo
* 22 aprile | L&#39;opportunità è stata creata per $3,000 (sia Steve che Jason hanno ruoli)
* 25 aprile | Jason partecipa (Webinar) - successo
* 30 aprile | Opportunità chiusa

| Metrica attribuzione | (Contenuto) | (webinar) |
|---|---|---|
| (MT) Opzione creata | `<pre>1</pre>` | `<pre>0</pre>` |
| (MT) Pipeline creata | `<pre>$3,000</pre>` | `<pre>$0</pre>` |
| (MT) Opty Won | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (MT) Entrate vinte | `<pre>$1,500</pre>` | `<pre>$1,500</pre>` |

**Mostra risposte**

>[!NOTE]
>
>**Spiegazione**
>
>Ricorda regola di attribuzione n. 3. Jason ha avuto il successo del programma DOPO la possibilità è stata creata. Pertanto, il webinar non può ottenere credito per la creazione dell&#39;opportunità. Ha vinto solo il merito per l&#39;Opty.
>
>Pertanto (Contenuto) ha il 100% del credito per la creazione e la pipeline di Opty, ma solo il 50% del credito per la società ha vinto.

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
>* [Esempio di attribuzione 1](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-1.md)
>* [Attribuzione Esempio 2](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-2.md)
>* [Esempio di attribuzione 4](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)

