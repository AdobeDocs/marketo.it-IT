---
unique-page-id: 2360181
description: Tracciamento delle attività e delle persone anonime - Documenti Marketo - Documentazione del prodotto
title: Tracciamento di attività e persone anonime
exl-id: 95a39e57-4636-4bae-8ca8-00cb43cb566c
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 0%

---

# Tracciamento di attività e persone anonime {#tracking-anonymous-activity-and-people}

La prima volta che qualcuno visita un Marketo [pagina di destinazione](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) (o una pagina del sito web che ha la [Codice di tracciamento Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)), Marketo crea un _attività anonima_ e utilizza un cookie del browser per tenerlo traccia. Una volta identificato il visitatore, diventa una persona e la cronologia associata al cookie del browser viene unita.

1. Quando un utente:

   * Visita il tuo Marketo [pagina di destinazione](/help/marketo/product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) la prima volta.
   * Visita una pagina del sito che ha [Tracciamento Munchkin](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md).
   * Fai clic su [Visualizza come pagina Web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) in un’e-mail di Marketo.

   >[!NOTE]
   >
   >A differenza di altri collegamenti nelle e-mail di Marketo, Visualizza come pagina web non viene tracciato come clic e-mail.

   Un’attività anonima viene unita a una persona nuova o esistente quando un utente:

   * Fai clic su [collegamento in un’e-mail di Marketo](/help/marketo/product-docs/email-marketing/general/using-tokens/add-tokens-to-an-email-link.md).
   * Riempie un Marketo [modulo](/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md).
   * Utilizza Marketo [API REST](https://developers.marketo.com/rest-api/lead-database/leads/) o [Munchkin](https://developers.marketo.com/documentation/websites/lead-tracking-munchkin-js/) API (per sviluppatori) per associare un’attività anonima a un record noto.

   Un nome nel database potrebbe essere legato a molti cookie perché le persone spesso utilizzano diversi dispositivi e browser per visitare il tuo sito.

   >[!NOTE]
   >
   >Quando i record anonimi vengono uniti in un record di persona nuovo o esistente, i valori dei campi personalizzati verranno **not** trasferimento.

   >[!MORELIKETHIS]
   >
   >[Visualizzare persone o visitatori anonimi nei rapporti web](/help/marketo/product-docs/reporting/basic-reporting/report-activity/display-people-or-anonymous-visitors-in-web-reports.md)
