---
unique-page-id: 2360181
description: Tracciamento delle attività e delle persone anonime - Marketo Docs - Documentazione prodotto
title: Tracciamento delle attività e delle persone anonime
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 0%

---


# Tracciamento delle attività anonime e delle persone {#tracking-anonymous-activity-and-people}

La prima volta che un utente visita una pagina di destinazione Marketo [o una pagina del sito Web con il [codice di monitoraggio Munchkin](../../../../product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md), Marketo crea un *anonimo* *activity* e utilizza un cookie del browser per tenerne traccia. ](../../../../product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) Una volta identificato, il visitatore diventa una persona e la cronologia associata al cookie del browser viene unita.

1. Quando un utente:

   * Visita per la prima volta la pagina di destinazione di Marketing [](../../../../product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md).
   * Visita una pagina del sito con [Monitoraggio Munchkin](../../../../product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md).
   * Fate clic sul collegamento [Visualizza come pagina Web](../../../../product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) in un messaggio e-mail di tipo Marketo.

   >[!NOTE]
   >
   >A differenza di altri collegamenti nelle e-mail Marketo, Visualizza come pagina Web non viene tracciato come clic e-mail.

   Un&#39;attività anonima viene unita in una persona nuova o esistente quando un utente:

   * Fate clic su un collegamento [in un&#39;e-mail di Marketo](../../../../product-docs/email-marketing/general/using-tokens/add-tokens-to-an-email-link.md).
   * Riempie il campo Marketo [form](http://docs.marketo.com/display/docs/forms).
   * Utilizza l&#39;API [REST API](http://developers.marketo.com/rest-api/lead-database/leads/) o [Munchkin](http://developers.marketo.com/documentation/websites/lead-tracking-munchkin-js/) di Marketo (per gli sviluppatori) per associare un&#39;attività anonima a un record noto.

   Un nome nel database potrebbe essere associato a molti cookie perché le persone spesso utilizzano dispositivi e browser diversi per visitare il sito.

   >[!NOTE]
   >
   >Quando i record anonimi vengono uniti in un record di persona nuovo o esistente, i valori dei campi personalizzati **non** vengono trasferiti.

   >[!MORELIKETHIS]
   >
   >
   >    
   >    
   >    * [Visualizzare persone o visitatori anonimi nei rapporti Web](display-people-or-anonymous-visitors-in-web-reports.md)


   >[!NOTE]
   >
   >**Tubo profondo**
   >
   >
   >Ulteriori informazioni su [Basic Reporting](http://docs.marketo.com/display/docs/basic+reporting).

