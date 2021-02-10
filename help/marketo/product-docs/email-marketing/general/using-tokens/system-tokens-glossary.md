---
unique-page-id: 1147344
description: Glossario dei token di sistema - Documenti Marketo - Documentazione del prodotto
title: Glossario dei token di sistema
translation-type: tm+mt
source-git-commit: 0f0217a88929661798015b51a26259a973f9f6ea
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---


# Glossario dei token di sistema {#system-tokens-glossary}

Oltre ai token per le persone, è possibile utilizzare anche alcuni token di sistema molto interessanti. Eccoli.

>[!NOTE]
>
>Le impostazioni del fuso orario dell&#39;account influiscono sull&#39;esecuzione dei token di data e ora.

## system.date {#system-date}

Il token `{{system.date}}` esegue il rendering della data corrente in fase di esecuzione, come segue: **08 agosto 2013**

**Funziona in:**

* [Passaggio Modifica ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) valore dati
* [Interessante passo ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md) Momentflow
* [Crea passaggio ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md) flusso di task
* Il corpo di un’e-mail o di un modello

## system.time {#system-time}

Il token `{{system.time}}` eseguirà il rendering dell&#39;ora corrente in fase di esecuzione come segue: **04:34 PM (GMT -0700)**

**Funziona in:**

* [Passaggio Modifica ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) valore dati
* [Interessante passo ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md) Momentflow
* [Crea passaggio ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md) flusso di task
* Il corpo di un’e-mail o di un modello

## system.dateTime {#system-datetime}

Il token `{{system.dateTime}}` esegue il rendering della data e dell&#39;ora correnti in fase di esecuzione come segue: **2013-08-08 16:36:13**

**Funziona in:**

* [Passaggio Modifica ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) valore dati
* [Interessante passo ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md) Momentflow
* [Crea passaggio ](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md) flusso di task
* Il corpo di un’e-mail o di un modello

## system.forwardToFriendLink {#system-forwardtofriendlink}

Il token `{{system.forwardToFriendLink}}` consente di controllare il posizionamento del [&#39;Inoltra a un collegamento amico&#39; in E-mail](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/forward-to-a-friend-link-in-emails.md).

**Funziona in:**

* [Aggiunta di un token di sistema come collegamento in un modello ](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md) Emailor

## system.unsubscriptionLink {#system-unsubscribelink}

Il token `{{system.unsubscribLink}}` consente di controllare il posizionamento del collegamento di annullamento della sottoscrizione in un&#39;e-mail.

**Funziona in:**

* [Aggiunta di un token di sistema come collegamento in un modello ](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md) Emailor

## system.viewAsWebpageLink {#system-viewaswebpagelink}

Il token `{{system.viewAsWebpageLink}}` consente di controllare il posizionamento del collegamento Visualizza come pagina Web in un messaggio e-mail.

**Funziona con:**

* [Aggiunta di un token di sistema come collegamento in un modello ](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md) Emailor
