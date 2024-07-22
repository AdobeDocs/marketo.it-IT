---
unique-page-id: 4719316
description: Utilizzo degli account persona - Documentazione di Marketo - Documentazione del prodotto
title: Utilizzo degli account persona
exl-id: 3cc67ff2-f689-4dfb-8b67-2b5b8d389aaf
feature: Salesforce Integration
source-git-commit: 4045f262889d06304111288d30da893529396e81
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---

# Utilizzo degli account persona {#using-person-accounts}

Gli account della persona possono essere impostati in Salesforce in base alle esigenze della tua organizzazione. Ecco come il Marketo Engage tratta gli account personali.

>[!NOTE]
>
>Gli account Salesforce predefiniti sono account aziendali. L’amministratore Salesforce deve impostare separatamente gli account personali.

## Che cos&#39;è un account persona? {#what-is-a-person-account}

Un account persona è molto simile all’oggetto account in Salesforce. Tuttavia, un account persona ha accesso sia ai campi account che ai campi contatto.

## Cosa succede quando un account persona viene sincronizzato con Marketo? {#what-happens-when-a-person-account-is-synced-to-marketo}

Un account persona viene sincronizzato in Marketo come azienda e come persona.

>[!NOTE]
>
>I campi personalizzati per un account persona vengono copiati sia nella società che nella persona in Marketo.

## Come posso distinguere gli account aziendali da quelli personali? {#how-do-i-differentiate-business-accounts-and-person-accounts}

Utilizza il filtro &quot;Account persona&quot; nell’elenco avanzato per separare gli account persona dagli account aziendali standard.

## Dove vengono visualizzate le informazioni sugli account personali in Marketo Sales Insight? {#where-is-my-person-accounts-information-displayed-in-marketo-sales-insight}

Le attività relative agli account persona vengono visualizzate nel pannello **[!UICONTROL Account]**.

>[!NOTE]
>
>Le opzioni **[!UICONTROL Aggiungi a Marketo Campaign]** e **[!UICONTROL Invia e-mail]** di Marketo Sales Insight non sono attualmente disponibili per gli account personali.

## Come si associano le opportunità a un account personale? {#how-do-i-associate-opportunities-to-a-person-account}

Marketo dipende dal ruolo di contatto dell’opportunità per determinare a quale persona associare l’opportunità. È necessario aggiungere il ruolo di contatto dell’opportunità per ogni account persona per collegare l’opportunità alla persona appropriata in Marketo. È consigliabile impostare un flusso di lavoro per aggiungere automaticamente il ruolo di contatto dell’opportunità.

## Quale campo e-mail utilizzare per gli account persona? {#which-email-field-should-i-use-for-person-accounts}

Per un account persona sono disponibili due campi e-mail. Utilizza il campo **Indirizzo e-mail** nei moduli (non **Indirizzo e-mail persona**) per garantire il corretto funzionamento della deduplicazione di Marketo e di altre elaborazioni e-mail.
