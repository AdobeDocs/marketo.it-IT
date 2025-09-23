---
unique-page-id: 1147322
description: Informazioni su attività e persone anonime - Documentazione di Marketo - Documentazione del prodotto
title: Informazioni su persone e a ttività anonime
exl-id: 1676e8f3-9138-42ed-8bb4-40e195391fc4
feature: Smart Lists
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '263'
ht-degree: 3%

---

# Informazioni su persone e a ttività anonime {#understanding-anonymous-activity-and-people}

La prima volta che un utente visita una pagina di destinazione di Marketo (o una pagina del sito Web che contiene il [Codice di monitoraggio di Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"}), Marketo crea una *attività anonima* e utilizza un cookie del browser per tenerne traccia. Una volta identificato, diventa una persona e la cronologia associata al cookie del browser viene unita in.

>[!IMPORTANT]
>
>L&#39;attivazione della funzionalità Beta **[!DNL Munchkin]V2 Attività di ripetizione anonima su Note** garantisce che le campagne attivate dalla promozione anonima dei lead vengano sempre rieseguite dopo che il lead anonimo è stato unito correttamente al record noto. Di conseguenza, i campi personalizzati modificati dai passaggi Modifica valore dati nelle campagne ripetute verranno mantenuti nel record noto.

**Un&#39;attività anonima** viene creata quando un utente:

* Visita la pagina di destinazione di Marketo la prima volta.
* Visita una pagina del sito con [tracciamento Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"}.
* Fai clic sul collegamento [Visualizza come pagina Web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md){target="_blank"} in un messaggio e-mail di Marketo.

>[!NOTE]
>
>A differenza di altri collegamenti nelle e-mail di Marketo, [Visualizza come pagina Web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md){target="_blank"} non viene tracciato come clic su e-mail.

Un’attività anonima viene unita a una persona nuova o esistente quando qualcuno:

* Fa clic su un [collegamento in un&#39;e-mail di Marketo](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"}.
* Compila un [modulo](/help/marketo/product-docs/demand-generation/forms/form-actions/embed-a-form-on-your-website.md){target="_blank"} Marketo.
* Utilizza l&#39;API [SOAP](/help/marketo/product-docs/administration/additional-integrations/configuring-your-soap-api-settings.md){target="_blank"} o [Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"} di Marketo (per sviluppatori) per associare una persona anonima a un record noto.

Un nome nel database potrebbe essere associato a molti cookie perché le persone spesso utilizzano dispositivi e browser diversi per visitare il sito.

>[!NOTE]
>
>Quando i record anonimi vengono uniti in un record persona nuovo o esistente, i valori dei campi personalizzati *non* verranno trasferiti.
