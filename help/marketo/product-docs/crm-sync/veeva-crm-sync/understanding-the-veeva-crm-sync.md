---
description: Informazioni sulla sincronizzazione di Veeva CRM - Documenti Marketo - Documentazione del prodotto
title: Informazioni sulla sincronizzazione di Veeva CRM
exl-id: 99ade106-7f32-40e8-8b9a-2b1d0e769b9c
source-git-commit: 884c9a27f3876ec3036f2f7187db30565cdd49a7
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---

# Informazioni sulla sincronizzazione di Veeva CRM {#understanding-the-veeva-crm-sync}

In pochi semplici passi, è facile eseguire una sincronizzazione tra Adobe Marketo Engage e Veeva CRM.

## Funzionamento della sincronizzazione {#how-the-sync-works}

Marketo Engage sincronizza con Veeva CRM tutto il giorno, ogni giorno. Ogni sincronizzazione richiede un po&#39; di tempo, si mette in pausa per 5 minuti, quindi si riavvia.

>[!NOTE]
>
>La prima sincronizzazione potrebbe richiedere ore o anche giorni perché il Marketo Engage sta copiando l&#39;intero database da Veeva. In seguito, ogni sincronizzazione richiede in genere minuti (a volte secondi) e sincronizza solo i dati che sono cambiati.

![](assets/understanding-the-veeva-sync-1.png)

La sincronizzazione tra Veeva e Marketo Engage è bidirezionale solo per i campi Contatto sull&#39;oggetto account Persona. In questi casi, ogni volta che apporti modifiche in Veeva o nel Marketo Engage, gli aggiornamenti verranno rispecchiati in entrambi i sistemi. Tutte le altre sincronizzazioni sono da Veeva al solo Marketo Engage. Fai clic sui link qui sotto per i dettagli su ciascuno.

## Che cosa è sincronizzato tra il Marketo Engage e Veeva {#what-is-synced-between-marketo-engage-and-veeva}

* [Account personali](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/person-account-sync-faq.md){target=&quot;_blank&quot;}
* Utenti
* [Chiama e chiama oggetti chiave](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target=&quot;_blank&quot;}
* [Oggetti personalizzati](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/custom-object-sync.md){target=&quot;_blank&quot;}

## Cose da sapere {#things-to-know}

* La [credenziali inserite in Marketo Engage per Veeva](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target=&quot;_blank&quot;} vengono utilizzati per sincronizzare i dati. Verranno inclusi solo i dati a cui tali credenziali hanno accesso.

* Veeva CRM è basato su force.com e il Marketo Engage di esperienze avanzate con la piattaforma viene ereditato in questa sincronizzazione.

* Veeva CRM mostra: Lead, contatto, account (account aziendali, opportunità, campagna e attività). Tuttavia, non sono supportati nella sincronizzazione con il Marketo Engage.
