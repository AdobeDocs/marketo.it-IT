---
description: Scopri come le Regole organizzative definiscono gli standard di governance e guidano Collaboratore per Marketo Engage nella creazione di programmi, nella pianificazione delle campagne e nella convalida.
title: Regole organizzative
source-git-commit: 60ab04f79b2b24ca659676f5847d6f87b867e2f4
workflow-type: tm+mt
source-wordcount: '828'
ht-degree: 0%
---
# Regole organizzative {#organizational-rules}

Le Regole organizzative definiscono gli standard delle operazioni di marketing e i requisiti di governance in un unico documento che guida Collaboratore per Marketo Engage nella creazione di programmi, nella pianificazione delle campagne e nei flussi di lavoro di convalida.

## Cosa sono le regole organizzative? {#what-are-organizational-rules}

Le Regole organizzative sono un documento di configurazione basato su markdown che acquisisce gli standard della campagna della tua organizzazione:

* Convenzioni di denominazione per programmi, e-mail e campagne intelligenti
* Risorse e struttura richieste (cartelle, token, rapporti)
* Requisiti di conformità (collegamenti per annullare l’abbonamento, parametri UTM, filtri di esclusione)
* Best practice (progettazione di e-mail, configurazione di elenchi avanzati)

Ogni istanza di Marketo include regole organizzative predefinite. Puoi personalizzarli per riflettere le specifiche esigenze di governance della tua organizzazione.

## Dove vengono utilizzate le regole organizzative {#where-organizational-rules-are-used}

Guida alle regole organizzative Collaboratore per Marketo Engage in tre ambiti:

| Competenza | Modalità di applicazione delle regole |
| --- | --- |
| Programmi di build | Le regole guidano la creazione della struttura del programma, la denominazione e la configurazione iniziale. Coworker for Marketo Engage segnala eventuali problemi di conformità nella descrizione prima di creare il programma. |
| Pianificare campagne | Le regole informano su come Coworker per Marketo Engage struttura le campagne intelligenti, i filtri e i passaggi di flusso in base agli standard. |
| Convalida programmi | Le regole definiscono ciò che viene verificato da Coworker for Marketo Engage durante la convalida dei programmi prima dell’attivazione. |

## Come accedere e personalizzare le regole organizzative {#how-to-access-and-customize-organizational-rules}

1. Nel tuo My Marketo, fai clic sul riquadro **Collaboratore per Marketo Engage**.
1. Fai clic sull’icona a forma di ingranaggio.
1. Selezionare la scheda **Regole organizzative**.
1. Esamina le regole predefinite (che sono precompilate con le best practice per le operazioni di marketing).
1. Modifica le regole in modo che corrispondano a quelle della tua organizzazione:

   * Convenzioni di denominazione (programmi, e-mail, campagne)
   * Struttura di cartelle richiesta
   * Token e campi obbligatori
   * Norme di conformità ed esclusione

1. Aggiorna il numero di versione quando apporti modifiche.
1. Salva le modifiche. Tutte le abilità di Collaboratore per Marketo Engage utilizzeranno immediatamente le regole personalizzate.

## Struttura delle regole organizzative {#organizational-rules-structure}

Le regole organizzative sono formattate in Markdown con il frontmatter YAML:

```markdown
---
name: Your Organization Name - Marketo Campaign Governance
version: 1.0
enabled: true
customized: true
---

# Naming Conventions

## Programs
- Pattern: {{REGION}}_FY{{YEAR}}_{{QUARTER}}_{{TYPE}}_{{DATE}}_{{NAME}}
- Example: AMER_FY25_Q2_WBR_250315_Product_Launch_Webinar
- Region codes: AMER, EMEA, APAC, GLOBAL

## Emails
- Pattern: {{PROGRAM_NAME}}_{{SEQUENCE}}_{{PURPOSE}}
- Example: Product_Launch_01_Invitation

# Program Structure

## Required Local Folders
- 01 Emails
- 02 Smart Campaigns
- 03 Reports

## Required Tokens
- {{my.eventDate}}
- {{my.replyToEmail}}

# Email Compliance

## Required Elements
- Unsubscribe link in footer
- Company name and physical address
- All external links include UTM parameters

## Recommended Elements
- Alt text on all images
- Mobile-responsive design (600px max-width)
```

## Best practice per le regole organizzative {#best-practices-for-organizational-rules}

* **Inizia con valori predefiniti**: controlla le regole predefinite prima di personalizzarle. Riflettono le best practice di settore per le operazioni di marketing.
* **Mantieni le regole concentrate**: includi solo i requisiti rilevanti per la tua organizzazione. Regole inutili creano rumore e riducono inutilmente i punteggi di conformità.
* **Utilizzare controlli automatici e manuali**:

  * Controlli automatizzati: convenzioni di denominazione, cartelle obbligatorie, utilizzo dei token (possono essere verificate da Collaboratore per Marketo Engage)
  * Controlli manuali: progettazione visiva delle e-mail, conformità del brand, logica della campagna (Coworker for Marketo Engage contrassegnerà questi come passaggi di revisione manuali)

