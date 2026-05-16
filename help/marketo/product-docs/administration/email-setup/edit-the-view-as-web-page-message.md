---
unique-page-id: 2360253
description: Personalizza il testo del collegamento Visualizza come pagina web e HTML nell’e-mail di amministrazione mantenendo intatte le variabili richieste.
title: Modifica il messaggio "Visualizza come pagina web"
exl-id: 5541fe6c-7297-4277-8355-ba7b4ac73e2e
feature: Email Setup
TQID: https://experienceleague.adobe.com/mREJHheKv7c16atJ17pv8S9ZGUoLnD8jd5jyk6QtgR8
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: d1d0a9cd-295d-4976-8c39-ddae266f240e
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 153
ht-degree: 0%

---

# Modifica il messaggio &quot;Visualizza come pagina web&quot; {#edit-the-view-as-web-page-message}

Scopri come modificare il testo &quot;[Visualizza come pagina Web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)&quot;.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

## Modifica il messaggio &quot;Visualizza come pagina web&quot; {#edit-the-view-as-web-page-message-1}

1. Passare all&#39;area **[!UICONTROL Admin]**.

   ![](assets/edit-the-view-as-web-page-message-1.png)

1. Fare clic su **[!UICONTROL Email]**.

   ![](assets/edit-the-view-as-web-page-message-2.png)

   >[!CAUTION]
   >
   >Le seguenti variabili sono critiche. Non eliminarle!
   >
   >`%mkt_webview_url%?mkt_tok=##MKT_TOK##`
   >
   >La seconda parte `##MKT_TOK##` è il cookie [!UICONTROL Munchkin] di quella persona. In questo modo, quando fanno clic sul collegamento, vengono tracciati correttamente.

1. Modifica le versioni **[!UICONTROL View as Web Page HTML]** e **[!UICONTROL View as Web Page Text]** e fai clic su **[!UICONTROL Save Changes]**.

   ![](assets/edit-the-view-as-web-page-message-3.png)

>[!CAUTION]
>
>Assicurati di evitare:
>
>* Aggiunta di URL aggiuntivi a una delle caselle di HTML
>* Inserimento di HTML nella versione di testo

Invia e-mail di prova per verificare la formattazione.

## Testo predefinito &quot;Visualizza come pagina Web&quot; {#default-view-as-web-page-text}

Se è necessario ripristinare il sistema predefinito &quot;[!UICONTROL View as Web Page]&quot;, copiare/incollare quanto segue:

**[!UICONTROL View as Web Page HTML]**:

`<div style="text-align: center"><font face="Verdana" size="1">To view this email as a web page, <a href="%mkt_webview_url%?mkt_tok=##MKT_TOK##">click here</a></font></div>`

**[!UICONTROL View as Web Page Text]**:

Per visualizzare questa e-mail come pagina Web, vai al seguente indirizzo:
`%mkt_webview_url%?mkt_tok=##MKT_TOK##`
