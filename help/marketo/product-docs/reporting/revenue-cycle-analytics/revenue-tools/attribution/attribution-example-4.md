---
unique-page-id: 7514151
description: Attribuzione Esempio 4 - Documenti Marketo - Documentazione prodotto
title: Esempio di attribuzione 4
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 0%

---


# Esempio di attribuzione 4 {#attribution-example}

Leggere lo scenario seguente e cercare di determinare i numeri che dovrebbero essere nella griglia.

* 11 aprile | E-Book con download Michelle (contenuto) - Successo
* 15 aprile | John frequenta (webinar) - Successo
* 22 aprile | (Opportunità 1) creata per $3.000
* 24 aprile | (Opportunità 2) creata per $5.000
* 25 aprile | John e Michelle sono associati a **sia** Optys
* 29 aprile | [Opty 1] è chiuso

| Nome programma | (Contenuto) | (webinar) |
|---|---|---|
|  | (Opty 1) | (Opty 2) | (Opty 1) | (Opty 2) |
| (MT) Opzione creata | `<pre>0.5</pre>` | `<pre>0.5</pre>` | `<pre>0.5</pre>` | `<pre>0.5</pre>` |
| (MT) Pipeline creata | `<pre>$1,500</pre>` | `<pre>$2,500</pre>` | `<pre>$1,500</pre>` | `<pre>$2,500</pre>` |
| (MT) Opty Won | `<pre>0.5</pre>` | `<pre>0</pre>` | `<pre>0.5</pre>` | `<pre>0</pre>` |
| (MT) Entrate vinte | `<pre>$1,500</pre>` | `<pre>$0</pre>` | `<pre>$1,500</pre>` | `<pre>$0</pre>` |

**Mostra risposte**

>[!NOTE]
>
>**Spiegazione**
>
>Quando si hanno più opportunità e più persone con successo del programma, è necessario ripartire il credito tra le persone e i programmi. Tuttavia, si noti che il credito per l&#39;opportunità 1 e 2 non è combinato. Ciascuna è una distinta valutazione del credito.
>
>Quando molte persone sono coinvolte, Marketo calcolerà automaticamente le frazioni di un&#39;opportunità per dare credito.

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

>[!MORELIKETHIS]
>
>* [Esempio di attribuzione 1](attribution-example-1.md)
>* [Attribuzione Esempio 2](attribution-example-2.md)
>* [Esempio di attribuzione 3](attribution-example-3.md)

