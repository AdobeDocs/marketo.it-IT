---
unique-page-id: 2360253
description: Modificare il messaggio "Visualizza come pagina web" - Marketo Docs - Documentazione del prodotto
title: Modificare il messaggio "Visualizza come pagina web"
exl-id: 5541fe6c-7297-4277-8355-ba7b4ac73e2e
source-git-commit: 2776969be44ba1a3d795e99986d10cf0470fb9e9
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 0%

---

# Modificare il messaggio &quot;Visualizza come pagina web&quot; {#edit-the-view-as-web-page-message}

Se devi modificare il valore &quot;[Visualizza come pagina web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)&quot; testo, ecco come.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

## Modificare il messaggio &quot;Visualizza come pagina web&quot; {#edit-the-view-as-web-page-message-1}

1. Vai a **Amministratore** area.

   ![](assets/edit-the-view-as-web-page-message-1.png)

1. Fai clic su **E-mail**.

   ![](assets/edit-the-view-as-web-page-message-2.png)

   >[!CAUTION]
   >
   >Le seguenti variabili sono fondamentali. Non cancellarle!
   >
   >`%mkt_webview_url%?mkt_tok=##MKT_TOK##`
   >
   >Seconda parte `##MKT_TOK##` è il biscotto di quella persona. Quando fanno clic sul collegamento, gli viene applicato un cookie appropriato.

1. Modifica le **Visualizza come HTML pagina Web** e **Visualizza come testo della pagina web** versioni a tuo piacimento e fai clic su **Salva modifiche**.

   ![](assets/edit-the-view-as-web-page-message-3.png)

>[!CAUTION]
>
>Assicurati di evitare:
>
>* Aggiunta di URL aggiuntivi a una delle caselle di HTML
>* Inserimento di HTML nella versione di testo


Ecco qua. Invia e-mail di prova per garantire la formattazione.

## Testo predefinito &quot;Visualizza come pagina web&quot; {#default-view-as-web-page-text}

Per ripristinare il sistema predefinito &quot;Visualizza come pagina Web&quot;, copia/incolla quanto segue:

**Visualizza come HTML pagina Web:**

`<pre data-theme="Confluence"><div style="text-align: center"><font face="Verdana" size="1">To view this email as a web page, <a href="%mkt_webview_url%?mkt_tok=##MKT_TOK##">click here</a></font></div></pre>`

**Visualizza come testo della pagina Web:**

Per visualizzare questa e-mail come pagina web, vai al seguente indirizzo:
`<pre data-theme="Confluence">%mkt_webview_url%?mkt_tok=##MKT_TOK##</pre>`

Tutto qui!
