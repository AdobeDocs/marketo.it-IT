---
unique-page-id: 1147322
description: Informazioni sulle attività e le persone anonime - Marketo Docs - Documentazione prodotto
title: Informazioni sulle attività anonime e sulle persone
translation-type: tm+mt
source-git-commit: 07f713ece9832b7696451001f61c6a3b45b4a94a
workflow-type: tm+mt
source-wordcount: '208'
ht-degree: 0%

---


# Informazioni sulle attività anonime e sulle persone {#understanding-anonymous-activity-and-people}

La prima volta che un utente visita una pagina di destinazione Marketo (o una pagina del sito Web con il [Codice di tracciamento Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md), Marketo crea un&#39;attività _anonima_ e utilizza un cookie del browser per tenerne traccia. Una volta identificato, diventa una persona e la cronologia associata al cookie del browser viene unita.

**Viene creata un&#39;attività** Anonimousine quando un utente:

* Visita la pagina di destinazione Marketo la prima volta.
* Visita una pagina del sito con [Monitoraggio Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md).
* Fate clic sul collegamento [Visualizza come pagina Web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) in un messaggio e-mail di tipo Marketo.

>[!NOTE]
>
>A differenza di altri collegamenti nelle e-mail di Marketo, [Visualizza come pagina Web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) non viene tracciato come clic tramite e-mail.

Un&#39;attività anonima viene unita in una persona nuova o esistente quando un utente:

* Fate clic su un collegamento [in un&#39;e-mail di Marketo](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md).
* Riempie il campo Marketo [Form](/help/marketo/product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md).
* Utilizza l&#39;API di Marketo [SOAP](/help/marketo/product-docs/administration/additional-integrations/configuring-your-soap-api-settings.md) o [Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) (per gli sviluppatori) per associare una persona anonima a un record noto.

Un nome nel database potrebbe essere associato a molti cookie perché le persone spesso utilizzano dispositivi e browser diversi per visitare il sito.

>[!NOTE]
>
>Quando i record anonimi vengono uniti in un record di persona nuovo o esistente, i valori dei campi personalizzati **non** vengono trasferiti.
