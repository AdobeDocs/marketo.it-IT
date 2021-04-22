---
unique-page-id: 2360253
description: Modificare il messaggio "Visualizza come pagina web" - Marketo Docs - Documentazione del prodotto
title: Modificare il messaggio "Visualizza come pagina web"
exl-id: 5541fe6c-7297-4277-8355-ba7b4ac73e2e
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '182'
ht-degree: 0%

---

# Modificare il messaggio &quot;Visualizza come pagina web&quot; {#edit-the-view-as-web-page-message}

Se devi modificare il testo &quot;[Visualizza come pagina web](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)&quot;, ecco come.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

## Modificare il messaggio &quot;Visualizza come pagina web&quot; {#edit-the-view-as-web-page-message-1}

1. In **Amministratore**, fai clic su **E-mail**.

   ![](assets/image2014-9-18-17-3a13-3a2.png)

   >[!CAUTION]
   >
   >Le seguenti variabili sono fondamentali. Non cancellarle!
   >
   >`%mkt_webview_url%?mkt_tok=##MKT_TOK##`
   >
   >La seconda parte `##MKT_TOK##` è il biscotto di munchkin di quella persona. Quando fanno clic sul collegamento, gli viene applicato un cookie appropriato.

1. Modifica le versioni **Visualizza come pagina Web HTML** e **Visualizza come testo di pagina web** e fai clic su **Salva modifiche**.

   ![](assets/image2016-8-26-14-3a40-3a29.png)

>[!CAUTION]
>
>Assicurati di evitare:
>
>* Aggiunta di URL aggiuntivi a una delle caselle HTML
>* Inserimento di HTML nella versione di testo


Ecco qua. Invia e-mail di prova per garantire la formattazione.

## Testo predefinito &quot;Visualizza come pagina web&quot; {#default-view-as-web-page-text}

Per ripristinare il sistema predefinito &quot;Visualizza come pagina Web&quot;, copia/incolla quanto segue:

**Visualizza come HTML della pagina Web:**

`<pre data-theme="Confluence"><div style="text-align: center"><font face="Verdana" size="1">To view this email as a web page, <a href="%mkt_webview_url%?mkt_tok=##MKT_TOK##">click here</a></font></div></pre>`

**Visualizza come testo della pagina Web:**

Per visualizzare questa e-mail come pagina web, vai al seguente indirizzo:
`<pre data-theme="Confluence">%mkt_webview_url%?mkt_tok=##MKT_TOK##</pre>` Boom! Ha finito.
