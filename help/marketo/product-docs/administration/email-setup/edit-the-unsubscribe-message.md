---
unique-page-id: 2360251
description: Modifica il messaggio di annullamento della sottoscrizione - Documenti Marketo - Documentazione prodotto
title: Modifica del messaggio di annullamento della sottoscrizione
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 0%

---


# Modifica del messaggio di annullamento della sottoscrizione {#edit-the-unsubscribe-message}

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

Quando invii e-mail di marketing (non [operative](../../../product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)), il testo di annullamento della sottoscrizione e i collegamenti vengono aggiunti in basso. Potete modificare le impostazioni predefinite. Ecco come.

## Modifica del messaggio di annullamento della sottoscrizione {#edit-the-unsubscribe-message-1}

1. In **Amministratore**, fai clic su **E-mail**.

   ![](assets/image2014-9-18-16-3a52-3a1.png)

   >[!CAUTION]
   >
   >
   >Le seguenti variabili sono fondamentali. Non eliminarle!
   >
   >    
   >    
   >    * **%mkt_opt_out_prefix%**
   >    * **mkt_unsubscription=1&amp;mkt_tok=##MKT_TOK#**


1. Modificate le versioni HTML **** Annulla sottoscrizione e **Annulla sottoscrizione testo** a vostro piacimento, quindi fate clic su **Salva modifiche**.

   ![](assets/image2016-8-26-13-3a40-3a55.png)

   Ecco qua. **Assicuratevi di provare!** Non vuoi che le tue e-mail di marketing abbiano collegamenti di annullamento della sottoscrizione interrotti.

>[!TIP]
>
>Potete personalizzare la posizione del codice HTML per l’annullamento della sottoscrizione nell’e-mail utilizzando [i token](../../../product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md).

## Testo per annullamento sottoscrizione predefinito {#default-unsubscribe-text}

Per ripristinare l’iscrizione predefinita al sistema, copiate/incollate quanto segue:

Annulla sottoscrizione HTML:
`<pre data-theme="Confluence"><p><font face="Verdana" size="1">If you no longer wish to receive these emails, click on the following link: <a href="%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##">Unsubscribe</a><br/></font></p></pre>` Testo per annullamento sottoscrizione:
`<pre data-theme="Confluence">%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##</pre>`

>[!MORELIKETHIS]
>
>* [Modifica il messaggio &quot;Visualizza come pagina Web&quot;](edit-the-view-as-web-page-message.md)

>



