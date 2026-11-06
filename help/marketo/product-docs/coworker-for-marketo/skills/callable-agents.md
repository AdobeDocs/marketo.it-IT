---
description: Utilizza gli agenti richiamabili in CX Enterprise Coworker for Marketo Engage per eseguire passaggi di intelligenza artificiale in campagne intelligenti che puliscono, classificano, arricchiscono o schermano i dati dei lead.
title: Agenti chiamabili
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
source-git-commit: 16b8e470bd4a4460c0179ccdd406ef89af7e9e17
workflow-type: tm+mt
source-wordcount: '1957'
ht-degree: 1%
---
# Agenti chiamabili {#callable-agents}

Gli agenti richiamabili consentono di utilizzare un agente di intelligenza artificiale come passaggio in una campagna Marketo Engage Smart. Crea un agente in CX Enterprise Coworker per Marketo Engage, scegli i campi lead che legge e aggiorna e pubblicalo per l’utilizzo nelle campagne. Gli agenti possono aiutare a pulire i dati, classificare i lead, arricchire le informazioni mancanti o inviare gli schermi sotto forma di moduli.

>[!PREREQUISITES]
>
>Devi disporre dell&#39;autorizzazione **Amministratore degli accessi** in Marketo Engage.

## Prima di iniziare {#before-you-begin}

- Decidi quali campi lead l’agente deve leggere e quali campi deve aggiornare. Ogni input e output deve essere mappato su un campo lead di Marketo Engage.
- Verifica che i campi di output siano aggiornabili. I campi di sola lettura e i campi dei membri del programma non sono supportati.

## Come usare {#how-to-use}

1. Nel Marketo personale, fare clic sul riquadro **[!UICONTROL CX Enterprise Coworker for Marketo Engage]**.

1. Selezionare **[!UICONTROL Callable agents]** nel menu di navigazione a sinistra. L’elenco mostra il nome, la data di creazione, l’autore e lo stato di ciascun agente. Cerca per nome o ordina per nome o data di creazione.

1. Seleziona **[!UICONTROL Create callable agent]**. Scegli un modello o lascia vuoto il selettore modelli per iniziare da zero.

1. Immettere un **[!UICONTROL Agent name]** e scrivere **[!UICONTROL Agent instructions]** descrivendo la modalità di elaborazione di ogni lead.

1. In **[!UICONTROL Lead fields to send]**, aggiungi i campi lead necessari all&#39;agente come input. In **[!UICONTROL Lead fields to update]**, aggiungi ogni valore che l&#39;agente deve restituire e mappalo su un campo lead aggiornabile.

1. Selezionare **[!UICONTROL Save]** per salvare una bozza oppure **[!UICONTROL Save and publish]** per rendere l&#39;agente disponibile in Marketo Engage.

1. Aprire una campagna avanzata e selezionare la scheda **[!UICONTROL Flow]**. Nella sezione Marketing dell&#39;elenco dei passaggi del flusso, individua **Agente di chiamata: _[Nome agente]_**e trascinalo nel flusso.

1. Prova la campagna con un piccolo set di lead. Rivedi il registro attività e verifica che i campi di output si aggiornino come previsto prima di attivare la campagna per tutti i lead.

## Aspetti da considerare {#things-to-note}

- Un agente chiamabile elabora ogni lead in modo indipendente. Marketo Engage invia i valori dei lead mappati all’agente, scrive i valori restituiti nei campi dei lead mappati e continua con il passaggio successivo della campagna.
- Puoi creare e gestire agenti chiamabili in CX Enterprise Coworker for Marketo Engage. Non è richiesta alcuna connessione esterna.
- Gli agenti pubblicati non sono modificabili. Per modificare un agente già pubblicato, è necessario creare un nuovo agente e aggiornare le campagne Smart pertinenti.

## Creare un agente {#create-an-agent}

### Creare un agente da zero {#create-an-agent-from-scratch}

Lascia vuoto il selettore modelli. Il modulo inizia con un campo di input vuoto e un campo di output vuoto. Immetti il nome e le istruzioni, quindi configura i campi di input e output in modo che corrispondano alla regola business.

### Iniziare da un modello {#start-from-a-template}

Scegli un modello per precompilare le istruzioni, i campi di input e i campi di output. L&#39;agente viene salvato come copia personalizzata, che è possibile modificare o eliminare. Se elimini un agente creato da un modello, il modello diventa nuovamente disponibile nel selettore.

