---
description: Domande frequenti sulla sincronizzazione dei dati delle azioni - Documentazione di Marketo - Documentazione del prodotto
title: Domande frequenti sulla sincronizzazione dei dati delle azioni
feature: Sales Insight Actions
exl-id: bb213d50-be22-492d-b74c-b8cfb834b2ca
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '958'
ht-degree: 1%

---

# Domande frequenti sulla sincronizzazione dei dati delle azioni {#actions-data-sync-faq}

La sincronizzazione dei campi di unificazione dei dati per [!DNL Sales Insight Actions] consente al sistema di richiamare le informazioni personali dal database Marketo Engage nel database [!DNL Sales Insight Actions].

In questo modo vengono forniti dati aggiornati sulle persone nell&#39;app Web [!DNL Sales Insight Actions] e viene consentito di raccogliere ID univoci per i record corrispondenti delle persone in Marketo e nei record lead/contatto/account/opportunità in [!DNL Salesforce], in modo che sia possibile fare riferimento correttamente ai record per la registrazione dei dati.

Questa sincronizzazione può essere abilitata dalla scheda Configurazione [!DNL Sales Insight Actions] nella sezione Amministratore di Marketo Engage. Per ulteriori informazioni, vedi [Avvia sincronizzazione dati](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.md#initiate-data-sync).

![](assets/actions-data-sync-faq-1.png)

Il diagramma precedente mostra come l’attività delle persone e i dati delle attività possono essere sincronizzati tra i sistemi. Alcune cose da notare:

* I record di persone sono sincronizzati con [!DNL Sales Insight Actions] da Marketo Engage, rendendo Marketo Engage l&#39;origine della verità per i dati di [!DNL Sales Insight Actions] persone
* Sia Marketo Engage che [!DNL Sales Insight Actions] [dispongono di un meccanismo](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md) per raccogliere e sincronizzare lo stato di annullamento dell&#39;iscrizione a [!DNL Salesforce]
* Lo stato di annullamento abbonamento non viene sincronizzato da Azioni di vendita a Marketo Engage, ma è possibile configurare [!DNL Sales Insight Actions] per verificare lo stato di annullamento abbonamento a Marketo delle persone prima di consentire ai venditori di inviare un&#39;e-mail con [Verifica annullamento abbonamento a Marketo](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md).

Di seguito sono riportate alcune domande frequenti relative al funzionamento della sincronizzazione di unificazione dei dati.

## Quali lead/contatti sono sincronizzati in [!DNL Sales Insight Actions]? {#what-lead-contacts-are-synced}

![](assets/actions-data-sync-faq-2.png)

I lead e i contatti a cui è assegnato un proprietario vendite verranno sincronizzati in Azioni di vendita.

Per verificare se un lead/contatto ha un proprietario vendite in [!DNL Salesforce], esaminare il campo proprietario standard esistente.

Il proprietario delle vendite non deve essere l&#39;utente di sincronizzazione Marketo o un utente [!DNL Salesforce] o di vendita specifico. È sufficiente che un utente sia elencato nel campo proprietario lead e proprietario contatto elencato in [!DNL Salesforce] per identificarlo come lead di vendita e sincronizzarlo in [!DNL Sales Insight Actions]. Eventuali aggiornamenti ai campi sincronizzati verranno rilevati e aggiornati in [!DNL Sales Insight Actions].

## Da dove vengono originati i dati dell&#39;attività visualizzati nella griglia avanzata di Sales Insight? {#where-does-the-activity-data-get-sourced-from}

![](assets/actions-data-sync-faq-3.png)

I dati dell’attività come e-mail, chiamate, momenti di interesse e web provengono tutti dal database di Marketo Engage. Sales Insight Smart Grid invia una richiesta all’istanza di Marketo Engage per recuperarla ogni volta che un utente di vendita carica il pannello Sales Insight.

![](assets/actions-data-sync-faq-4.png)

Per garantire che tutti i dati delle attività possano essere originati da Marketo Engage, [!DNL Sales Insight Actions] sincronizza tutti i dati delle attività in Marketo Engage.

## Quali campi relativi ai record delle persone sono sincronizzati da Marketo Engage a [!DNL Sales Insight Actions]? {#what-fields-sync}

Sono 11 i campi sincronizzati da Marketo Engage a [!DNL Sales Insight Actions]:

* Nome
* Cognome
* ID contatto [!DNL Salesforce]
* ID lead [!DNL Salesforce]
* ID account [!DNL Salesforce]
* ID opportunità [!DNL Salesforce]
* ID Marketo
* Azienda
* Titolo
* E-mail
* Numero di telefono
* URL [!DNL Linkedin]
* Origine

## I campi sincronizzati tra Marketo Engage e [!DNL Sales Insight Actions] sono configurabili? {#are-the-fields-that-sync-configurable}

La configurazione dei campi di Marketo Engage sincronizzati con [!DNL Sales Insight Actions] non è disponibile e non è possibile mappare i campi. La sincronizzazione da Marketo associa automaticamente i campi Marketo standard ai campi standard nell’istanza Azione di vendita.

## Perché [!DNL Sales Insight Actions] ha un proprio database? {#why-does-actions-have-its-own-database}

[!DNL Sales Insight Actions] dispone di una propria applicazione Web con un database dedicato di persone e attività per fornire un&#39;area di lavoro ottimizzata creata e progettata per i team di vendita. Questo consente ai responsabili delle vendite e ai venditori di disporre di uno spazio per sviluppare e gestire la propria strategia di coinvolgimento   senza concedere l’accesso o i privilegi all’area di lavoro principale di Marketo Engage, ottimizzata per gli specialisti delle operazioni di marketing.

## Come vengono gestiti i duplicati? {#how-are-duplicates-handled}

Il database delle azioni di vendita sarà una copia delle persone qualificate (lead/contatti con un proprietario delle vendite) presenti nel database Marketo Engage. Ciò significa che se in Marketo sono presenti due record con lo stesso indirizzo e-mail, verrà creato un record duplicato in Azioni di vendita.

## Quanto tempo è necessario per completare la sincronizzazione iniziale? {#how-long-initial-sync}

Il processo iniziale per la sincronizzazione di tutti i dati dei lead di vendita in una nuova istanza [!DNL Sales Insight Actions] in genere elabora le persone a circa 1.000 ogni 1-2 minuti. Questa è solo una stima e può variare.

Una volta eseguita la sincronizzazione iniziale e tutti i lead di vendita sono stati inseriti nell&#39;istanza dell&#39;app Web [!DNL Sales Insight Actions], verrà eseguita una sincronizzazione incrementale ogni volta che si aggiorna uno dei campi supportati sincronizzati.

## Gli utenti di [!DNL Sales Insight Actions] possono modificare i dati relativi alle persone dall&#39;app Web Actions? {#can-actions-users-edit-people-data}

No, la possibilità di creare e modificare i record di persone in Actions non è disponibile sia per gli utenti che per gli amministratori dell&#39;app web Actions. La creazione e la modifica delle persone devono essere eseguite in [!DNL Salesforce] o Marketo Engage. [!DNL Sales Insight Actions] utilizza Marketo come fonte di verità per i dati delle persone sincronizzando continuamente i nuovi dati, pertanto se una persona viene aggiornata o creata in Marketo da un flusso di lavoro in Marketo o sincronizzata da [!DNL Salesforce], tali aggiornamenti verranno passati al database dell&#39;app Web [!DNL Sales Insight Actions].

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

## Le attività di vendita vengono registrate in [!DNL Salesforce]? {#do-sales-activities-log-to-salesforce}

Sì, le attività di coinvolgimento vendite accederanno a [!DNL Salesforce] come attività native. Queste attività possono quindi essere utilizzate nei report [!DNL Salesforce] per alimentare i dashboard del team che tengono traccia delle attività di vendita.

[!DNL Sales Insight Actions] consente agli amministratori di configurare le attività di vendita registrate in [!DNL Salesforce]. Queste attività includono e-mail, chiamate e attività di promemoria aperte.

![](assets/actions-data-sync-faq-6.png)

Il diagramma precedente mostra le informazioni registrate in [!DNL Salesforce]. Attività quali e-mail e chiamate vengono registrate in [!DNL Salesforce] in [sincronizzazione unidirezionale](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/salesforce-sync-settings.md). [Annullamenti abbonamenti](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md) e [Le attività promemoria](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md) sono sempre aggiornate con una sincronizzazione bidirezionale. Ognuna di queste sincronizzazioni dati è configurabile dall&#39;interfaccia dell&#39;app Web [!DNL Sales Insight Actions].

>[!MORELIKETHIS]
>
>* [Sincronizzazione delle sottoscrizioni annullate con [!DNL Salesforce]](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/syncing-unsubscribes-with-salesforce.md)
>* [Verifica annullamento abbonamento Marketo](/help/marketo/product-docs/marketo-sales-insight/actions/email/unsubscribes/marketo-unsubscribe-check.md)
>* [[!DNL Salesforce] Impostazioni sincronizzazione](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/salesforce-sync-settings.md)
>* [Sincronizzazione attività promemoria con [!DNL Salesforce]](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md)
>* [Avvia sincronizzazione dati](/help/marketo/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.md#initiate-data-sync)

