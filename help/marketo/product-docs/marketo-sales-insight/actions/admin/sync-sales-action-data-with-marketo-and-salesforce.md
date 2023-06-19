---
description: Sincronizzare i dati relativi alle azioni di vendita con Marketo e Salesforce - Documenti Marketo - Documentazione del prodotto
title: Sincronizzare i dati relativi alle azioni di vendita con Marketo e Salesforce
exl-id: bb213d50-be22-492d-b74c-b8cfb834b2ca
source-git-commit: 02354356949aef7aa8836d4753ec538b7819a65a
workflow-type: tm+mt
source-wordcount: '1064'
ht-degree: 1%

---

# Sincronizzare i dati relativi alle azioni di vendita con Marketo e Salesforce {#sync-sales-action-data-with-marketo-and-salesforce}

La sincronizzazione dei campi di unificazione dei dati per le azioni di approfondimento sulle vendite consente al sistema di richiamare le informazioni sulle persone dal database del Marketo Engage nel database delle azioni di approfondimento sulle vendite.

Questo fornisce dati aggiornati sulle persone nell’app web Sales Insight Actions e consente al sistema di raccogliere ID univoci per i record corrispondenti delle persone in Marketo e nei record lead/contatto/account/opportunità in Salesforce, in modo da poter fare riferimento correttamente ai record per la registrazione dei dati.

