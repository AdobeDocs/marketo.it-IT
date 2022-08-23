---
unique-page-id: 1147322
description: Informazioni sulle attività e le persone anonime - Documentazione di Marketo - Documentazione del prodotto
title: Informazioni sulle attività e le persone anonime
exl-id: 1676e8f3-9138-42ed-8bb4-40e195391fc4
source-git-commit: cc66f4ff2e3e0e6ddfabab91215e3ad31f3b9226
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 0%

---

# Informazioni sulle attività e le persone anonime {#understanding-anonymous-activity-and-people}

La prima volta che un utente visita una pagina di destinazione di Marketo (o una pagina del sito web che ha [Codice di tracciamento Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md), Marketo crea un _attività anonima_ e utilizza un cookie del browser per tenerlo traccia. Una volta identificato, diventa una persona e la cronologia associata al cookie del browser viene unita.

>[!IMPORTANT]
>
>Abilitazione della funzione Beta **Munchkin V2 Anonymous Replay attività su noto** assicura che le campagne attivate da una promozione lead anonima vengano sempre riprodotte dopo che il lead anonimo è stato unito con successo al record noto. Di conseguenza, i campi personalizzati modificati dai passaggi Cambia valore dati in qualsiasi campagna riprodotta verranno mantenuti nel record noto.

**Un Anonimo** l’attività viene creata quando un utente:

* Visita la prima volta la pagina di destinazione di Marketo.
* Visita una pagina del sito che ha [Tracciamento Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md).
* Fai clic su [Visualizza come pagina Web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) in un’e-mail di Marketo.

>[!NOTE]
>
>A differenza di altri collegamenti nelle e-mail di Marketo, [Visualizza come pagina Web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) non viene tracciato come clic e-mail.

Un’attività anonima viene unita a una persona nuova o esistente quando un utente:

* Fai clic su [collegamento in un’e-mail di Marketo](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md).
* Riempie un Marketo [Modulo](/help/marketo/product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md).
* Utilizza Marketo [SOAP](/help/marketo/product-docs/administration/additional-integrations/configuring-your-soap-api-settings.md) o [Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md) API (per sviluppatori) per associare una persona anonima a un record noto.

Un nome nel database potrebbe essere legato a molti cookie perché le persone spesso utilizzano diversi dispositivi e browser per visitare il tuo sito.

>[!NOTE]
>
>Quando i record anonimi vengono uniti in un record di persona nuovo o esistente, i valori dei campi personalizzati verranno **not** trasferimento.
