---
unique-page-id: 7514146
description: Attribuzione Esempio 2 - Documenti Marketo - Documentazione prodotto
title: Attribuzione Esempio 2
translation-type: tm+mt
source-git-commit: fa4ab03b98ac922e10c6daf3647dc460c12244d3
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 0%

---


# Esempio di attribuzione 2 {#attribution-example}

Leggere lo scenario seguente e cercare di determinare i numeri che dovrebbero essere nella griglia.

* 11 aprile | Fattura acquisita da (Sala commerciale)
* 15 aprile | Joan è acquisita da (Webinar)
* 22 aprile | (Opportunità 1) creata per $6.000
* 24 aprile | (Opportunità 2) creata per $10.000
* 25 aprile | Bill e Joan sono associati ai ruoli per **BOTH** Optys
* 29 aprile | (Opportunità 1) chiusa

| Nome programma | (Presentazione) | (webinar) |
|---|---|---|
| (FT) Opzione creata | `<pre>1</pre>` | `<pre>1</pre>` |
| (FT) Pipeline creata | `<pre>$8,000</pre>` | `<pre>$8,000</pre>` |
| (FT) Opty Won | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (FT) Entrate vinte | `<pre>$3,000</pre>` | `<pre>$3,000</pre>` |

**Mostra risposte**

>[!NOTE]
>
>**Spiegazione**
>
>Poiché sia Bill che Joan erano associati ai ruoli per le opportunità **BOTH**, il sistema (secondo le regole) suddivide il credito in modo uniforme tra di loro.
>
>La pipeline creata per ciascun programma ($8.000) è la metà del totale ($16.000) disponibile per il credito.

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
>* [Esempio di attribuzione 3](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-3.md)
>* [Esempio di attribuzione 4](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-tools/attribution/attribution-example-4.md)

