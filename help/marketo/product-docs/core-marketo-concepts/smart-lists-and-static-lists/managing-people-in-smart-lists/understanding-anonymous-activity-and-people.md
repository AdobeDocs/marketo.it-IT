---
unique-page-id: 1147322
description: Informazioni su attività e persone anonime - Documentazione di Marketo - Documentazione del prodotto
title: Informazioni su attività e persone anonime
exl-id: 1676e8f3-9138-42ed-8bb4-40e195391fc4
feature: Smart Lists
source-git-commit: 208ba59e3a5cb8e613e887b4c89e51cec4b3f897
workflow-type: tm+mt
source-wordcount: '262'
ht-degree: 0%

---

# Informazioni su attività e persone anonime {#understanding-anonymous-activity-and-people}

La prima volta che un utente visita una pagina di destinazione di Marketo (o una pagina del sito web con [Codice di tracciamento Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"}), Marketo crea un *attività anonima* e utilizza un cookie del browser per tracciarlo. Una volta identificato, diventa una persona e la cronologia associata al cookie del browser viene unita in.

>[!IMPORTANT]
>
>Abilitazione della funzione beta **Attività riproduzione anonima Munchkin V2 su noto** garantisce che le campagne attivate dalla promozione anonima di lead vengano sempre riprodotte dopo che il lead anonimo è stato unito correttamente al record noto. Di conseguenza, i campi personalizzati modificati dai passaggi Modifica valore dati nelle campagne ripetute verranno mantenuti nel record noto.

**Un anonimo** l&#39;attività viene creata quando un utente:

* Visita la pagina di destinazione di Marketo la prima volta.
* Visita una pagina del sito con [Tracciamento di Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"}.
* Fa clic su [Visualizza come pagina Web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md){target="_blank"} in un messaggio e-mail di Marketo.

>[!NOTE]
>
>A differenza di altri collegamenti nelle e-mail di Marketo, [Visualizza come pagina Web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md){target="_blank"} non viene tracciato come clic e-mail.

Un’attività anonima viene unita a una persona nuova o esistente quando qualcuno:

* Clic su un [collegamento in un messaggio e-mail di Marketo](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"}.
* Compila un Marketo [Modulo](/help/marketo/product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md){target="_blank"}.
* Utilizza Marketo [SOAP](/help/marketo/product-docs/administration/additional-integrations/configuring-your-soap-api-settings.md){target="_blank"} or [Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"} API (per sviluppatori) per associare una persona anonima a un record noto.

Un nome nel database potrebbe essere associato a molti cookie perché le persone spesso utilizzano dispositivi e browser diversi per visitare il sito.

>[!NOTE]
>
>Quando i record anonimi vengono uniti in un record persona nuovo o esistente, i valori dei campi personalizzati *non* trasferimento.
