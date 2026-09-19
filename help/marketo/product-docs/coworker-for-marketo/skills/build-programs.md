---
description: Utilizza Coworker for Marketo Engage per creare un programma Marketo adattando un modello esistente. Prepara campagne avanzate, pianificazione e segnaposto per le risorse per la revisione e il perfezionamento.
title: Creare programmi
source-git-commit: fc1bcbdaa543e39127945852a6f89e69f2966c21
workflow-type: tm+mt
source-wordcount: '804'
ht-degree: 0%
---
# Creare programmi {#build-programs}

Descrivi una campagna di marketing in un linguaggio semplice e Coworker for Marketo Engage adatta un modello di programma esistente alle tue esigenze, aggiornando automaticamente il contenuto delle e-mail e creando risorse aggiuntive duplicando la struttura del modello.

Le [regole organizzative](/help/marketo/product-docs/coworker-for-marketo/organizational-rules.md){target="_blank"} della tua organizzazione guidano il modo in cui Coworker for Marketo Engage struttura e convalida il programma durante la creazione. Queste regole garantiscono che il nuovo programma sia allineato alle convenzioni di denominazione, ai token richiesti, alla struttura delle cartelle e agli standard di conformità.

>[!PREREQUISITES]
>
>* Per utilizzare questa funzione devi prima accettare i [termini Gen-AI di base e i termini supplementari](https://www.adobe.com/legal/terms/enterprise-licensing/genai-ww.html){target="_blank"}. Per informazioni, contatta il team dell’account di Adobe (il tuo account manager).
>
>* È necessario disporre dell&#39;autorizzazione per creare programmi nell&#39;account Marketo e disporre di almeno un programma Marketo esistente da utilizzare come modello. Il programma modello deve contenere almeno un’e-mail e una Smart Campaign.

## Come usare {#how-to-use}

1. Nel tuo My Marketo, fai clic sul riquadro **Collaboratore per Marketo Engage**.

1. Selezionare un programma modello. Scegli un programma esistente che corrisponda al tipo di campagna (ad esempio e-mail, webinar, Nurture).

1. Nella finestra del prompt, digita una descrizione della campagna da creare. Essere specifici o generali come si desidera (è sempre possibile perfezionare).

1. Coworker for Marketo Engage conferma l’interpretazione del tuo resoconto ed elenca i contenuti della sua attività. Rivedi questo prima che venga compilato.

1. Conferma e Collaboratore per Marketo Engage crea il programma nel tuo ambiente.

1. Apri il nuovo programma creato in Marketo e controlla la struttura.

1. Sostituisci le risorse e-mail segnaposto con il contenuto effettivo.

1. Verifica che i filtri e i passaggi del flusso di Smart Campaign corrispondano al pubblico e alla logica previsti.

1. Dopo aver completato tutti i perfezionamenti manuali (configurazione della logica di Smart Campaign, finalizzazione dei filtri, personalizzazione del contenuto delle e-mail), esegui [Convalida programmi](/help/marketo/product-docs/coworker-for-marketo/skills/validate-programs.md) per garantire che le modifiche siano conformi alle regole organizzative prima dell&#39;attivazione.

## Casi di utilizzo {#use-cases}

**Programma di registrazione webinar**: un gestore di campagne digita &quot;Crea un programma di registrazione webinar per la demo del prodotto di agosto. Invia un’e-mail di invito, un promemoria il giorno prima e un follow-up con il collegamento di registrazione in seguito.&quot; Collaboratore per Marketo Engage crea un programma con tre campagne avanzate (invito, promemoria, follow-up), e-mail segnaposto per ciascuna di esse e pianificazione in base alla data dell’evento.

**Campagna trigger punteggio lead**: un esperto di operazioni di marketing di tipo &quot;Genera un programma che viene attivato quando un lead raggiunge un punteggio di 50 e lo invia a un elenco avanzato MQL&quot;. Coworker for Marketo Engage crea il programma con una campagna trigger in ascolto della variazione di punteggio e un passaggio di flusso che aggiunge il lead all’elenco MQL.

**Alimentazione di ricoinvolgimento**: un responsabile della generazione della domanda richiede una serie di ricoinvolgimento di 3 e-mail per i lead che non si impegnano da 90 giorni. In Collaboratore per Marketo Engage viene creata la campagna batch con il filtro di inattività, tre passaggi di invio e-mail con i passaggi di attesa appropriati tra loro e un passaggio di flusso per aggiornare lo stato del lead se un utente si riattiva.

**Programma di follow-up eventi**: dopo una fiera, un manager chiede a Coworker per Marketo Engage di creare un programma di follow-up post-evento che invia un&#39;e-mail di ringraziamento ai partecipanti e un&#39;e-mail di mancato consenso agli iscritti che non sono stati visualizzati. Collaboratore per Marketo Engage crea due campagne avanzate, una per ogni segmento, con i filtri e i segnaposto e-mail corretti.

>[!NOTE]
>
>In ogni esempio precedente, Collaboratore clona un modello di programma esistente (un semplice programma e-mail o evento con struttura di base) e crea e-mail e campagne aggiuntive duplicando le risorse del modello e aggiornandone il contenuto. I passaggi di flusso e i filtri di Smart Campaign vengono adattati ove possibile, ma potrebbe essere necessario un perfezionamento manuale per corrispondere alla logica specifica della campagna.

## Aspetti da considerare {#things-to-note}

* Avere un’idea chiara di cosa dovrebbe fare la campagna, chi è il pubblico, quale azione lo attiva (o se si tratta di un invio in batch) e qual è l’obiettivo.
* È necessario selezionare un modello. Scegli un modello con almeno un messaggio e-mail e una campagna avanzata. Lo strumento non può funzionare con modelli vuoti.
* Il contenuto delle e-mail viene generato automaticamente, ma i filtri e i passaggi del flusso di Smart Campaign rimangono manuali. Dopo la creazione, devi configurare la logica in modo che corrisponda al comportamento previsto della campagna.
* Le risorse aggiuntive vengono create tramite duplicazione. Se la tua breve richiesta richiede 4 e-mail ma il modello ha 1, lo strumento crea 3 duplicati. Esamina tutti per coerenza; ereditano la struttura e la struttura del modello.
* Collaboratore per Marketo Engage non può accedere automaticamente agli elenchi di pubblico esistenti. Devi configurare manualmente i filtri per elenchi avanzati per eseguire il targeting dei segmenti effettivi dopo la creazione del programma.
* I programmi con più passaggi complessi con logica di diramazione avanzata possono richiedere un perfezionamento manuale dopo la creazione.
* Se l’ambiente Marketo utilizza convenzioni di denominazione o strutture di cartelle, specificale nella descrizione in modo che il programma venga creato nella posizione giusta.
