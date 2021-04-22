---
unique-page-id: 4719316
description: Utilizzo di account personali - Documenti Marketo - Documentazione del prodotto
title: Utilizzo di account personali
exl-id: 3cc67ff2-f689-4dfb-8b67-2b5b8d389aaf
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---

# Utilizzo di account personali {#using-person-accounts}

Gli account personali possono essere configurati in Salesforce per soddisfare le esigenze della tua organizzazione. Ecco come Marketo tratta gli account personali.

>[!NOTE]
>
>Gli account Salesforce predefiniti sono account aziendali. L’amministratore di Salesforce deve configurare gli account personali separatamente.

## Che cos’è un account persona? {#what-is-a-person-account}

Un account persona è molto simile all’oggetto account in Salesforce. Tuttavia, un account persona ha accesso sia ai campi dell’account che ai campi di contatto.

## Cosa succede quando un account persona viene sincronizzato con Marketo? {#what-happens-when-a-person-account-is-synced-to-marketo}

Un account persona viene sincronizzato in Marketo come azienda e come persona.

>[!NOTE]
>
>I campi personalizzati per un account persona vengono copiati sia nella società che nella persona in Marketo.

## Come differenziare account aziendali e account personali? {#how-do-i-differentiate-business-accounts-and-person-accounts}

Utilizza il filtro **Is Person Account** nel tuo smart list per separare gli account delle persone dagli account aziendali standard.

## Dove vengono visualizzate le informazioni sugli account personali in Marketo Sales Insight? {#where-is-my-person-accounts-information-displayed-in-marketo-sales-insight}

Le attività relative agli account utente vengono visualizzate nel pannello **Account** .

>[!NOTE]
>
>Le opzioni **Aggiungi a Marketo Campaign** e **Invia e-mail** di Marketo Sales Insight non sono attualmente disponibili per gli account personali.

## Come si associano le opportunità a un account persona? {#how-do-i-associate-opportunities-to-a-person-account}

Marketo dipende dal ruolo di contatto opportunità per determinare a quale persona associare l’opportunità. È necessario aggiungere il ruolo di contatto opportunità per ogni account personale per collegare l&#39;opportunità alla persona appropriata in Marketo. È consigliabile impostare un flusso di lavoro per aggiungere automaticamente il ruolo di contatto opportunità .

## Quale campo e-mail devo utilizzare per gli account personali? {#which-email-field-should-i-use-for-person-accounts}

Esistono due campi e-mail per un account persona. Utilizza il campo **Indirizzo e-mail** nei moduli (non l’ **Indirizzo e-mail persona**) per garantire il corretto funzionamento della deduplicazione Marketo e di altre elaborazioni e-mail.
