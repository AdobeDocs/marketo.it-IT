---
unique-page-id: 2360251
description: Modificare il messaggio di annullamento dell’abbonamento - Documenti Marketo - Documentazione del prodotto
title: Modificare il messaggio di annullamento dell’abbonamento
exl-id: 68a3ebc1-b2c9-4e6c-bb13-e5a94c9596d2
source-git-commit: 931b42d7266b9c57308567527042dfcad9847993
workflow-type: tm+mt
source-wordcount: '135'
ht-degree: 0%

---

# Modificare il messaggio di annullamento dell’abbonamento {#edit-the-unsubscribe-message}

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

Quando invii e-mail di marketing (non-[operativo](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)), il testo dell’annullamento dell’abbonamento e i collegamenti sono aggiunti in basso. È possibile modificare le impostazioni predefinite. Ecco come.

## Modificare il messaggio di annullamento dell’abbonamento {#edit-the-unsubscribe-message-1}

1. Sotto **Amministratore**, fai clic su **E-mail**.

   ![](assets/image2014-9-18-16-3a52-3a1.png)

   >[!CAUTION]
   >
   >Le seguenti variabili sono fondamentali. Non cancellarle!
   >
   >* `%mkt_opt_out_prefix%`
   >* `mkt_unsubscribe=1&mkt_tok=##MKT_TOK##`


1. Modifica le **Annulla sottoscrizione HTML** e **Testo non registrato** versioni a tuo piacimento e fai clic su **Salva modifiche**.

   ![](assets/image2016-8-26-13-3a40-3a55.png)

   Ecco qua. _Assicurati di provare!_ Non vuoi che le tue e-mail di marketing dispongano di collegamenti di annullamento dell’abbonamento interrotti.

>[!TIP]
>
>Puoi personalizzare la posizione del HTML di annullamento dell’abbonamento nell’e-mail utilizzando [gettoni](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md).

## Testo per annullamento sottoscrizione predefinito {#default-unsubscribe-text}

Per ripristinare l’annullamento dell’abbonamento al sistema predefinito, copia/incolla quanto segue:

Annulla sottoscrizione HTML:
`<pre data-theme="Confluence"><p><font face="Verdana" size="1">If you no longer wish to receive these emails, click on the following link: <a href="%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##">Unsubscribe</a><br/></font></p></pre>` Testo per annullamento sottoscrizione:
`<pre data-theme="Confluence">%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##</pre>`

>[!MORELIKETHIS]
>
>[Modificare il messaggio &quot;Visualizza come pagina web&quot;](/help/marketo/product-docs/administration/email-setup/edit-the-view-as-web-page-message.md)