| Modello | Finalità | Input | Uscite |
| --- | --- | --- | --- |
| Nome società Normalizer | Pulisce i nomi delle aziende rimuovendo i suffissi legali, correggendo errori di battitura comuni e applicando la capitalizzazione del marchio standard. | Azienda | Società normalizzata (testo); affidabilità (numero) |
| Telefono E.164 Formatter | Formatta i numeri di telefono con lo standard internazionale E.164. | Telefono | Telefono normalizzato (testo); affidabilità (numero) |
| Standardizzazione posizione lavorativa | Standardizza le qualifiche professionali e deriva l&#39;anzianità. | Titolo | Titolo normalizzato (testo); anzianità (C-Level, VP, Director, Manager, Individual o Unknown); affidabilità |
| Rilevatore bot e spam | Segnala l’invio di moduli bot o spam. | E-mail, Nome, Cognome, Società, Telefono | È bot (true/false); affidabilità; motivo; flag (separati da virgola) |
| Rilevamento e-mail usa e getta | Identifica gli indirizzi e-mail temporanei o usa e getta. | E-mail | È bot (vero/falso); affidabilità; motivo; tipo di e-mail (usa e getta, personale o aziendale) |
| Classificatore lead | Segmenta i lead per dimensione dell’azienda, settore, persona e intento. | Società, Titolo, E-mail, Dipendenti, Entrate | Segmento (Enterprise, Mid-Market, SMB, Startup o Unknown); settore; persona; livello intento (High, Medium o Low); affidabilità |
| Arricchimento lead | Deduce i dettagli del lead mancanti dalle informazioni disponibili. | E-mail, Titolo, Società | Società, reparto, anzianità dedotta, entità con potere decisionale (vero/falso), B2B (vero/falso), affidabilità |
| Ricerca società | Genera informazioni sulle vendite dalle informazioni aziendali. | Azienda, sito Web, descrizione | Vedi il modello per l’elenco completo |

### Scrivi istruzioni valide {#write-effective-instructions}

- Inserisci regole generali ed esempi nelle istruzioni dell&#39;agente. Utilizzare le istruzioni dei campi per specificare le aspettative per un singolo output.
- Siate specifici. Ad esempio, &quot;Rimuovere i suffissi legali come Inc, LLC e Corp&quot; è più chiaro di &quot;pulire i nomi delle società&quot;.
- Includi esempi di input e output previsti, in particolare per i casi edge.
- Indica cosa deve restituire l’agente quando non è in grado di decidere, ad esempio &quot;In caso di dubbi, restituisce il valore originale.&quot;
- Aggiungi un output di affidabilità in modo che la logica della campagna possa instradare i risultati a bassa affidabilità per la revisione.
- Mantenere concisi i prompt. I prompt più brevi vengono eseguiti più rapidamente e a costi inferiori.

## Salvare, pubblicare e gestire gli agenti {#save-publish-and-manage-agents}

### Salva come bozza o pubblicazione {#save-as-a-draft-or-publish}

Selezionare **[!UICONTROL Save]** per salvare l&#39;agente come bozza. Le bozze possono essere modificate ma non sono disponibili come passaggi di flusso di Smart Campaign. Selezionare **[!UICONTROL Save and publish]** quando l&#39;agente è pronto. Marketo Engage rende l’agente disponibile come passaggio di flusso e ti riporta all’elenco degli agenti con una conferma della pubblicazione. Seleziona **[!UICONTROL Cancel]** per uscire senza salvare.

| Stato | Significato | Azione disponibile |
| --- | --- | --- |
| Bozza | L&#39;agente viene salvato ma non è disponibile in Marketo Engage. | Modificalo, quindi seleziona **[!UICONTROL Save and publish]** quando è pronto. |
| Pubblicato | L’agente è disponibile in Smart Campaigns. Gli agenti pubblicati sono congelati. | Utilizza l’agente pubblicato oppure crea un nuovo agente per apportare modifiche. |
| Pubblicazione non riuscita | Marketo Engage ha rifiutato l&#39;agente, ad esempio perché il nome di un campo di output è riservato. Ma l&#39;agente viene comunque salvato come bozza. | Modifica l’agente, correggi il campo denominato nel messaggio e pubblica di nuovo. |

### Modifica, controlla l’utilizzo o elimina {#edit-check-usage-or-delete}

