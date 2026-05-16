---
unique-page-id: 2360181
description: Scopri come tracciare le attività anonime e le persone in Marketo Engage, incluso il tracciamento delle attività anonime e. Utilizza questa guida per completare il passaggio successivo.
title: Tracciare attività e persone anonime
exl-id: 95a39e57-4636-4bae-8ca8-00cb43cb566c
feature: Reporting
TQID: https://experienceleague.adobe.com/BZakQFVtQystRyrlzo81s-p8N65LXHUJ2ZoSAzeTG6Q
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b0bb9048-d951-48d8-8232-45cf248a7e27id: b13bd2ad-8e65-49e5-9691-2a0d31067b35id: c5f60233-d5ea-4453-a799-0ad258b4d399id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: ea90ebee-5c84-42d9-8b21-006bdabc95a3
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 255
ht-degree: 8%

---

# Tracciare attività e persone anonime {#tracking-anonymous-activity-and-people}

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
   * Utilizza l&#39;[API REST](https://experienceleague.adobe.com/en/docs/marketo-developer/marketo/rest/lead-database/leads) o l&#39;API [Munchkin](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/javascriptapi/leadtracking/lead-tracking) di Marketo (per sviluppatori) per associare un&#39;attività anonima a un record noto.

   Un nome nel database potrebbe essere associato a molti cookie perché le persone spesso utilizzano dispositivi e browser diversi per visitare il sito.

   >[!NOTE]
   >
   >Quando i record anonimi vengono uniti in un record persona nuovo o esistente, i valori dei campi personalizzati **non** verranno trasferiti.

   >[!MORELIKETHIS]
   >
   >[Visualizzare persone o visitatori anonimi nei report Web](/help/marketo/product-docs/reporting/basic-reporting/report-activity/display-people-or-anonymous-visitors-in-web-reports.md)
