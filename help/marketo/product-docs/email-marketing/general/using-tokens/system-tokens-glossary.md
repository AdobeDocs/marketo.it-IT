---
unique-page-id: 1147344
description: Glossario dei token di sistema - Documenti Marketo - Documentazione del prodotto
title: Glossario dei token di sistema
exl-id: 8a7694af-4edb-4b32-b408-19d2e7bd596e
source-git-commit: 93032a016a67fe0edf7a8093633d6b06ec25c18d
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%

---

# Glossario dei token di sistema {#system-tokens-glossary}

Oltre ai token per le persone, è possibile utilizzare alcuni token di sistema molto interessanti. Eccoli qui.

>[!NOTE]
>
>Le impostazioni del fuso orario dell’account influiscono su quando vengono eseguiti i token di data e ora.

## system.date {#system-date}

La `{{system.date}}` il token eseguirà il rendering della data corrente in fase di runtime nel modo seguente: **8 agosto 2013**

**Lavora in:**

* [Modifica valore dati](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md)Passaggio di flusso {target=&quot;_blank&quot;}
* [Momento interessante](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md)Passaggio di flusso {target=&quot;_blank&quot;}
* [Crea attività](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md)Passaggio di flusso {target=&quot;_blank&quot;}
* Il corpo di un’e-mail o di un modello

## system.time {#system-time}

La `{{system.time}}` il token eseguirà il rendering dell’ora corrente in fase di runtime in questo modo: **04:34 (GMT -0700)**

**Lavora in:**

* [Modifica valore dati](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md)Passaggio di flusso {target=&quot;_blank&quot;}
* [Momento interessante](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md)Passaggio di flusso {target=&quot;_blank&quot;}
* [Crea attività](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md)Passaggio di flusso {target=&quot;_blank&quot;}
* Il corpo di un’e-mail o di un modello

## system.dateTime {#system-datetime}

La `{{system.dateTime}}` il token eseguirà il rendering della data e dell’ora correnti in fase di runtime nel modo seguente: **08/08/2013:36:13**

**Lavora in:**

* [Modifica valore dati](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md)Passaggio di flusso {target=&quot;_blank&quot;}
* [Momento interessante](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md)Passaggio di flusso {target=&quot;_blank&quot;}
* [Crea attività](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md)Passaggio di flusso {target=&quot;_blank&quot;}
* Il corpo di un’e-mail o di un modello

## system.forwardToFriendLink {#system-forwardtofriendlink}

La `{{system.forwardToFriendLink}}` token consente di controllare il posizionamento del [&quot;Inoltra a un link amico&quot; nelle e-mail](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/forward-to-a-friend-link-in-emails.md){target=&quot;_blank&quot;}.

**Lavora in:**

* [Aggiungere un token di sistema come collegamento in un’e-mail](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target=&quot;_blank&quot;} o modello

## system.unsubscribeLink {#system-unsubscribelink}

La `{{system.unsubscribeLink}}` token consente di controllare il posizionamento del collegamento di annullamento dell’abbonamento in un messaggio e-mail.

**Lavora in:**

* [Aggiungere un token di sistema come collegamento in un’e-mail](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target=&quot;_blank&quot;} o modello

## system.viewAsWebpageLink {#system-viewaswebpagelink}

La `{{system.viewAsWebpageLink}}` token consente di controllare il posizionamento del collegamento Visualizza come pagina web in un messaggio e-mail.

**Funziona con:**

* [Aggiungere un token di sistema come collegamento in un’e-mail](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target=&quot;_blank&quot;} o modello
