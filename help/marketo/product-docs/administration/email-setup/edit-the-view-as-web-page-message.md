---
unique-page-id: 2360253
description: Modificare il messaggio "Visualizza come pagina web" - Documentazione di Marketo - Documentazione del prodotto
title: Modificare il messaggio “Visualizza come pagina web”
exl-id: 5541fe6c-7297-4277-8355-ba7b4ac73e2e
feature: Email Setup
source-git-commit: 65d607e279fb86b0816ccaec2f4bf3c69e309cb9
workflow-type: tm+mt
source-wordcount: '155'
ht-degree: 16%

---

# Modificare il messaggio “Visualizza come pagina web” {#edit-the-view-as-web-page-message}

Se devi modificare il testo &quot;[Visualizza come pagina Web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)&quot;, ecco come.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

## Modificare il messaggio “Visualizza come pagina web” {#edit-the-view-as-web-page-message-1}

1. Passa alla schermata **[!UICONTROL Admin]**.

   ![](assets/edit-the-view-as-web-page-message-1.png)

1. Fai clic su **[!UICONTROL Email]**.

   ![](assets/edit-the-view-as-web-page-message-2.png)

   >[!CAUTION]
   >
   >Le seguenti variabili sono critiche. Non eliminarle!
   >
   >`%mkt_webview_url%?mkt_tok=##MKT_TOK##`
   >
   >La seconda parte `##MKT_TOK##` è il cookie [!UICONTROL munchkin] di quella persona. Si assicura che vengano cookie in modo appropriato quando fanno clic sul collegamento.

1. Modifica le versioni **[!UICONTROL View as Web Page HTML]** e **[!UICONTROL View as Web Page Text]** e fai clic su **[!UICONTROL Save Changes]**.

   ![](assets/edit-the-view-as-web-page-message-3.png)

>[!CAUTION]
>
>Assicurati di evitare:
>
>* Aggiunta di URL aggiuntivi a una delle caselle di HTML
>* Inserimento di HTML nella versione di testo

Eccola qui. Invia e-mail di test per garantire la formattazione.

## Testo predefinito &quot;Visualizza come pagina Web&quot; {#default-view-as-web-page-text}

Se è necessario ripristinare il sistema predefinito &quot;[!UICONTROL View as Web Page]&quot;, copiare/incollare quanto segue:

**[!UICONTROL View as Web Page HTML]**:

`<div style="text-align: center"><font face="Verdana" size="1">To view this email as a web page, <a href="%mkt_webview_url%?mkt_tok=##MKT_TOK##">click here</a></font></div>`

**[!UICONTROL View as Web Page Text]**:

Per visualizzare questa e-mail come pagina Web, vai al seguente indirizzo:
`%mkt_webview_url%?mkt_tok=##MKT_TOK##`

Tutto qui!
