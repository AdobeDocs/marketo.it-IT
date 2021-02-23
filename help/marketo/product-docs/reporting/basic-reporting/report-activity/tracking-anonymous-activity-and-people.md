---
unique-page-id: 2360181
description: Tracciamento delle attività e delle persone anonime - Marketo Docs - Documentazione prodotto
title: Tracciamento delle attività e delle persone anonime
translation-type: tm+mt
source-git-commit: 03ee7b69f691efce12825aa708c81dffa23cecd9
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 0%

---


# Tracciamento delle attività anonime e delle persone {#tracking-anonymous-activity-and-people}

La prima volta che un utente visita una pagina di destinazione Marketo [](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) (o una pagina del sito Web con il [codice di monitoraggio Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)), Marketo crea un&#39;attività _anonima_ e utilizza un cookie del browser per tenerne traccia. Una volta identificato, il visitatore diventa una persona e la cronologia associata al cookie del browser viene unita.

1. Quando un utente:

   * Visita per la prima volta la pagina di destinazione di Marketing [](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md).
   * Visita una pagina del sito con [Monitoraggio Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md).
   * Fate clic sul collegamento [Visualizza come pagina Web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) in un messaggio e-mail di tipo Marketo.

   >[!NOTE]
   >
   >A differenza di altri collegamenti nelle e-mail Marketo, Visualizza come pagina Web non viene tracciato come clic e-mail.

   Un&#39;attività anonima viene unita in una persona nuova o esistente quando un utente:

   * Fate clic su un collegamento [in un&#39;e-mail di Marketo](/help/marketo/product-docs/email-marketing/general/using-tokens/add-tokens-to-an-email-link.md).
   * Riempie il campo Marketo [form](/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md).
   * Utilizza l&#39;API [REST API](https://developers.marketo.com/rest-api/lead-database/leads/) o [Munchkin](https://developers.marketo.com/documentation/websites/lead-tracking-munchkin-js/) di Marketo (per gli sviluppatori) per associare un&#39;attività anonima a un record noto.

   Un nome nel database potrebbe essere associato a molti cookie perché le persone spesso utilizzano dispositivi e browser diversi per visitare il sito.

   >[!NOTE]
   >
   >Quando i record anonimi vengono uniti in un record di persona nuovo o esistente, i valori dei campi personalizzati **non** vengono trasferiti.

   >[!MORELIKETHIS]
   >
   >[Visualizzare persone o visitatori anonimi nei rapporti Web](/help/marketo/product-docs/reporting/basic-reporting/report-activity/display-people-or-anonymous-visitors-in-web-reports.md)
