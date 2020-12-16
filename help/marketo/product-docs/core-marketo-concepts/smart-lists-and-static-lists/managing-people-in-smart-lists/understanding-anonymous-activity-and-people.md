---
unique-page-id: 1147322
description: Informazioni sulle attività e le persone anonime - Marketo Docs - Documentazione prodotto
title: Informazioni sulle attività anonime e sulle persone
translation-type: tm+mt
source-git-commit: d7d6aee63144c472e02fe0221c4a164183d04dd4
workflow-type: tm+mt
source-wordcount: '219'
ht-degree: 0%

---


# Informazioni sulle attività anonime e sulle persone {#understanding-anonymous-activity-and-people}

La prima volta che un utente visita un Marketo [l `anding page`](http://docs.marketo.com/display/DOCS/Personalizing+Landing+Pages) (o una pagina del tuo sito Web con il codice [di tracciamento](../../../../product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)Munchkin), Marketo crea una **attività* *anonima e utilizza un cookie del browser per tenerne traccia. Una volta identificato, diventa una persona e la cronologia associata al cookie del browser viene unita.

**Quando un utente:**

* Visita la pagina di destinazione Marketo la prima volta.

* Visita una pagina del tuo sito con tracciamento [](../../../../product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)Munchkin.

* Fate clic sul collegamento [Visualizza come pagina](../../../../product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) Web in un messaggio e-mail di tipo Marketo.

>[!NOTE]
>
>A differenza di altri collegamenti nelle e-mail di Marketo, [Visualizza come pagina](../../../../product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) Web non viene tracciato come clic e-mail.

Un&#39;attività anonima viene unita in una persona nuova o esistente quando un utente:

* Fate clic su un [collegamento in un messaggio e-mail](../../../../product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md)di Marketo.
* Compilare un [modulo](../../../../product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md)Marketo.
* Utilizza l&#39;API [SOAP](http://docs.marketo.com/pages/viewpage.action?pageid=7509846) o [Munchkin](../../../../product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) di Marketo (per gli sviluppatori) per associare una persona anonima a un record noto.

Un nome nel database potrebbe essere associato a molti cookie perché le persone spesso utilizzano dispositivi e browser diversi per visitare il sito.

>[!NOTE]
>
>Quando i record anonimi vengono uniti in un record di persona nuovo o esistente, i valori dei campi personalizzati **non** vengono trasferiti.