- Seleziona **[!UICONTROL Edit]** su una bozza per modificarla. **[!UICONTROL Save]** ti mantiene sulla pagina e mostra una conferma di &quot;Agente salvato&quot;. È inoltre possibile selezionare **[!UICONTROL Save and publish]**, **[!UICONTROL Cancel]** o **[!UICONTROL Delete]**.
- Gli agenti pubblicati vengono congelati perché le campagne avanzate possono dipendere da essi. Crea un nuovo agente per apportare modifiche.
- Selezionare **[!UICONTROL Used by]** per vedere quali campagne Smart fanno riferimento a un agente prima di eliminare un agente o di modificarne la configurazione della campagna.
- Non è possibile eliminare un agente mentre è ancora utilizzato da una campagna avanzata. Rimuovi il passaggio di flusso dell’agente da ciascuna campagna elencata, quindi elimina l’agente.

## Integrazione delle regole organizzative {#organizational-rules-integration}

### Convenzioni di denominazione {#naming-conventions}

- **Nome agente:** da 1 a 100 caratteri e univoco all&#39;interno della sottoscrizione. Il nome viene utilizzato anche nel passaggio di flusso di Smart Campaign. Scegliere un nome riconoscibile, ad esempio `Company Name Normalizer`.
- **Nome campo di output:** Utilizzare lettere, cifre e caratteri di sottolineatura. Il nome deve iniziare con una lettera o un carattere di sottolineatura, essere univoco e non superare i 64 caratteri.
- **Nomi riservati:** Alcuni nomi di output sono riservati per l&#39;utilizzo del sistema. Se un nome viene rifiutato, scegliere un altro nome, ad esempio `qualificationReason` anziché `reason`.

### Elementi obbligatori e campi supportati {#required-elements-and-supported-fields}

- Mappa ogni campo di input su un campo lead di Marketo Engage prima di salvarlo.
- Configura almeno un campo di output. Mappa ogni output su un campo lead aggiornabile; i campi di sola lettura non sono disponibili nel selettore campi.
- I campi dei membri del programma non sono supportati. Il selettore di campi mostra solo i campi lead.
- I tipi di output supportati sono **Text**, **Number** e **True/False**.
- Per restituire un elenco, utilizza un valore di testo separato da virgole e descrivi il formato previsto nelle istruzioni del campo.
- Ogni esecuzione corretta restituisce esattamente i campi di output configurati.

### Limiti {#limits}

| Impostazione | Limite |
| --- | --- |
| Nome agente | 1-100 caratteri; univoco nell’abbonamento |
| Istruzioni agente | 1-4.000 caratteri |
| Campi di input | Fino a 20; ciascuno deve essere mappato su un campo lead |
| Campi di output | 1-20; ogni deve essere mappata a un campo lead aggiornabile |
| Nome campo di output | Fino a 64 caratteri; lettere, cifre e caratteri di sottolineatura; inizia con una lettera o un carattere di sottolineatura; univoco |
| Istruzioni campo di output | Fino a 512 caratteri |
| Lead per richiesta | Fino a 1.000 lead da Marketo Engage, elaborati in parallelo |

## Screening dei contenuti e gestione dei dati {#content-screening-and-data-handling}

Quando crei un agente o ne modifichi le istruzioni, Marketo Engage controlla le istruzioni dell’agente e le istruzioni del campo di output per individuare eventuali violazioni dei criteri, iniezioni tempestive e tentativi di exfiltrazione dei dati. Alcuni esempi includono le richieste di visualizzazione delle credenziali o di sostituzione del comportamento dell’agente. Se il contenuto è contrassegnato, il salvataggio viene bloccato e può essere visualizzato un messaggio di tipo &quot;Il prompt contiene contenuto con restrizioni&quot; o &quot;Richiesta di moderazione non riuscita del contenuto&quot;. Rivedi il testo e salva di nuovo.

- **L&#39;accesso:** La gestione degli agenti richiede l&#39;autorizzazione **Amministratore accesso**. Gli agenti e la cronologia delle chiamate sono isolati per iscrizione.
- **Protezione dati lead:** I dati del lead vengono passati separatamente dalle istruzioni dell&#39;agente, con protezioni che trattano i valori del lead come dati anziché come comandi.
- **Criterio contenuto:** se i dati di un lead violano il criterio contenuto del provider di IA, il lead riceve un&#39;attività di errore anziché un risultato.
- **Mantenimento:** i payload di richieste e risposte, inclusi i valori dei campi lead inviati all&#39;agente, vengono conservati nella cronologia delle chiamate per 30 giorni per supportare la risoluzione dei problemi, quindi eliminati automaticamente.

## Esecuzione degli agenti chiamabili in una campagna {#how-callable-agents-run-in-a-campaign}

