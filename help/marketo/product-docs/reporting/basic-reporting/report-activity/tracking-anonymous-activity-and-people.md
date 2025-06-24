---
unique-page-id: 2360181
description: Tracciamento attività e persone anonime - Documentazione di Marketo - Documentazione del prodotto
title: Tracciamento di attività e persone anonime
exl-id: 95a39e57-4636-4bae-8ca8-00cb43cb566c
feature: Reporting
source-git-commit: e3f61755dccd9bea1378a429fc428b440fc3ecb4
workflow-type: tm+mt
source-wordcount: '221'
ht-degree: 0%

---

# Tracciamento di attività e persone anonime {#tracking-anonymous-activity-and-people}

La prima volta che un utente visita una [pagina di destinazione](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) di Marketo (o una pagina del sito Web che contiene il [codice di tracciamento di Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)), Marketo crea una _attività anonima_ e utilizza un cookie del browser per tenerne traccia. Una volta identificato, il visitatore diventa una persona e la cronologia associata al cookie del browser viene unita in.

1. Un&#39;attività anonima viene creata quando un utente:

   * Visita la [pagina di destinazione](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) di Marketo la prima volta.
   * Visita una pagina del sito con [tracciamento Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md).
   * Fai clic sul collegamento [Visualizza come pagina Web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) in un messaggio e-mail di Marketo.

   >[!NOTE]
   >
   >A differenza di altri collegamenti nelle e-mail di Marketo, Visualizza come pagina web non viene tracciato come clic e-mail.

   Un’attività anonima viene unita a una persona nuova o esistente quando qualcuno:

   * Fa clic su un [collegamento in un&#39;e-mail di Marketo](/help/marketo/product-docs/email-marketing/general/using-tokens/add-tokens-to-an-email-link.md).
   * Compila un [modulo](/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md) Marketo.
   * Utilizza l&#39;[API REST](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/leads) o l&#39;API [Munchkin](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/javascriptapi/leadtracking/lead-tracking) di Marketo (per sviluppatori) per associare un&#39;attività anonima a un record noto.

   Un nome nel database potrebbe essere associato a molti cookie perché le persone spesso utilizzano dispositivi e browser diversi per visitare il sito.

   >[!NOTE]
   >
   >Quando i record anonimi vengono uniti in un record persona nuovo o esistente, i valori dei campi personalizzati **non** verranno trasferiti.

   >[!MORELIKETHIS]
   >
   >[Visualizzare persone o visitatori anonimi nei report Web](/help/marketo/product-docs/reporting/basic-reporting/report-activity/display-people-or-anonymous-visitors-in-web-reports.md)
