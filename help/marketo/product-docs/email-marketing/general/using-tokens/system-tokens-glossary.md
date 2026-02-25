---
unique-page-id: 1147344
description: Glossario dei token di sistema - Documentazione di Marketo - Documentazione del prodotto
title: Glossario dei token di sistema
exl-id: 8a7694af-4edb-4b32-b408-19d2e7bd596e
feature: Tokens
source-git-commit: bf420edcc79aa551e286302fa002df9162371873
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 2%

---

# Glossario dei token di sistema {#system-tokens-glossary}

Oltre ai token di persona, puoi utilizzare anche alcuni token di sistema molto interessanti. Eccoli.

>[!NOTE]
>
>Le impostazioni del fuso orario dell’account influiscono sull’esecuzione dei token di data e ora.

## system.date {#system-date}

Il token `{{system.date}}` riprodurrà la data corrente in fase di runtime come segue: **8 agosto 2013**

**Funziona in:**

* [Modifica valore dati](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"} passaggio di flusso
* [Passaggio di flusso Momento di interesse](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target="_blank"}
* [Crea attività](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"} passaggio di flusso
* Corpo di un messaggio e-mail o di un modello

## system.time {#system-time}

Il token `{{system.time}}` eseguirà il rendering dell&#39;ora corrente in fase di runtime come segue: **04:34 PM (GMT -0700)**

**Funziona in:**

* [Modifica valore dati](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"} passaggio di flusso
* [Passaggio di flusso Momento di interesse](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target="_blank"}
* [Crea attività](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"} passaggio di flusso
* Corpo di un messaggio e-mail o di un modello

## system.dateTime {#system-datetime}

Il token `{{system.dateTime}}` restituirà la data e l&#39;ora correnti in fase di runtime come segue: **2013-08-08 16:36:13**

**Funziona in:**

* [Modifica valore dati](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/change-data-value.md){target="_blank"} passaggio di flusso
* [Passaggio di flusso Momento di interesse](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/interesting-moment.md){target="_blank"}
* [Crea attività](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/salesforce-flow-actions/create-task.md){target="_blank"} passaggio di flusso
* Corpo di un messaggio e-mail o di un modello

## system.unsubscribeLink {#system-unsubscribelink}

Il token `{{system.unsubscribeLink}}` consente di controllare il posizionamento del collegamento per l&#39;annullamento dell&#39;abbonamento in un messaggio e-mail.

**Funziona in:**

* [Aggiungere un token di sistema come collegamento in un messaggio e-mail](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"} o in un modello

## system.viewAsWebpageLink {#system-viewaswebpagelink}

Il token `{{system.viewAsWebpageLink}}` consente di controllare la posizione del collegamento Visualizza come pagina Web in un messaggio e-mail.

**Funziona con:**

* [Aggiungere un token di sistema come collegamento in un messaggio e-mail](/help/marketo/product-docs/email-marketing/general/using-tokens/add-a-system-token-as-a-link-in-an-email.md){target="_blank"} o in un modello
