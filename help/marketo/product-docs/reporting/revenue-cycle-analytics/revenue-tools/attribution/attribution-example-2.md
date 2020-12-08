---
unique-page-id: 7514146
description: Attribuzione Esempio 2 - Documenti Marketo - Documentazione prodotto
title: Attribuzione Esempio 2
translation-type: tm+mt
source-git-commit: 1a29614ec938074902af201b2ffc11cfaa625f7a
workflow-type: tm+mt
source-wordcount: '164'
ht-degree: 0%

---


# Attribuzione Esempio 2 {#attribution-example}

Leggere lo scenario seguente e cercare di determinare i numeri che dovrebbero essere nella griglia.

* 11 aprile | Fattura acquisita da (Sala commerciale)
* 15 aprile | Joan è acquisita da (Webinar)
* 22 aprile | (Opportunità 1) creata per $6.000
* 24 aprile | (Opportunità 2) creata per $10.000
* 25 aprile | Bill e Joan sono associati con i ruoli a **BOTH **Optys
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
>Dato che sia Bill che Joan erano associati con ruoli a **BOTH **opportunità, il sistema (secondo le regole) ha suddiviso il credito in modo uniforme tra loro.
>
>La pipeline creata per ciascun programma ($8.000) è la metà del totale ($16.000) disponibile per il credito.

>[!NOTE]
>
>**Regole di attribuzione**
>
>1. Il credito è suddiviso in modo uniforme
>1. Non puoi dare più credito di quanto hai guadagnato
>1. Non si può dare credito a qualcosa che è successo in passato

>



<br> 

Prova tutti gli esempi e sarai un professionista di attribuzione!

>[!NOTE]
>
>**Articoli correlati**
>
>* [Esempio di attribuzione 1](attribution-example-1.md)
>* [Esempio di attribuzione 3](attribution-example-3.md)
>* [Esempio di attribuzione 4](attribution-example-4.md)

