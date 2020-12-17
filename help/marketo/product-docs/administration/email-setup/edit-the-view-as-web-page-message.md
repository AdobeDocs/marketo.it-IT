---
unique-page-id: 2360253
description: Modifica il messaggio "Visualizza come pagina Web" - Documenti Marketo - Documentazione del prodotto
title: Modifica il messaggio "Visualizza come pagina Web"
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 0%

---


# Modifica il messaggio &quot;Visualizza come pagina Web&quot; {#edit-the-view-as-web-page-message}

Per modificare il testo &quot; [Visualizza come pagina Web](../../../product-docs/email-marketing/general/functions-in-the-editor/add-a-view-as-web-page-link-to-an-email.md)&quot;, vedere come.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

## Modifica il messaggio &quot;Visualizza come pagina Web&quot; {#edit-the-view-as-web-page-message-1}

1. In **Admin**, fare clic su **Email**.

   ![](assets/image2014-9-18-17-3a13-3a2.png)

   >[!CAUTION]
   >
   >Le seguenti variabili sono fondamentali. Non eliminarle!
   >
   >    
   >    
   >    * %mkt_webview_url%?mkt_tok=##MKT_TOK#
   >    
   >    
   >La seconda parte ##MKT_TOK## è il biscotto di quella persona. In questo modo, quando fanno clic sul collegamento, gli utenti potranno ricevere il cookie appropriato.

1. Modificate le versioni **Visualizza come pagina Web HTML** e **Visualizza come testo pagina Web **a vostro piacimento, quindi fate clic su **Salva modifiche**.

   ![](assets/image2016-8-26-14-3a40-3a29.png)

>[!CAUTION]
>
>Assicuratevi di evitare:
>
>* Aggiunta di URL aggiuntivi a una delle caselle HTML
>* Inserimento di HTML nella versione di testo

>



Ecco qua. Invia e-mail di prova per garantire la formattazione.

## Testo predefinito &quot;Visualizza come pagina Web&quot; {#default-view-as-web-page-text}

Per ripristinare il sistema predefinito &quot;Visualizza come pagina Web&quot;, copiate/incollate quanto segue:

**Visualizza come HTML pagina Web:**
`<pre data-theme="Confluence"><div style="text-align: center"><font face="Verdana" size="1">To view this email as a web page, <a href="%mkt_webview_url%?mkt_tok=##MKT_TOK##">click here</a></font></div></pre>` **Visualizza come testo pagina Web:**

Per visualizzare questo messaggio e-mail come pagina Web, andate al seguente indirizzo:
`<pre data-theme="Confluence">%mkt_webview_url%?mkt_tok=##MKT_TOK##</pre>` Boom! Hai finito.
