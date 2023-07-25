---
unique-page-id: 1147344
description: Glossario dei token di sistema - Documentazione di Marketo - Documentazione del prodotto
title: Glossario dei token di sistema
exl-id: 8a7694af-4edb-4b32-b408-19d2e7bd596e
feature: Tokens
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---

# Glossario dei token di sistema {#system-tokens-glossary}

Oltre ai token di persona, puoi utilizzare anche alcuni token di sistema molto interessanti. Eccoli.

>[!NOTE]
>
>Le impostazioni del fuso orario dell’account influiscono sull’esecuzione dei token di data e ora.

## system.date {#system-date}

Il `{{system.date}}` il token riporterà la data corrente in fase di runtime nel modo seguente: **8 agosto 2013**

**Funziona in:**

* [Modifica valore dati](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"} passaggio di flusso
* [Momento di interesse](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target="_blank"} passaggio di flusso
* [Crea attività](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"} passaggio di flusso
* Corpo di un messaggio e-mail o di un modello

## system.time {#system-time}

Il `{{system.time}}` il token eseguirà il rendering dell’ora corrente in fase di runtime nel modo seguente: **16:34 (GMT -0700)**

**Funziona in:**

* [Modifica valore dati](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"} passaggio di flusso
* [Momento di interesse](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target="_blank"} passaggio di flusso
* [Crea attività](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"} passaggio di flusso
* Corpo di un messaggio e-mail o di un modello

## system.dateTime {#system-datetime}

Il `{{system.dateTime}}` il token eseguirà il rendering della data e dell’ora correnti in fase di runtime nel modo seguente: **08/08/2013 16:36:13**

**Funziona in:**

* [Modifica valore dati](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"} passaggio di flusso
* [Momento di interesse](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target="_blank"} passaggio di flusso
* [Crea attività](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"} passaggio di flusso
* Corpo di un messaggio e-mail o di un modello

## system.forwardToFriendLink {#system-forwardtofriendlink}

Il `{{system.forwardToFriendLink}}` token consente di controllare il posizionamento del [&#39;Inoltra a un collegamento amico&#39; nelle e-mail](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/forward-to-a-friend-link-in-emails.md){target="_blank"}.

**Funziona in:**

* [Aggiungere un token di sistema come collegamento in un messaggio e-mail](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"} o modello

## system.unsubscribeLink {#system-unsubscribelink}

Il `{{system.unsubscribeLink}}` token consente di controllare il posizionamento del collegamento per annullare l’abbonamento in un’e-mail.

**Funziona in:**

* [Aggiungere un token di sistema come collegamento in un messaggio e-mail](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"} o modello

## system.viewAsWebpageLink {#system-viewaswebpagelink}

Il `{{system.viewAsWebpageLink}}` token consente di controllare la posizione del collegamento Visualizza come pagina web in un messaggio e-mail.

**Funziona con:**

* [Aggiungere un token di sistema come collegamento in un messaggio e-mail](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"} o modello
