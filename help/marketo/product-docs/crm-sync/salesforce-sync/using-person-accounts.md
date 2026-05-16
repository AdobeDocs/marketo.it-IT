---
unique-page-id: 4719316
description: Scopri come Marketo Engage tratta gli account personali di Salesforce. Differenziare account persona e account aziendali e utilizzare il filtro Account persona Is in elenchi avanzati.
title: Utilizzare gli account persona
exl-id: 3cc67ff2-f689-4dfb-8b67-2b5b8d389aaf
feature: Salesforce Integration
TQID: https://experienceleague.adobe.com/-NqSQnq-q6-McMyxsWgX5WKx1F7pwTaOIPg1Se8M1zM
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b0bb9048-d951-48d8-8232-45cf248a7e27
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 297
ht-degree: 2%

---

# Utilizzare gli account persona {#using-person-accounts}

Gli account personali possono essere impostati in Salesforce in base alle esigenze della tua organizzazione. Di seguito viene descritto il modo in cui Marketo Engage tratta gli account personali.

>[!NOTE]
>
>Gli account [!DNL Salesforce] predefiniti sono account aziendali. L&#39;amministratore di [!DNL Salesforce] deve impostare gli account personali separatamente.

## Che cos&#39;è un account persona? {#what-is-a-person-account}

Un account persona è molto simile all&#39;oggetto account in [!DNL Salesforce]. Tuttavia, un account persona ha accesso sia ai campi account che ai campi contatto.

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
>Le opzioni **[!UICONTROL Add to Marketo Campaign]** e **[!UICONTROL Send Email]** di Marketo Sales Insight non sono attualmente disponibili per gli account personali.

## Come si associano le opportunità a un account personale? {#how-do-i-associate-opportunities-to-a-person-account}

Marketo dipende dal ruolo di contatto dell’opportunità per determinare a quale persona associare l’opportunità. È necessario aggiungere il ruolo di contatto dell’opportunità per ogni account persona per collegare l’opportunità alla persona appropriata in Marketo. È consigliabile impostare un flusso di lavoro per aggiungere automaticamente il ruolo di contatto dell’opportunità.

## Quale campo e-mail utilizzare per gli account persona? {#which-email-field-should-i-use-for-person-accounts}

Per un account persona sono disponibili due campi e-mail. Utilizza il campo **[!UICONTROL Email Address]** nei moduli (non **[!UICONTROL Person Email Address]**) per garantire il corretto funzionamento della deduplicazione di Marketo e di altre elaborazioni e-mail.
