---
unique-page-id: 1147344
description: Glossario dei token di sistema - Documenti Marketo - Documentazione del prodotto
title: Glossario dei token di sistema
translation-type: tm+mt
source-git-commit: 1c4c4c62215550a09125f76fb76017348aba2bdf
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

Il `{{system.date}}` token esegue il rendering della data corrente in fase di esecuzione, come segue: **08 agosto 2013**

**Funziona in:**

* [Modifica passaggio del flusso del valore](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) dei dati
* [Interessante fase del flusso del momento](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md)
* [Crea passaggio flusso attività](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md)
* Il corpo di un’e-mail o di un modello

## system.time {#system-time}

Il `{{system.time}}` token eseguirà il rendering dell&#39;ora corrente in fase di esecuzione come segue: **04:34 PM (GMT -0700)**

**Funziona in:**

* [Modifica passaggio del flusso del valore](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) dei dati
* [Interessante fase del flusso del momento](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md)
* [Crea passaggio flusso attività](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md)
* Il corpo di un’e-mail o di un modello

## system.dateTime {#system-datetime}

Il `{{system.dateTime}}` token esegue il rendering della data e dell&#39;ora correnti in fase di esecuzione, come segue: **2013-08-08 16:36:13**

**Funziona in:**

* [Modifica passaggio del flusso del valore](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md) dei dati
* [Interessante fase del flusso del momento](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md)
* [Crea passaggio flusso attività](../../../../product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md)
* Il corpo di un’e-mail o di un modello

## system.forwardToFriendLink {#system-forwardtofriendlink}

Il `{{system.forwardToFriendLink}}` token consente di controllare la posizione del [&quot;Inoltra a un collegamento amico&quot; nelle e-mail](../../../../product-docs/email-marketing/general/functions-in-the-editor/forward-to-a-friend-link-in-emails.md).

**Funziona in:**

* [Aggiungere un token di sistema come collegamento in un messaggio e-mail](add-a-system-token-as-a-link-in-an-email.md) o in un modello

## system.unsubscriptionLink {#system-unsubscribelink}

Il `{{system.unsubscribLink}}` token consente di controllare la posizione del collegamento per l’annullamento della sottoscrizione in un messaggio e-mail.

**Funziona in:**

* [Aggiungere un token di sistema come collegamento in un messaggio e-mail](add-a-system-token-as-a-link-in-an-email.md) o in un modello

## system.viewAsWebpageLink {#system-viewaswebpagelink}

Il `{{system.viewAsWebpageLink}}` token consente di controllare il posizionamento del collegamento Visualizza come pagina Web in un messaggio e-mail.

**Funziona con:**

* [Aggiungere un token di sistema come collegamento in un messaggio e-mail](add-a-system-token-as-a-link-in-an-email.md) o in un modello