* **Equilibrio tra rigidità e flessibilità**: regole troppo rigide possono rallentare la creazione del programma. Le regole troppo vaghe non colgono importanti problemi di conformità.
* **Versione delle regole**: aggiorna il numero di versione quando apporti modifiche significative in modo che il tuo team sappia che gli standard di governance sono stati aggiornati.
* **Comunicare le modifiche**: quando aggiorni le Regole organizzative, comunica al tuo team di addetti al marketing cosa è cambiato e perché.

## Cosa può e non può convalidare Coworker for Marketo Engage {#what-coworker-can-and-cannot-validate}

Collaboratore per Marketo Engage PUÒ convalidare (controlli automatici):

* Le convenzioni di denominazione corrispondono ai tuoi modelli
* La struttura di cartelle richiesta esiste
* I token richiesti sono presenti
* L’e-mail contiene un collegamento che consente di annullare l’abbonamento e alcuni elementi del piè di pagina richiesti
* I collegamenti esterni includono i parametri UTM
* I nomi delle campagne intelligenti seguono le convenzioni

Impossibile convalidare il collaboratore per Marketo Engage (è necessaria una revisione manuale):

* Logica filtro elenchi avanzati (limitazione API: è necessario configurare i filtri manualmente)
* Logica del passaggio di flusso di Smart Campaign (limitazione API: è necessario configurare i flussi manualmente)
* Rendering visivo e reattività dell’e-mail (è necessaria un’ispezione visiva)
* Rispetto del brand e tono di messaggistica (richiede il giudizio umano)
* Regole di segmentazione dinamica dei contenuti (limitazione API)

Quando Coworker for Marketo Engage rileva qualcosa che non può convalidare, lo contrassegna come un passaggio di revisione manuale nel flusso di lavoro.

## Valutazione della conformità {#compliance-scoring}

Quando si utilizza Convalida programmi, Collaboratore per Marketo Engage calcola un punteggio di conformità in base a:

* **Controlli superati**: il collaboratore per Marketo Engage ha verificato la conformità e non ha rilevato problemi
* **Controlli non riusciti**: il collaboratore per Marketo Engage ha rilevato violazioni delle regole organizzative
* **Passaggi di revisione manuali**: elementi che richiedono la verifica umana (questi NON vengono conteggiati rispetto al punteggio)

Un programma può avere una conformità del 100% e richiedere comunque passaggi di revisione manuali; sono esclusi dal calcolo del punteggio.

## Esempi di personalizzazione delle regole organizzative {#examples-of-organizational-rules-customization}

**Esempio 1: convenzione di denominazione rigorosa**

```markdown
## Programs
Pattern: {{COUNTRY}}-{{BUSINESS_UNIT}}-{{CAMPAIGN_TYPE}}-FY{{YEAR}}-{{QUARTER}}-{{DATE}}
```

Utilizzalo se la tua organizzazione richiede una governance rigorosa tra aree geografiche e business unit.

**Esempio 2: denominazione flessibile con prefisso obbligatorio**

```markdown
## Programs
Pattern: {{PREFIX}}_* (where PREFIX = EMEA, AMER, APAC, GLOBAL)
Example: AMER_Q2_Product_Launch_Webinar_2025
```

Utilizzatelo se desiderate coerenza sui codici di regione ma flessibilità sugli altri.

**Esempio 3: regole minime (attenzione alla conformità)**

```markdown
# Email Compliance - REQUIRED

- Unsubscribe link present
- CAN-SPAM physical address in footer
- Reply-to email configured
```

Utilizzalo se la tua organizzazione dà priorità alla conformità rispetto alla coerenza di denominazione/struttura.

## Risoluzione dei problemi {#troubleshooting}

**D: ho aggiornato le regole organizzative ma Collaboratore per Marketo Engage utilizza ancora le regole precedenti.**

R: Le modifiche diventano immediatamente effettive per i nuovi programmi e le convalide. Se stai lavorando a un programma esistente, aggiorna il browser o avvia un nuovo flusso di lavoro Collaboratore per Marketo Engage per visualizzare le regole aggiornate.

**Q: posso ripristinare le regole predefinite?**

R: Sì. Vai a **Impostazioni** > **Regole organizzative** e fai clic su **Ripristina impostazioni predefinite**. Le regole personalizzate verranno sostituite con le regole predefinite.

**Q: il livello di conformità è basso anche se il programma è buono.**

R: Controllare quali controlli non sono riusciti. Rivedi le Regole organizzative per verificare se sono troppo rigide per i flussi di lavoro correnti o se devi adeguare il programma per soddisfare i tuoi standard.
