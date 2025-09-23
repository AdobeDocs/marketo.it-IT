---
unique-page-id: 2360251
description: Modificare il messaggio di annullamento dell’iscrizione - Documentazione di Marketo - Documentazione del prodotto
title: Modificare il messaggio di annullamento dell’iscrizione
exl-id: 68a3ebc1-b2c9-4e6c-bb13-e5a94c9596d2
feature: Email Setup
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '127'
ht-degree: 8%

---

# Modificare il messaggio di annullamento dell’iscrizione {#edit-the-unsubscribe-message}

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

Quando invii e-mail di marketing (non [operative](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md)), il testo e i collegamenti per l&#39;annullamento dell&#39;iscrizione vengono aggiunti in basso. È possibile modificare i valori predefiniti. Ecco come.

## Dove effettuare la modifica {#where-to-make-the-edit}

1. Passare alla sezione **[!UICONTROL Admin]**.

   ![](assets/edit-the-unsubscribe-message-1.png)

1. Fai clic su **[!UICONTROL Email]**.

   ![](assets/edit-the-unsubscribe-message-2.png)

   >[!CAUTION]
   >
   >Le seguenti variabili sono critiche. Non eliminarle!
   >
   >* `%mkt_opt_out_prefix%`
   >* `mkt_unsubscribe=1&mkt_tok=##MKT_TOK##`

1. Modifica le versioni **[!UICONTROL Unsubscribe HTML]** e **[!UICONTROL Unsubscribe Text]** e fai clic su **[!UICONTROL Save Changes]**.

   ![](assets/edit-the-unsubscribe-message-3.png)

   Eccola qui. _Verifica._ Non vuoi che le e-mail di marketing abbiano collegamenti di annullamento degli abbonamenti interrotti.

>[!TIP]
>
>Puoi personalizzare la posizione del HTML per l&#39;annullamento dell&#39;abbonamento nell&#39;e-mail utilizzando [token](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md).

## Testo predefinito per annullamento iscrizione {#default-unsubscribe-text}

Se hai bisogno di ripristinare il sistema predefinito per annullare l’abbonamento, copia/incolla quanto segue:

[!UICONTROL Unsubscribe HTML]:
`<p><font face="Verdana" size="1">If you no longer wish to receive these emails, click on the following link: <a href="%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##">Unsubscribe</a><br/></font></p>` [!UICONTROL Unsubscribe Text]:
`%mkt_opt_out_prefix%UnsubscribePage.html?mkt_unsubscribe=1&mkt_tok=##MKT_TOK##`

>[!MORELIKETHIS]
>
>[Modifica il messaggio &quot;Visualizza come pagina Web&quot;](/help/marketo/product-docs/administration/email-setup/edit-the-view-as-web-page-message.md)
