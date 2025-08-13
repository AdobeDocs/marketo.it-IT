---
solution: Marketo Engage
product: marketo
title: Token Personalization
description: Scopri come utilizzare i token di personalizzazione nel nuovo Designer e-mail di Marketo Engage
level: Beginner, Intermediate
feature: Email Designer
exl-id: 4828e1a5-822f-48a9-bbb8-b1ffe8421e4f
hide: true
hidefromtoc: true
source-git-commit: 2488e0e6af38a4d50b1a8f5f6194c64bd8504717
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---

# Token Personalization {#personalization-tokens}

E-mail designer ha un formato diverso rispetto all’editor e-mail classico quando si tratta di token di personalizzazione e-mail. La modifica è stata implementata per migliorare la compatibilità con gli script Handlebar e semplificare il processo di creazione delle e-mail.

>[!AVAILABILITY]
>
>A partire dal 23 maggio 2025, agli utenti di Marketo Engage verrà eseguito il provisioning di questa funzione in batch, con un’area aggiornata alla settimana. Durante il rollout, tutte le e-mail create utilizzando il nuovo e-mail designer eseguiranno automaticamente la migrazione dei token esistenti al nuovo formato. Con questo aggiornamento, tutti i token saranno disponibili solo in inglese.

## Caso d’uso principale {#primary-use-case}

Questo miglioramento è utile principalmente per coloro che passano dallo script [Velocity](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/email-scripting){target="_blank"} allo script Handlebar. Il nuovo e-mail designer supporta solo il nuovo formato di token. Il formato aggiornato elimina gli spazi e introduce una struttura di testo predefinita rivista, garantendo un’esperienza di scripting più fluida ed efficiente.

## Esperienza token {#token-experience}

Guarda l’esperienza del token, sia vecchia che nuova.

### Formato precedente {#old-format}

Nell&#39;editor di posta elettronica classico è possibile aggiungere token con spazi, ad esempio `lead.Anonymous IP` o `member.registration code`. Formato del testo predefinito: `{{lead.City:default=fallback}}`

![](assets/personalization-tokens-1.png){width="800" zoomable="yes"}

### Nuovo formato {#new-format}

Nella finestra di progettazione e-mail è necessario utilizzare [notazione camel](https://developer.mozilla.org/en-US/docs/Glossary/Camel_case) o caratteri di sottolineatura per i token (ad esempio, `lead.anonymousIP` o `member.registration_code`). Anche il formato del testo predefinito diventa `{%=lead.city ?: "fallback" %}`.

![](assets/personalization-tokens-2.png){width="800" zoomable="yes"}

## Aspetti da considerare {#things-to-note}

* L’editor di personalizzazione offre anche le seguenti funzioni per semplificare l’authoring:

   * Annulla/Ripristina
   * Trova/Trova e sostituisci

* **Tutti** i token precedentemente supportati in Marketo Engage sono supportati nel nuovo editor di personalizzazione.
