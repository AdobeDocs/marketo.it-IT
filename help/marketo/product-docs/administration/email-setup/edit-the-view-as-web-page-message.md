---
unique-page-id: 2360253
description: Modificare il messaggio "Visualizza come pagina web" - Documentazione di Marketo - Documentazione del prodotto
title: Modifica il messaggio "Visualizza come pagina web"
exl-id: 5541fe6c-7297-4277-8355-ba7b4ac73e2e
feature: Email Setup
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 0%

---

# Modifica il messaggio &quot;Visualizza come pagina web&quot; {#edit-the-view-as-web-page-message}

Se devi modificare il &quot;[Visualizza come pagina Web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)&quot;text, ecco come.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

## Modifica il messaggio &quot;Visualizza come pagina web&quot; {#edit-the-view-as-web-page-message-1}

1. Vai a **[!UICONTROL Amministratore]** area.

   ![](assets/edit-the-view-as-web-page-message-1.png)

1. Clic **[!UICONTROL E-mail]**.

   ![](assets/edit-the-view-as-web-page-message-2.png)

   >[!CAUTION]
   >
   >Le seguenti variabili sono critiche. Non eliminarle!
   >
   >`%mkt_webview_url%?mkt_tok=##MKT_TOK##`
   >
   >La seconda parte `##MKT_TOK##` è il [!UICONTROL munchkin] cookie di quella persona. Si assicura che vengano cookie in modo appropriato quando fanno clic sul collegamento.

1. Modifica il **[!UICONTROL Visualizza come Web Page HTML]** e **[!UICONTROL Visualizza come testo pagina Web]** versioni desiderate e fare clic su **[!UICONTROL Salva modifiche]**.

   ![](assets/edit-the-view-as-web-page-message-3.png)

>[!CAUTION]
>
>Assicurati di evitare:
>
>* Aggiunta di URL aggiuntivi a una delle caselle di HTML
>* Inserimento di HTML nella versione di testo

Eccola qui. Invia e-mail di test per garantire la formattazione.

## Testo predefinito &quot;Visualizza come pagina Web&quot; {#default-view-as-web-page-text}

Se hai bisogno di tornare al sistema predefinito &quot;[!UICONTROL Visualizza come pagina Web]&quot;, copia/incolla quanto segue:

**[!UICONTROL Visualizza come Web Page HTML]**:

`<pre data-theme="Confluence"><div style="text-align: center"><font face="Verdana" size="1">To view this email as a web page, <a href="%mkt_webview_url%?mkt_tok=##MKT_TOK##">click here</a></font></div></pre>`

**[!UICONTROL Visualizza come testo pagina Web]**:

Per visualizzare questa e-mail come pagina Web, vai al seguente indirizzo:
`<pre data-theme="Confluence">%mkt_webview_url%?mkt_tok=##MKT_TOK##</pre>`

Tutto qui!
