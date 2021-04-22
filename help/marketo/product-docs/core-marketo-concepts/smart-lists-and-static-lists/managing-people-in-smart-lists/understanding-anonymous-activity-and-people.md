---
unique-page-id: 1147322
description: Informazioni sulle attività e le persone anonime - Documentazione di Marketo - Documentazione del prodotto
title: Informazioni sulle attività e le persone anonime
exl-id: 1676e8f3-9138-42ed-8bb4-40e195391fc4
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '208'
ht-degree: 0%

---

# Informazioni sulle attività e le persone anonime {#understanding-anonymous-activity-and-people}

La prima volta che un utente visita una pagina di destinazione di Marketo (o una pagina del sito web con il [codice di tracciamento di Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md), Marketo crea un’ _attività anonima_ e utilizza un cookie del browser per tenerne traccia. Una volta identificato, diventa una persona e la cronologia associata al cookie del browser viene unita.

**Viene creata un&#39;attività** Anonimousine quando un utente:

* Visita la prima volta la pagina di destinazione di Marketo.
* Visita una pagina del tuo sito che ha [Munchkin tracking](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md).
* Fai clic sul collegamento [Visualizza come pagina web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) in un messaggio e-mail di Marketo.

>[!NOTE]
>
>A differenza di altri collegamenti nelle e-mail di Marketo, [Visualizza come pagina web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) non viene tracciato come clic e-mail.

Un’attività anonima viene unita a una persona nuova o esistente quando un utente:

* Fai clic su un collegamento [in un messaggio e-mail Marketo](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md).
* Riempie un Marketo [Form](/help/marketo/product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md).
* Utilizza l&#39;API Marketo [SOAP](/help/marketo/product-docs/administration/additional-integrations/configuring-your-soap-api-settings.md) o [Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) (per gli sviluppatori) per associare una persona anonima a un record noto.

Un nome nel database potrebbe essere legato a molti cookie perché le persone spesso utilizzano diversi dispositivi e browser per visitare il tuo sito.

>[!NOTE]
>
>Quando i record anonimi vengono uniti in un record di persona nuovo o esistente, i valori dei campi personalizzati vengono trasferiti **non**.
