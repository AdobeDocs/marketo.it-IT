---
unique-page-id: 2360181
description: Tracciamento delle attività e delle persone anonime - Marketo Docs - Documentazione prodotto
title: Tracciamento delle attività e delle persone anonime
translation-type: tm+mt
source-git-commit: 1a29614ec938074902af201b2ffc11cfaa625f7a
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 0%

---


# Tracciamento delle attività e delle persone anonime {#tracking-anonymous-activity-and-people}

La prima volta che un utente visita una pagina [di](../../../../product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) destinazione Marketo (o una pagina del tuo sito Web con il codice [di monitoraggio](../../../../product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)Munchkin), Marketo crea un&#39; *attività* *anonima* e utilizza un cookie del browser per tenerla traccia. Una volta identificato, il visitatore diventa una persona e la cronologia associata al cookie del browser viene unita.

1. Quando un utente:

   * Visita la pagina [di](../../../../product-docs/demand-generation/landing-pages/free-form-landing-pages/create-a-free-form-landing-page.md) destinazione Marketo la prima volta.
   * Visita una pagina del tuo sito con tracciamento [](../../../../product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md)Munchkin.
   * Fate clic sul collegamento [Visualizza come pagina](../../../../product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md) Web in un messaggio e-mail di tipo Marketo.

   >[!NOTE]
   >
   >A differenza di altri collegamenti nelle e-mail Marketo, Visualizza come pagina Web non viene tracciato come clic e-mail.

   Un&#39;attività anonima viene unita in una persona nuova o esistente quando un utente:

   * Fate clic su un [collegamento in un messaggio e-mail](../../../../product-docs/email-marketing/general/using-tokens/add-tokens-to-an-email-link.md)di Marketo.
   * Compilare un [modulo](http://docs.marketo.com/display/docs/forms)Marketo.
   * Utilizza l&#39;API [](http://developers.marketo.com/rest-api/lead-database/leads/) REST di Marketo o l&#39;API [Munchkin](http://developers.marketo.com/documentation/websites/lead-tracking-munchkin-js/) (per gli sviluppatori) per associare un&#39;attività anonima a un record noto.

   Un nome nel database potrebbe essere associato a molti cookie perché le persone spesso utilizzano dispositivi e browser diversi per visitare il sito.

   >[!NOTE]
   >
   >Quando i record anonimi vengono uniti in un record di persona nuovo o esistente, i valori dei campi personalizzati **non** vengono trasferiti.

   >[!NOTE]
   >
   >**Articoli correlati**
   >
   >    
   >    
   >    * [Visualizzare persone o visitatori anonimi nei rapporti Web](display-people-or-anonymous-visitors-in-web-reports.md)


   >[!NOTE]
   >
   >**Tubo profondo**
   >
   >
   >Ulteriori informazioni sui rapporti [di](http://docs.marketo.com/display/docs/basic+reporting)base.