Questa sincronizzazione può essere abilitata dalla scheda Configurazione azioni di Sales Insight nella sezione Admin del Marketo Engage. Per ulteriori informazioni, consulta [Avvia sincronizzazione dati](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.md#initiate-data-sync).

![](assets/actions-data-sync-faq-1.png)

Il diagramma precedente mostra come l’attività delle persone e i dati delle attività possono essere sincronizzati tra i sistemi. Alcune cose da notare:

* I record Persone vengono sincronizzati con le azioni di Sales Insight dal Marketo Engage, rendendo il Marketo Engage la fonte di verità per i dati sulle persone delle azioni di Sales Insight
* Azioni Marketo Engage e approfondimento vendite [disporre di un meccanismo](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md) per raccogliere e sincronizzare lo stato di annullamento dell’iscrizione a Salesforce
* Lo stato di annullamento dell’iscrizione non viene sincronizzato dalle azioni di vendita al Marketo Engage, ma è possibile configurare le azioni di approfondimento sulle vendite per verificare lo stato di annullamento dell’iscrizione a Marketo delle persone prima di consentire ai venditori di inviare un’e-mail con [Verifica annullamento iscrizione Marketo](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md).

Di seguito sono riportate alcune domande frequenti relative al funzionamento della sincronizzazione di unificazione dei dati.

## Quali lead/contatti sono sincronizzati con le azioni di approfondimento sulle vendite? {#what-lead-contacts-are-synced}

![](assets/actions-data-sync-faq-2.png)

I lead e i contatti a cui è assegnato un proprietario vendite verranno sincronizzati in Azioni di vendita.

Puoi verificare se un lead/contatto ha un proprietario vendite in Salesforce osservando il campo del proprietario standard esistente.

Il proprietario delle vendite non deve essere l&#39;utente di sincronizzazione Marketo o un utente Salesforce o di vendita specifico. Tutto ciò che ci serve è che ci sia un utente elencato nel campo proprietario del lead e proprietario del contatto elencato in Salesforce, in modo da poterlo identificare come lead di vendita e sincronizzarlo con le azioni di Sales Insight. Eventuali aggiornamenti ai campi con cui eseguiamo la sincronizzazione verranno rilevati e aggiornati anche in Azioni approfondimenti vendite.

## Da dove vengono originati i dati dell’attività visualizzati nella griglia avanzata di Sales Insight? {#where-does-the-activity-data-get-sourced-from}

![](assets/actions-data-sync-faq-3.png)

I dati dell’attività come e-mail, chiamate, momenti di interesse e web, provengono tutti dal database del Marketo Engage. Lo Smart Grid di Sales Insight invia una richiesta all’istanza di Marketo Engage per recuperarla ogni volta che un utente di vendita carica il pannello di Sales Insight.

![](assets/actions-data-sync-faq-4.png)

Per garantire che tutti i dati relativi all’attività possano provenire dal Marketo Engage, Sales Insight Actions sincronizza tutti i dati relativi all’attività nel Marketo Engage.

## Quali campi relativi ai record delle persone vengono sincronizzati dal Marketo Engage alle azioni di approfondimento sulle vendite? {#what-fields-sync}

Sono disponibili 11 campi che si sincronizzano tra il Marketo Engage e le azioni di approfondimento sulle vendite:

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

## I campi sincronizzati tra Marketi Engage e le azioni di approfondimento sulle vendite sono configurabili? {#are-the-fields-that-sync-configurable}

La configurazione dei campi Marketo Engage sincronizzati con le azioni di approfondimento sulle vendite non è disponibile, né è possibile mappare i campi. La sincronizzazione da Marketo associa automaticamente i campi Marketo standard ai campi standard nell’istanza Azione di vendita.

## Perché le azioni Sales Insight dispongono di un proprio database? {#why-does-actions-have-its-own-database}

Sales Insight Actions dispone di una propria applicazione web con un database dedicato di persone e attività per fornire un&#39;area di lavoro ottimizzata creata e progettata per i team di vendita. Questo consente ai responsabili vendite e ai venditori di disporre di uno spazio per sviluppare e gestire la propria strategia di coinvolgimento senza concedere l&#39;accesso o i privilegi all&#39;area di lavoro principale del Marketo Engage, ottimizzata per gli specialisti delle operazioni di marketing.

## Come vengono gestiti i duplicati? {#how-are-duplicates-handled}

Il database delle azioni di vendita sarà una copia delle persone qualificate (lead/contatti con un proprietario delle vendite) presenti nel database di Marketo Engage. Ciò significa che se in Marketo sono presenti due record con lo stesso indirizzo e-mail, verrà creato un record duplicato in Azioni di vendita.

## Quanto tempo è necessario per completare la sincronizzazione iniziale? {#how-long-initial-sync}

Il processo iniziale per la sincronizzazione di tutti i dati dei lead di vendita in una nuova istanza di Sales Insight Actions in genere elabora le persone a circa 1.000 ogni 1-2 minuti. Questa è solo una stima e può variare.

Una volta eseguita la sincronizzazione iniziale e tutti i lead di vendita sono stati inseriti nell’istanza dell’app Web Sales Insight Actions, verrà eseguita una sincronizzazione incrementale ogni volta che si aggiorna uno dei campi supportati sincronizzati.

## Gli utenti di Azioni approfondimento vendite possono modificare i dati relativi alle persone dall’app web Azioni? {#can-actions-users-edit-people-data}

No, la possibilità di creare e modificare i record di persone in Actions non è disponibile sia per gli utenti che per gli amministratori dell&#39;app web Actions. La creazione e la modifica delle persone devono essere eseguite in Salesforce o Marketi Engage. Sales Insight Actions utilizza Marketo come fonte di verità per i dati delle persone sincronizzando continuamente nuovi dati, quindi se una persona viene aggiornata o creata in Marketo da un flusso di lavoro in Marketo o sincronizzata da Salesforce, tali aggiornamenti verranno passati al database dell&#39;app web Sales Insight Actions.

## Le attività di vendita accedono a Marketo? {#do-sales-activities-log-to-marketo}

Sì, le attività di coinvolgimento vendite accederanno a Marketo come attività native. Queste attività includono anche filtri nativi che possono essere utilizzati con vincoli per eseguire il targeting dei lead in base agli attributi dell’attività di vendita.

![](assets/actions-data-sync-faq-5.png)

Di seguito è riportato un elenco delle attività che accedono a Marketo:

* Invia e-mail vendite
* Apri e-mail vendite
* Fai clic su E-mail vendita
* Risposta all&#39;e-mail di vendita
* E-mail di vendita non recapitata
* Chiamata di vendita ricevuta
* Aggiungi a campagna di vendita
* Rimosso dalla campagna di vendita

## Le attività di vendita accedono a Salesforce? {#do-sales-activities-log-to-salesforce}

Sì, le attività di coinvolgimento vendite accederanno a Salesforce come attività native. Queste attività possono quindi essere utilizzate nei rapporti Salesforce per alimentare dashboard del team che tengono traccia delle attività di vendita.

Le azioni di approfondimento sulle vendite consentono agli amministratori di configurare le attività di vendita registrate in Salesforce. Queste attività includono e-mail, chiamate e attività di promemoria aperte.

![](assets/actions-data-sync-faq-6.png)

Il diagramma precedente mostra quali informazioni vengono registrate in Salesforce. Attività come e-mail e chiamate vengono registrate in Salesforce in un [sincronizzazione unidirezionale](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md). [Annulla iscrizione](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md) e [Attività promemoria](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md) vengono mantenuti aggiornati con una sincronizzazione bidirezionale. Ognuna di queste sincronizzazioni dati è configurabile dall’interfaccia dell’app web Sales Insight Actions.

>[!MORELIKETHIS]
>
>* [Sincronizzazione degli annullamenti di abbonamenti con Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md)
>* [Verifica annullamento iscrizione Marketo](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md)
>* [Sincronizza attività di vendita con Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md)
>* [Sincronizzazione attività promemoria con Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md)
>* [Avvia sincronizzazione dati](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.md#initiate-data-sync)