1. Durante l’esecuzione della campagna, Marketo Engage invia all’agente i valori dei campi lead mappati per ciascun lead qualificato.
1. L’agente elabora ogni lead in modo indipendente e restituisce i campi di output configurati.
1. Marketo Engage scrive i risultati nei campi lead mappati. I campi modificati vengono visualizzati anche come attività standard di modifica del valore dei dati.
1. La campagna passa al passaggio successivo.

Elaborazione asincrona. Il passaggio di flusso attende un risultato fino alla finestra di attesa del passaggio di flusso in Marketo Engage. Se un lead non riesce (ad esempio a causa di un timeout), riceve un’attività di errore e gli altri lead continuano. Ogni risultato viene visualizzato nel registro attività del lead per l&#39;agente chiamabile.

Utilizza i campi di output nella logica della campagna. Ad esempio, il ramo in **È bot** per instradare le richieste di posta indesiderata in modo diverso, oppure il ramo in **affidabilità** per inviare risultati con bassa affidabilità a un passaggio di revisione.

## Controllo di qualità pre-attivazione {#pre-activation-qa}

Prima di attivare una campagna per tutti i lead:

- Esegui la campagna con un piccolo set di test di lead.
- Rivedi il registro attività di ciascun lead e verifica che i campi di output siano stati aggiornati correttamente.
- Casi limite del test, inclusi valori mancanti e input insoliti.
- Conferma che i rami della campagna gestiscano valori quali affidabilità bassa o classificazione bot/spam come previsto.

## Casi di utilizzo {#use-cases}

- **Pulizia dati:** standardizzare i nomi delle società, formattare i numeri di telefono in E.164 e normalizzare i titoli dei processi al momento della creazione o dell&#39;importazione dei lead.
- **Screening dei bot e dello spam:** Controlla gli invii per nomi incomprensibili, e-mail sospette e numeri di telefono a cifre ripetute. Disconnetti la campagna in base al risultato.
- **Rilevamento e-mail usa e getta:** Identificare gli indirizzi e-mail temporanei e indirizzarli in modo diverso rispetto agli indirizzi aziendali.
- **Classificazione lead:** lead di segmento per dimensione dell&#39;azienda, settore, persona e intento di supportare il routing o il punteggio.
- **Arricchimento lead:** dedurre i dettagli mancanti come reparto, anzianità o se un lead è un responsabile delle decisioni.
- **Regole personalizzate:** Crea un controllo o una categorizzazione Sì/No che può essere descritta come regola di elaborazione dei lead, ad esempio contrassegnare i lead da un&#39;area geografica o da un settore.

## Risoluzione dei problemi {#troubleshooting}

| Problema | Risoluzione |
| --- | --- |
| **Gli agenti** non vengono visualizzati nella navigazione. | Chiedi all&#39;amministratore di Marketo Engage di concedere l&#39;autorizzazione **Amministratore accesso**. |
| Il salvataggio è bloccato con un messaggio di contenuto. | Rivedi le istruzioni dell’agente o le istruzioni del campo per rimuovere il contenuto contrassegnato, quindi salva di nuovo. |
| Lo stato dell&#39;agente è **Pubblicazione non riuscita**. | Modificare l&#39;agente, correggere il campo denominato nel messaggio e selezionare **Salva e pubblica**. |
| Impossibile modificare un agente pubblicato. | Gli agenti pubblicati sono congelati. Crea un nuovo agente per apportare modifiche. |
| Impossibile eliminare un agente. | Rimuovi il relativo passaggio di flusso da ciascuna Smart Campaign elencata come utilizzando l’agente, quindi eliminalo. |
| Un nome di campo viene segnalato come riservato. | Scegliere un nome di campo di output diverso, ad esempio `qualificationReason`, e salvare di nuovo. |
| Alcuni lead ricevono un’attività di errore. | Controllare il registro attività del lead. Singoli errori, inclusi timeout o violazioni dei criteri dei contenuti, non influiscono su altri lead. |
| Risultati imprevisti. | Rendi le istruzioni più specifiche, aggiungi esempi, perfeziona le istruzioni sul campo e testa di nuovo con un piccolo set di lead. |

## Passaggi successivi {#next-steps}

- Rivedi l&#39;elenco **Usato da** dell&#39;agente e conferma quali campagne Smart lo utilizzeranno.
- Testa il passaggio di flusso con un piccolo gruppo di lead e convalida i registri attività e i campi di output.
- Utilizza i campi di output per aggiungere rami della campagna per le classificazioni o i risultati a bassa affidabilità.
- Prima di eliminare l’agente, rimuovi il passaggio di flusso dell’agente da tutte le campagne.
