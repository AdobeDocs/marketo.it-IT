---
description: Utilizza Marketo AI per creare un programma Marketo da una descrizione in linguaggio semplice. Prepara campagne intelligenti, pianificazione e segnaposto per le risorse per la revisione e il perfezionamento.
title: Creare programmi
badge: Beta
hide: true
source-git-commit: f2be5a29916b48fd0ba4932925aa4826b7f4ee7f
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 0%

---

# Creare programmi {#build-programs}

Descrivi una campagna di marketing in linguaggio semplice e Marketo AI crea la struttura del programma, completa di segnaposto delle risorse e pianificazione.

>[!PREREQUISITES]
>
>* Per utilizzare questa funzione devi prima accettare i [termini Gen-AI di base e i termini supplementari](https://www.adobe.com/legal/terms/enterprise-licensing/genai-ww.html){target="_blank"}. Per informazioni, contatta il team dell’account di Adobe (il tuo account manager).
>
>* È necessario disporre dell&#39;autorizzazione per la creazione di programmi nell&#39;account Marketo.

>[!AVAILABILITY]
>
>Questa funzione è attualmente in versione beta chiusa. Non divulgare questa documentazione.

## Come usare {#how-to-use}

1. In Il mio Marketo, fai clic sul riquadro **Genera con IA**.

1. Nella finestra del prompt, digita una descrizione della campagna da creare. Essere specifici o generali come si desidera (è sempre possibile perfezionare).

1. Marketo AI conferma l’interpretazione del tuo resoconto ed elenca cosa intende creare. Rivedi questo prima che venga compilato.

1. Conferma e Marketo AI crea il programma nel tuo ambiente.

1. Apri il nuovo programma creato in Marketo e controlla la struttura.

1. Sostituisci le risorse e-mail segnaposto con il contenuto effettivo.

1. Verifica che i filtri e i passaggi di flusso delle campagne intelligenti corrispondano al pubblico e alla logica previsti.

1. Esegui l&#39;agente di controllo qualità [Programma](/help/marketo/product-docs/marketo-ai/agents/program-qa.md) prima dell&#39;attivazione.

## Casi d’uso {#use-cases}

**Programma di registrazione webinar**: un gestore di campagne digita &quot;Crea un programma di registrazione webinar per la demo del prodotto di agosto. Invia un’e-mail di invito, un promemoria il giorno prima e un follow-up con il collegamento di registrazione in seguito.&quot; Marketo AI crea un programma con tre campagne intelligenti (invito, promemoria, follow-up), e-mail segnaposto per ciascuna e pianificazione in base alla data dell’evento.

**Campagna trigger punteggio lead**: un esperto di operazioni di marketing di tipo &quot;Genera un programma che viene attivato quando un lead raggiunge un punteggio di 50 e lo invia a un elenco avanzato MQL&quot;. Marketo AI crea il programma con una campagna trigger in ascolto della modifica del punteggio e un passaggio di flusso che aggiunge il lead all’elenco MQL.

**Alimentazione di ricoinvolgimento**: un responsabile della generazione della domanda richiede una serie di ricoinvolgimento di 3 e-mail per i lead che non si impegnano da 90 giorni. Marketo AI crea la campagna batch con il filtro di inattività, tre passaggi di invio e-mail con i passaggi di attesa appropriati tra loro e un passaggio di flusso per aggiornare lo stato del lead se qualcuno si riattiva.

**Programma di follow-up eventi**: dopo una fiera, un manager chiede ad Marketo AI di creare un programma di follow-up post-evento che invia un&#39;e-mail di ringraziamento ai partecipanti e un&#39;e-mail di mancato consenso ai partecipanti che non sono stati visualizzati. Marketo AI crea due campagne intelligenti, una per ogni segmento, con i filtri e i segnaposto e-mail corretti.

## Aspetti da considerare {#things-to-note}

* Avere un’idea chiara di cosa dovrebbe fare la campagna, chi è il pubblico, quale azione lo attiva (o se si tratta di un invio in batch) e qual è l’obiettivo.
* Non sono richiesti modelli o moduli iniziali. Marketo AI crea la struttura e successivamente puoi collegare le risorse (sei ancora responsabile della scrittura della copia e-mail e della configurazione di eventuali pagine di destinazione).
* Marketo AI non può accedere automaticamente agli elenchi di pubblico esistenti. Dopo aver creato il programma, è necessario collegare i filtri per elenchi avanzati ai segmenti effettivi.
* I programmi con più passaggi complessi con logica di diramazione avanzata possono richiedere un perfezionamento manuale dopo la creazione.
* Se l’ambiente Marketo utilizza convenzioni di denominazione o strutture di cartelle, specificale nella descrizione in modo che il programma venga creato nella posizione giusta.
