---
unique-page-id: 4719316
description: Utilizzo di account utente - Documenti Marketo - Documentazione prodotto
title: Utilizzo di account di persona
translation-type: tm+mt
source-git-commit: 728066ab05de82f6123bfaa1f0b05af8632e32b2
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---


# Utilizzo di account di persona {#using-person-accounts}

Gli account personali possono essere configurati in Salesforce per soddisfare le esigenze della tua organizzazione. Ecco come Marketo gestisce gli account delle persone.

>[!NOTE]
>
>Gli account Salesforce predefiniti sono account aziendali. L&#39;amministratore di Salesforce deve configurare gli account utente separatamente.

## Che cos&#39;è un account persona? {#what-is-a-person-account}

Un account utente è molto simile all&#39;oggetto account in Salesforce. Tuttavia, un account utente ha accesso sia ai campi dell&#39;account che ai campi dei contatti.

## Cosa succede quando un account utente viene sincronizzato su Marketo? {#what-happens-when-a-person-account-is-synced-to-marketo}

Un account utente viene sincronizzato con Marketo come azienda e come persona.

>[!NOTE]
>
>I campi personalizzati per un account utente vengono copiati sia nella società che nella persona di Marketo.

## Come si differenziano gli account aziendali e gli account delle persone? {#how-do-i-differentiate-business-accounts-and-person-accounts}

Utilizzate il filtro Account **persona** presente nell&#39;elenco smart per separare gli account delle persone dagli account aziendali standard.

## Dove sono visualizzate le informazioni sugli account personali in Marketing Sales Insight? {#where-is-my-person-accounts-information-displayed-in-marketo-sales-insight}

Le attività relative agli account utente vengono visualizzate nel pannello **Account** .

>[!NOTE]
>
>Le opzioni di Marketing Sales Insight **Add to Marketo Campaign **and **Send Email **attualmente non sono disponibili per gli account utente.

## Come si associano le opportunità a un account personale? {#how-do-i-associate-opportunities-to-a-person-account}

Marketo dipende dal ruolo di contatto opportunità per determinare a quale persona associare l&#39;opportunità. È necessario aggiungere il ruolo di contatto opportunità per ogni account personale per collegare l&#39;opportunità alla persona appropriata in Marketo. È consigliabile impostare un flusso di lavoro per aggiungere automaticamente il ruolo di contatto opportunità.

## Quale campo e-mail devo utilizzare per gli account utente? {#which-email-field-should-i-use-for-person-accounts}

Esistono due campi e-mail per un account utente. Utilizzare il campo Indirizzo **e-** mail nei moduli (non l&#39;indirizzo **e-mail** Persona) per garantire il corretto funzionamento della deduplicazione di Marketo e di altre elaborazioni e-mail.
