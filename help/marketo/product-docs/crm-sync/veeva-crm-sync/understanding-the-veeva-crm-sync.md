---
description: Informazioni sulla sincronizzazione di  [!DNL Veeva] CRM - Documentazione di Marketo - Documentazione del prodotto
title: Informazioni sulla sincronizzazione di  [!DNL Veeva] CRM
exl-id: 99ade106-7f32-40e8-8b9a-2b1d0e769b9c
feature: Veeva CRM
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# Informazioni sulla sincronizzazione CRM per [!DNL Veeva] {#understanding-the-veeva-crm-sync}

In pochi semplici passaggi è facile eseguire una sincronizzazione tra Adobe Marketo Engage e il CRM [!DNL Veeva].

## Funzionamento della sincronizzazione {#how-the-sync-works}

Marketo Engage esegue la sincronizzazione con [!DNL Veeva] CRM tutto il giorno, ogni giorno. Ogni sincronizzazione richiede un po’ di tempo, si mette in pausa per 5 minuti, quindi si riavvia.

>[!NOTE]
>
>La prima sincronizzazione potrebbe richiedere ore o anche giorni perché Marketo Engage sta copiando l&#39;intero database da [!DNL Veeva]. Successivamente, ogni sincronizzazione richiede in genere minuti (a volte secondi) e sincronizza solo i dati modificati.

![](assets/understanding-the-veeva-sync-1.png)

La sincronizzazione tra [!DNL Veeva] e Marketo Engage è bidirezionale solo per i campi Contatto nell&#39;oggetto account Persona. In questi casi, ogni volta che si apportano modifiche in [!DNL Veeva] o Marketo Engage, gli aggiornamenti verranno applicati a entrambi i sistemi. Tutte le altre sincronizzazioni sono solo da [!DNL Veeva] a Marketo Engage. Fai clic sui collegamenti riportati di seguito per ottenere informazioni dettagliate su ciascuno di essi.

## Cos&#39;è sincronizzato tra Marketo Engage e [!DNL Veeva] {#what-is-synced-between-marketo-engage-and-veeva}

* [Account persona](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/person-account-sync-faq.md){target="_blank"}
* Utenti
* [Richiama e richiama oggetti chiave](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target="_blank"}
* [Oggetti personalizzati](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/custom-object-sync.md){target="_blank"}

## Aspetti da considerare {#things-to-know}

* Le [credenziali immesse in Marketo Engage per  [!DNL Veeva]](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"} vengono utilizzate per sincronizzare i dati. Verranno inclusi solo i dati a cui le credenziali hanno accesso.

* [!DNL Veeva] CRM è basato su force.com e l&#39;esperienza avanzata di Marketo Engage con la piattaforma è ereditata in questa sincronizzazione.

* Il CRM Veeva mostra: lead, contatto, account, account aziendali, opportunità, campagna e attività. Tuttavia, non sono supportati nella sincronizzazione con Marketo Engage.
