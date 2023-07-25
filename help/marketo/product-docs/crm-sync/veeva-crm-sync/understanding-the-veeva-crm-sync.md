---
description: Informazioni su Veeva CRM Sync - Marketo Docs - Documentazione del prodotto
title: Informazioni su Veeva CRM Sync
exl-id: 99ade106-7f32-40e8-8b9a-2b1d0e769b9c
feature: Veeva CRM
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 0%

---

# Informazioni su Veeva CRM Sync {#understanding-the-veeva-crm-sync}

In pochi semplici passaggi, è facile eseguire una sincronizzazione tra Adobe Marketo Engage e il CRM Veeva.

## Funzionamento della sincronizzazione {#how-the-sync-works}

Il Marketo Engage si sincronizza con Veeva CRM tutto il giorno, ogni giorno. Ogni sincronizzazione richiede un po’ di tempo, si mette in pausa per 5 minuti, quindi si riavvia.

>[!NOTE]
>
>La prima sincronizzazione potrebbe richiedere ore o addirittura giorni perché il Marketo Engage sta copiando l&#39;intero database da Veeva. Successivamente, ogni sincronizzazione richiede in genere minuti (a volte secondi) e sincronizza solo i dati modificati.

![](assets/understanding-the-veeva-sync-1.png)

La sincronizzazione tra Veeva e Marketi Engage è bidirezionale solo per i campi Contatto sull’oggetto account Persona. In questi casi, ogni volta che apporti modifiche in Veeva o Marketi Engage, gli aggiornamenti verranno rispecchiati in entrambi i sistemi. Tutte le altre sincronizzazioni sono da Veeva solo al Marketo Engage. Fai clic sui collegamenti riportati di seguito per ottenere informazioni dettagliate su ciascuno di essi.

## Cos’è sincronizzato tra Marketi Engage e Veeva {#what-is-synced-between-marketo-engage-and-veeva}

* [Account persona](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/person-account-sync-faq.md){target="_blank"}
* Utenti
* [Richiama e richiama oggetti chiave](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target="_blank"}
* [Oggetti personalizzati](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/custom-object-sync.md){target="_blank"}

## Aspetti da considerare {#things-to-know}

* Il [credenziali immesse nel Marketo Engage per Veeva](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"} vengono utilizzati per sincronizzare i dati. Verranno inclusi solo i dati a cui le credenziali hanno accesso.

* Veeva CRM è basato su force.com e il Marketo Engage di esperienza avanzato con la piattaforma è ereditato in questa sincronizzazione.

* Il CRM Veeva mostra: lead, contatto, account (account aziendali, opportunità, campagna e attività). Tuttavia, non sono supportati nella sincronizzazione con il Marketo Engage.
