---
unique-page-id: 11373011
description: Transizione all’Editor e-mail 2.0 - Documentazione di Marketo - Documentazione del prodotto
title: Transizione all’editor e-mail 2.0
exl-id: eb9ec8cc-d6e8-4839-a4d9-608d2f264cbb
hide: true
hidefromtoc: true
feature: Email Editor
source-git-commit: b3bc6a7ec14a513e4b294852d066f9e3d0f74ef8
workflow-type: tm+mt
source-wordcount: '642'
ht-degree: 0%

---

# Transizione all’editor e-mail 2.0 {#transitioning-to-email-editor}

A partire dalla versione del 19 giugno, tutti gli abbonamenti Marketo sono stati trasferiti a Email Editor 2.0. [Ulteriori informazioni](https://nation.marketo.com/docs/DOC-7038) sulla rimozione di Email Editor 1.0.

Le e-mail e i modelli e-mail all’interno dell’abbonamento devono avere un numero di versione. La versione si trova nella pagina di riepilogo della risorsa.

![](assets/five-5.png)

Per impostazione predefinita, tutte le e-mail e i modelli e-mail esistenti saranno contrassegnati come v1.0 se sono stati creati prima della versione della primavera 2016 o dopo la versione quando Editor e-mail 2.0 è disabilitato. Con l’Editor e-mail 2.0 ora abilitato automaticamente, viene visualizzato il seguente comportamento:

* Quando crei una nuova e-mail, verrà visualizzato il [Selettore modello e-mail](email-template-picker-overview.md) e potrai scegliere un modello e-mail v2.0.
* Ogni volta che crei o modifichi un&#39;e-mail con Editor e-mail 2.0, l&#39;e-mail risultante **sarà sempre** contrassegnata come v2.0 (anche se hai utilizzato un modello e-mail v1.0).

Se la tua sottoscrizione include e-mail v1.0 prima del passaggio a Editor e-mail 2.0, osserverai il seguente comportamento in base allo stato corrente della risorsa:

**Approvato** - Facendo clic su &quot;Modifica bozza&quot; verrà creata una bozza v2.0 dell&#39;e-mail approvata. Se poi approvi la bozza v2.0, lo stato approvato dell’e-mail diventa v2.0 e non è possibile tornare alla v1.0.\
**Bozza** - Facendo clic su &quot;Modifica bozza&quot;, la bozza verrà contrassegnata automaticamente come v2.0. A questo punto, non sarà possibile eliminare e ripristinare la versione 1.0 perché non esiste una versione approvata della risorsa.
**Approvato con bozza** - Facendo clic su &quot;Modifica bozza&quot;, la bozza verrà automaticamente contrassegnata come v2.0. Per questo motivo, non è possibile ripristinare la bozza alla versione 1.0.

Se il tuo abbonamento dispone di modelli e-mail v1.0 prima del passaggio a Editor e-mail 2.0, si verificherà il seguente comportamento:

**Approvato** - Facendo clic su &quot;Modifica bozza&quot; verrà creata una bozza v2.0 del modello e-mail esistente.
**Bozza** - Facendo clic su &quot;Modifica bozza&quot;, la bozza verrà contrassegnata automaticamente come v2.0. A questo punto, non sarebbe possibile ignorare e ripristinare la versione 1.0 perché non esiste una versione approvata della risorsa.
**Approvato con bozza** - Facendo clic su &quot;Modifica bozza&quot;, la bozza verrà contrassegnata automaticamente come v2.0. Per questo motivo, non è possibile ripristinare la bozza alla versione 1.0.

Se approvi un modello e-mail che in precedenza era v1.0 (in uno qualsiasi degli stati di cui sopra), visualizzerai il seguente comportamento:

Per le e-mail v1.0 esistenti che utilizzavano il modello (in precedenza v1.0):\
**E-mail v1.0 approvata** - Per questa e-mail verrà creata una bozza v2.0, che utilizza ancora il modello v2.0 appena approvato. Riceverà anche eventuali modifiche al modello.\
**E-mail bozza v1.0** - La bozza rimarrà v1.0 fino a quando non farai clic su &quot;Modifica bozza&quot;. Successivamente, verrà automaticamente contrassegnata come v2.0 e riceverà eventuali modifiche al modello.\
**Approvato con bozza e-mail v1.0** - La bozza rimarrà v1.0 fino a quando non si fa clic su &quot;Modifica bozza&quot;. Successivamente, verrà automaticamente contrassegnata come v2.0 e riceverà eventuali modifiche al modello.

Per le e-mail v2.0 esistenti che utilizzavano il modello (in precedenza v1.0):\
**E-mail v2.0 approvata** - Per questa e-mail verrà creata una bozza v2.0, che &quot;utilizza&quot; ancora il modello appena approvato, e riceverà eventuali modifiche al modello.\
**E-mail bozza v2.0** - La bozza rimarrà invariata (v2.0) e riceverà eventuali modifiche al modello.\
**Approvato con bozza e-mail v2.0** - La bozza rimarrà invariata (v2.0) e riceverà eventuali modifiche al modello.

>[!CAUTION]
>
>Se hai mai approvato la bozza v2.0 di un modello e-mail v1.0, il modello diventerà v2.0. **impossibile** ripristinarla alla versione 1.0.

Aspetti da considerare

* Le e-mail approvate sono **mai** modificate.

* I modelli e-mail approvati sono **mai** modificati.

* In alcuni **rari** casi, non è possibile aprire un&#39;e-mail v1.0 in Editor e-mail 2.0. In tal caso, scartare la bozza e contattare il supporto tecnico Marketo.

>[!MORELIKETHIS]
>
>* [Panoramica di Editor e-mail 2.0](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md)
>* [Sintassi modello e-mail](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md)
