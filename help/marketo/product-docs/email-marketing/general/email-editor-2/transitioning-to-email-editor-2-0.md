---
unique-page-id: 11373011
description: Transizione all’editor di e-mail 2.0 - Documenti Marketo - Documentazione del prodotto
title: Transizione all’editor di e-mail 2.0
exl-id: eb9ec8cc-d6e8-4839-a4d9-608d2f264cbb
source-git-commit: 64ff6900a761b9df796a9a7f417cca1ddc628cce
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 0%

---

# Transizione all’editor di e-mail 2.0 {#transitioning-to-email-editor}

A partire dalla versione del 19 giugno, tutte le iscrizioni Marketo sono state trasferite a Email Editor 2.0. [Ulteriori informazioni](https://nation.marketo.com/docs/DOC-7038) sulla rimozione di Email Editor 1.0.

Le e-mail e i modelli e-mail all’interno dell’abbonamento devono avere un numero di versione. La versione è disponibile nella pagina di riepilogo della risorsa.

![](assets/five-5.png)

Per impostazione predefinita, tutte le e-mail e i modelli di e-mail esistenti saranno contrassegnati come v1.0 se sono stati creati prima della versione primaverile del 16 o dopo la release quando Email Editor 2.0 è disabilitato. Ora che l’editor di e-mail 2.0 è abilitato automaticamente, verrà visualizzato il seguente comportamento:

* Quando crei un nuovo messaggio e-mail, viene visualizzato il [Selettore modelli e-mail](email-template-picker-overview.md) e potrai scegliere un modello e-mail v2.0.
* Ogni volta che crei o modifichi un’e-mail con Email Editor 2.0, l’e-mail risultante sarà **sempre** contrassegnata come v2.0 (anche se hai utilizzato un modello e-mail v1.0).

Se l’abbonamento dispone di e-mail v1.0 prima del passaggio a E-mail Editor 2.0, si verifica il seguente comportamento in base allo stato corrente della risorsa:

**Approvato** : facendo clic su &quot;Modifica bozza&quot; verrà creata una bozza v2.0 dell’e-mail approvata. Se poi approvi la bozza v2.0, lo stato approvato dell’e-mail diventa v2.0 e non c’è modo di ripristinare la versione v1.0.\
**Bozza** : facendo clic su &quot;Modifica bozza&quot; la bozza viene contrassegnata automaticamente come v2.0. A questo punto, non sarà possibile eliminare e ripristinare la versione v1.0 perché non è disponibile una versione approvata della risorsa.
**Approvato con bozza** : facendo clic su &quot;Modifica bozza&quot; la bozza viene contrassegnata automaticamente come v2.0. Per questo motivo, non è possibile ripristinare la bozza alla versione 1.0.

Se l’abbonamento dispone di modelli e-mail v1.0 prima del passaggio a E-mail Editor 2.0, si verifica il seguente comportamento:

**Approvato** : facendo clic su &quot;Modifica bozza&quot; verrà creata una bozza v2.0 del modello e-mail esistente.
**Bozza** : facendo clic su &quot;Modifica bozza&quot; la bozza viene contrassegnata automaticamente come v2.0. A questo punto, non sarà possibile eliminare e ripristinare la versione v1.0 perché non è disponibile una versione approvata della risorsa.
**Approvato con bozza** : facendo clic su &quot;Modifica bozza&quot; la bozza viene contrassegnata automaticamente come v2.0. Per questo motivo, non è possibile ripristinare la bozza alla versione 1.0.

Se approvi un modello e-mail precedentemente v1.0 (in uno qualsiasi degli stati di cui sopra), vedrai il seguente comportamento:

Per le e-mail v1.0 esistenti che utilizzavano il modello (in precedenza v1.0):\
**E-mail v1.0 approvata**  - Verrà creata una bozza di A v2.0 per questa e-mail, utilizzando comunque il modello v2.0 appena approvato. Riceverà anche eventuali modifiche al modello.\
**Bozza e-mail v1.0**  - La bozza rimarrà v1.0 finché non fai clic su &quot;Modifica bozza&quot;. Successivamente, verrà automaticamente contrassegnato come v2.0 e riceverà eventuali modifiche al modello.\
**Approvato con bozza v1.0 e-mail**  - La bozza rimarrà v1.0 finché non fai clic su &quot;Modifica bozza&quot;. Successivamente, verrà automaticamente contrassegnato come v2.0 e riceverà eventuali modifiche al modello.

Per le e-mail v2.0 esistenti che utilizzavano il modello (in precedenza v1.0):\
**E-mail v2.0 approvata**  - Verrà creata una bozza v2.0 per questa e-mail, ancora &quot;utilizzando&quot; il modello appena approvato, e riceverà eventuali modifiche al modello.\
**Bozza e-mail v2.0**  - La bozza rimarrà invariata (v2.0) e riceverà eventuali modifiche al modello.\
**Approvato con bozza v2.0 e-mail**  - La bozza rimarrà invariata (v2.0) e riceverà eventuali modifiche al modello.

>[!CAUTION]
>
>Se approvi la bozza v2.0 di un modello e-mail v1.0, il modello diventerà v2.0. **nessun modo** per ripristinarlo alla versione v1.0.

Aspetti da considerare

* Le e-mail approvate vengono **mai** modificate.

* I modelli e-mail approvati sono **mai** modificati.

* In alcuni casi **rari**, non è possibile aprire un messaggio e-mail v1.0 in Email Editor 2.0. In questo caso, elimina la bozza e contatta il supporto Marketo.

>[!MORELIKETHIS]
>
>* [Panoramica di Email Editor 2.0](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-editor-v2-0-overview.md)
>* [Sintassi del modello e-mail](/help/marketo/product-docs/email-marketing/general/email-editor-2/email-template-syntax.md)

