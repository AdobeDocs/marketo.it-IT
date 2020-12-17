---
unique-page-id: 11373011
description: Passaggio all'editor di posta elettronica 2.0 - Documenti Marketo - Documentazione prodotto
title: Passaggio all'editor di posta elettronica 2.0
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 0%

---


# Passaggio all&#39;editor di posta elettronica 2.0 {#transitioning-to-email-editor}

A partire dalla [versione del 19 giugno 2019](../../../../release-notes/2016/release-notes-spring-16.md), tutte le iscrizioni a Marketo sono state trasferite a Editor e-mail 2.0. [Per saperne di più](https://nation.marketo.com/docs/DOC-7038) sull&#39;eliminazione di Email Editor 1.0.

Le e-mail e i modelli e-mail all&#39;interno dell&#39;iscrizione devono avere un numero di versione. La versione è disponibile nella pagina di riepilogo della risorsa.

![](assets/five-5.png)

Per impostazione predefinita, tutti i modelli esistenti di e-mail e e e-mail saranno contrassegnati come v1.0 se creati prima della release primaverile del 16 o dopo la release in cui Editor e-mail 2.0 è disabilitato. Con l&#39;Editor e-mail 2.0 ora abilitato automaticamente, si verificherà il seguente comportamento:

* Quando create un nuovo messaggio e-mail, viene visualizzato il [Selettore modello e-mail](email-template-picker-overview.md) e potrete scegliere un modello e-mail v2.0.
* Ogni volta che create o modificate un&#39;e-mail con Editor e-mail 2.0, l&#39;e-mail visualizzata sarà sempre **sempre** contrassegnata come v2.0 (anche se avete utilizzato un modello e-mail v1.0).

Se l’iscrizione contiene e-mail con v1.0 prima del passaggio a Editor e-mail 2.0, il comportamento dell’utente sarà il seguente in base allo stato corrente della risorsa:

**Approvato** - Facendo clic su &quot;Modifica bozza&quot; verrà creata una bozza v2.0 dell&#39;e-mail approvata. Se quindi approvate la bozza v2.0, lo stato approvato dell&#39;e-mail diventa v2.0 e non c&#39;è modo di ripristinare la versione 1.0.\
**Bozza** : facendo clic su &quot;Modifica bozza&quot; la bozza viene contrassegnata automaticamente come v2.0. A questo punto, non sarà possibile eliminare e ripristinare la versione 1.0 perché non è disponibile una versione approvata della risorsa.\
**Approvato con bozza** - Facendo clic su &quot;Modifica bozza&quot; la bozza viene contrassegnata automaticamente come v2.0. Per questo motivo, non è possibile ripristinare la bozza a v1.0.

Se l’iscrizione include modelli e-mail v1.0 prima del passaggio a Editor e-mail 2.0, si verificherà il seguente comportamento:

**Approvato** - Facendo clic su &quot;Modifica bozza&quot; verrà creata una bozza v2.0 del modello e-mail esistente.\
**Bozza** : facendo clic su &quot;Modifica bozza&quot; la bozza viene contrassegnata automaticamente come v2.0. A questo punto, non sarebbe possibile eliminare e ripristinare la versione 1.0 perché non esiste una versione approvata della risorsa.\
**Approvato con bozza** - Facendo clic su &quot;Modifica bozza&quot; la bozza viene contrassegnata automaticamente come v2.0. Per questo motivo, non è possibile ripristinare la bozza a v1.0.

Se approvate un modello e-mail che era già v1.0 (in uno degli stati precedenti), verrà visualizzato il seguente comportamento:

Per le e-mail v1.0 esistenti che utilizzavano il modello (in precedenza v1.0):\
**Messaggio e-mail**  v1.0 approvato - Per questo messaggio e-mail verrà creata una bozza A v2.0, sempre utilizzando il modello v2.0 approvato di recente. Inoltre, verranno apportate eventuali modifiche al modello.\
**Bozza e-mail**  v1.0: la bozza rimarrà v1.0 finché non si fa clic su &quot;Edit Draft&quot; (Modifica bozza). Successivamente, verrà automaticamente contrassegnato come v2.0 e riceverà eventuali modifiche apportate al modello.\
**Approvato con bozza v1.0 e-mail** - La bozza rimarrà v1.0 finché non si fa clic su &quot;Edit Draft&quot; (Modifica bozza). Successivamente, verrà automaticamente contrassegnato come v2.0 e riceverà eventuali modifiche apportate al modello.

Per le e-mail v2.0 esistenti che utilizzavano il modello (v1.0 in precedenza):\
**Messaggio e-mail**  v2.0 approvato: per questo messaggio e-mail verrà creata una bozza A v2.0, che continua a &quot;utilizzare&quot; il modello appena approvato e che riceverà eventuali modifiche al modello.\
**Bozza e-mail**  v2.0: la bozza rimarrà invariata (v2.0) e riceverà eventuali modifiche al modello.\
**Approvato con bozza v2.0 e-mail**  - La bozza rimarrà invariata (v2.0) e riceverà eventuali modifiche al modello.

>[!CAUTION]
>
>Se approvate la bozza v2.0 di un modello e-mail v1.0, il modello diventerà v2.0. **nessun modo** per ripristinarlo a v1.0.

Cose da notare

* Le e-mail approvate vengono **mai** modificate.

* I modelli e-mail approvati sono **mai** modificati.

* In alcuni casi **rari**, non è possibile aprire un&#39;e-mail v1.0 in Editor e-mail 2.0. In tal caso, eliminate la bozza e contattate il supporto di Marketo.

>[!MORELIKETHIS]
>
>* [Panoramica di Email Editor 2.0](email-editor-v2-0-overview.md)
>* [Sintassi modello e-mail](email-template-syntax.md)

>



