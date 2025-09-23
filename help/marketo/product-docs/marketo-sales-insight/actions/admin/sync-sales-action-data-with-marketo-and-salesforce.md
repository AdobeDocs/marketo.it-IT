---
description: Sincronizzare i dati relativi alle azioni di vendita con Marketo e Salesforce - Documenti Marketo - Documentazione del prodotto
title: Sincronizzare i dati relativi alle azioni di vendita con Marketo e Salesforce
exl-id: bb213d50-be22-492d-b74c-b8cfb834b2ca
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '1068'
ht-degree: 3%

---

# Sincronizzare i dati relativi alle azioni di vendita con Marketo e Salesforce {#sync-sales-action-data-with-marketo-and-salesforce}

La sincronizzazione dei campi di unificazione dei dati per le azioni di Sales Insight consente al sistema di richiamare le informazioni sulle persone dal database di Marketo Engage nel database delle azioni di Sales Insight.

Questo fornisce dati aggiornati sulle persone nell’app web Azioni di Sales Insight e consente di raccogliere ID univoci per i record corrispondenti delle persone in Marketo e per i record relativi a lead/contatti/account/opportunità in Salesforce, in modo che sia possibile fare riferimento correttamente ai record per la registrazione dei dati.

Questa sincronizzazione può essere abilitata dalla scheda Configurazione azioni di Sales Insight nella sezione Admin di Marketo Engage. Per ulteriori informazioni, vedi [Avvia sincronizzazione dati](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.md#initiate-data-sync).

![](assets/actions-data-sync-faq-1.png)

Il diagramma precedente mostra come l’attività delle persone e i dati delle attività possono essere sincronizzati tra i sistemi. Alcune cose da notare:

* I record Persone vengono sincronizzati con le azioni Insight di vendita di Marketo Engage, rendendo Marketo Engage la fonte di verità per i dati relativi alle persone delle azioni Insight di vendita
* Le azioni Marketo Engage e Sales Insight [dispongono di un meccanismo](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md) per raccogliere e sincronizzare lo stato di annullamento dell&#39;iscrizione a Salesforce
* Lo stato di annullamento abbonamento non viene sincronizzato da Azioni di vendita a Marketo Engage, ma è possibile configurare Azioni di Insight vendite per verificare lo stato di annullamento abbonamento a Marketo delle persone prima di consentire ai venditori di inviare un&#39;e-mail con [Verifica annullamento abbonamento a Marketo](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md).

Di seguito sono riportate alcune domande frequenti relative al funzionamento della sincronizzazione di unificazione dei dati.

## Quali lead/contatti sono sincronizzati con le azioni di Sales Insight? {#what-lead-contacts-are-synced}

![](assets/actions-data-sync-faq-2.png)

I lead e i contatti a cui è assegnato un proprietario vendite verranno sincronizzati in Azioni di vendita.

Puoi verificare se un lead/contatto ha un proprietario vendite in Salesforce consultando il campo del proprietario standard esistente.

Il proprietario del servizio di vendita non deve essere l&#39;utente Marketo Sync o un utente Salesforce o di vendita specifico. È sufficiente che un utente sia elencato nei campi proprietario lead e proprietario contatto elencati in Salesforce, in modo da identificarlo come lead di vendita e sincronizzarlo con le azioni di Sales Insight. Eventuali aggiornamenti ai campi con cui eseguiamo la sincronizzazione verranno rilevati e aggiornati anche in Azioni Sales Insight.

## Da dove vengono originati i dati dell&#39;attività visualizzati nella griglia avanzata di Sales Insight? {#where-does-the-activity-data-get-sourced-from}

![](assets/actions-data-sync-faq-3.png)

I dati dell’attività come e-mail, chiamate, momenti di interesse e web provengono tutti dal database di Marketo Engage. Sales Insight Smart Grid invia una richiesta all’istanza di Marketo Engage per recuperarla ogni volta che un utente di vendita carica il pannello Sales Insight.

![](assets/actions-data-sync-faq-4.png)

Per garantire che tutti i dati delle attività possano provenire da Marketo Engage, Sales Insight Actions sincronizza tutti i dati delle attività in Marketo Engage.

## Quali campi relativi ai record delle persone vengono sincronizzati da Marketo Engage alle azioni di Sales Insight? {#what-fields-sync}

Sono disponibili 11 campi sincronizzati da Marketo Engage alle azioni di Sales Insight:

* Nome
* Cognome
* ID contatto Salesforce
* ID lead Salesforce
* ID account Salesforce
* ID opportunità Salesforce
* ID Marketo
* Azienda
* Titolo
* E-mail
* Numero di telefono
* URL LinkedIn
* Origine

## I campi sincronizzati tra Marketo Engage e le azioni di Sales Insight sono configurabili? {#are-the-fields-that-sync-configurable}

La configurazione dei campi Marketo Engage sincronizzati con le azioni di Sales Insight non è disponibile, né è possibile mappare i campi. La sincronizzazione da Marketo associa automaticamente i campi Marketo standard ai campi standard nell’istanza Azione di vendita.

## Perché le azioni di Sales Insight dispongono di un proprio database? {#why-does-actions-have-its-own-database}

Sales Insight Actions dispone di una propria applicazione web con un database dedicato di persone e attività per fornire un&#39;area di lavoro ottimizzata creata e progettata per i team di vendita. Questo consente ai responsabili delle vendite e ai venditori di disporre di uno spazio per sviluppare e gestire la propria strategia di coinvolgimento   senza concedere l’accesso o i privilegi all’area di lavoro principale di Marketo Engage, ottimizzata per gli specialisti delle operazioni di marketing.

## Come vengono gestiti i duplicati? {#how-are-duplicates-handled}

Il database delle azioni di vendita sarà una copia delle persone qualificate (lead/contatti con un proprietario delle vendite) presenti nel database Marketo Engage. Ciò significa che se in Marketo sono presenti due record con lo stesso indirizzo e-mail, verrà creato un record duplicato in Azioni di vendita.

## Quanto tempo è necessario per completare la sincronizzazione iniziale? {#how-long-initial-sync}

Il processo iniziale per la sincronizzazione di tutti i dati dei lead di vendita in una nuova istanza Sales Insight Actions in genere elabora le persone a circa 1.000 ogni 1-2 minuti. Questa è solo una stima e può variare.

Una volta eseguita la sincronizzazione iniziale e tutti i lead di vendita sono stati inseriti nell’istanza dell’app Web Sales Insight Actions, verrà eseguita una sincronizzazione incrementale ogni volta che si aggiorna uno dei campi supportati sincronizzati.

## Gli utenti di Azioni di Insight per le vendite possono modificare i dati relativi alle persone dall’app web Actions? {#can-actions-users-edit-people-data}

No, la possibilità di creare e modificare i record di persone in Actions non è disponibile sia per gli utenti che per gli amministratori dell&#39;app web Actions. La creazione e la modifica delle persone devono essere eseguite in Salesforce o Marketo Engage. Sales Insight Actions utilizza Marketo come fonte di verità per i dati delle persone sincronizzando continuamente nuovi dati, quindi se una persona viene aggiornata o creata in Marketo da un flusso di lavoro in Marketo o sincronizzata da Salesforce, tali aggiornamenti verranno passati al database dell&#39;app Web Sales Insight Actions.

## Le attività di vendita accedono a Marketo? {#do-sales-activities-log-to-marketo}

Sì, le attività di coinvolgimento vendite accederanno a Marketo come attività native. Queste attività includono anche filtri nativi che possono essere utilizzati con vincoli per eseguire il targeting dei lead in base agli attributi dell’attività di vendita.

![](assets/actions-data-sync-faq-5.png)

Di seguito è riportato un elenco delle attività che accedono a Marketo:

* Invia e-mail vendite
* Apri e-mail vendite
* Fai clic sull’e-mail vendite
* Risposta all&#39;e-mail di vendita
* E-mail di vendita non recapitata
* Chiamata di vendita ricevuta
* Aggiungi a campagna di vendita
* Rimosso dalla campagna di vendita

## Le attività di vendita accedono a Salesforce? {#do-sales-activities-log-to-salesforce}

Sì, le attività di coinvolgimento vendite accederanno a Salesforce come attività native. Queste attività possono quindi essere utilizzate nei rapporti di Salesforce per alimentare dashboard del team che tengono traccia delle attività di vendita.

Azioni di Insight per le vendite consente agli amministratori di configurare le attività di vendita registrate in Salesforce. Queste attività includono e-mail, chiamate e attività di promemoria aperte.

![](assets/actions-data-sync-faq-6.png)

Il diagramma precedente mostra quali informazioni vengono registrate in Salesforce. Attività quali e-mail e chiamate vengono registrate in Salesforce in [sincronizzazione unidirezionale](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md). [Annullamenti abbonamenti](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md) e [Le attività promemoria](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md) sono sempre aggiornate con una sincronizzazione bidirezionale. Ognuna di queste sincronizzazioni dati è configurabile dall’interfaccia dell’app web Sales Insight Actions.

>[!MORELIKETHIS]
>
>* [Sincronizzazione delle sottoscrizioni annullate con Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md)
>* [Verifica annullamento abbonamento Marketo](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md)
>* [Sincronizza attività di vendita con Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md)
>* [Sincronizzazione attività promemoria con Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md)
>* [Avvia sincronizzazione dati](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.md#initiate-data-sync)
