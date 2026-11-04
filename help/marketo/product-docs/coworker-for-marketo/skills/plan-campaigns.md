---
description: Utilizza CX Enterprise Coworker for Marketo Engage per trasformare un resoconto della campagna in un piano di programma strutturato che includa logica di pubblico, e-mail, token e controlli di qualità.
title: Pianificare le campagne
source-git-commit: b47454801d391f4d7a75ebcfce7ac76c2f4b8af4
workflow-type: tm+mt
source-wordcount: '736'
ht-degree: 0%
---
# Pianificare le campagne {#plan-campaigns}

Trasforma il resoconto di una campagna in un piano di implementazione strutturato per Marketo Engage. L’abilità Pianifica campagne definisce la struttura del programma, la logica del pubblico, le e-mail, le campagne intelligenti, i token, il reporting e i controlli di preattivazione. L’output è un rapporto scaricabile visualizzato nel pannello dell’area di lavoro.

>[!NOTE]
>
>Questa abilità genera piani di implementazione per i programmi Marketo Engage (documenti strutturati che indicano a un utente o a un sistema di automazione esattamente come creare una campagna). Non crea nulla in Marketo Engage. Esiste un&#39;abilità separata per [la creazione di programmi](/help/marketo/product-docs/coworker-for-marketo/skills/build-programs.md).

## Prerequisiti {#prerequisites}

- Per un piano di programma, fornisci un resoconto della campagna con le informazioni disponibili, ad esempio obiettivi della campagna, pubblico di destinazione, messaggi, timeline e metriche di successo.
- Per migliorare una descrizione o un piano esistente, fornisci il documento e descrivi le modifiche desiderate.
- Per iniziare senza breve, richiedi un resoconto di esempio o chiedi un piano basato su uno scenario di campagna comune.

## Come usare {#how-to-use}

1. Nel Marketo personale, fare clic sul riquadro **[!UICONTROL CX Enterprise Coworker for Marketo Engage]**.

1. Selezionare l&#39;abilità **[!UICONTROL Plan campaigns]** e fare clic su **[!UICONTROL Use this skill]**.

1. Scegliere l&#39;operazione da eseguire:
   - Pianifica un programma da una descrizione della campagna.
   - Genera un resoconto di esempio sulla campagna.
   - Polacco: un&#39;idea già esistente.
   - Rivedere un piano di installazione esistente.

1. Fornisci la descrizione o il documento. Includi eventuali modifiche specifiche, requisiti della campagna o convenzioni organizzative.

1. Esamina il rapporto generato nel pannello dell’area di lavoro. Aprilo per rivedere i dettagli o scaricare il rapporto.

1. Rivedi e approva il piano di installazione prima di creare il programma in Marketo Engage.

## Opzioni abilità {#skill-options}

### Pianificare un programma {#plan-a-program}

Un piano di programma traduce i requisiti della campagna in istruzioni per la creazione del programma. A seconda delle specifiche, può includere:

- **Panoramica del programma:** nome della campagna, obiettivi, pubblico di destinazione e timeline.
- **Struttura delle cartelle:** Cartelle locali consigliate per e-mail, campagne avanzate e report.
- **Elenchi avanzati:** logica di segmentazione, definizioni di filtri ed esclusioni richieste.
- **Configurazione e-mail:** righe oggetto, testo preintestazione, struttura del contenuto, dettagli mittente ed elementi di conformità.
- **Campagne avanzate:** nomi di campagne, designazione del trigger o del batch, passaggi del flusso e raccomandazioni sulla pianificazione.
- **Token e campi:** Token personali, token obbligatori e personalizzati ed eventuali campi personalizzati necessari con i relativi tipi e valori.
- **Flusso di Percorso:** Sequenza campagna, passaggi attesa e logica decisionale.
- **Generazione rapporti e controllo qualità:** Metriche di successo, rapporti consigliati e controlli di convalida pre-attivazione.

### Crea un resoconto di esempio {#create-a-sample-brief}

Richiedi un riepilogo di esempio quando desideri che un esempio si adatti. Puoi specificare un argomento o un tipo di campagna, ad esempio un lancio di prodotto o un webinar. Se chiedi un piano senza fornirne una breve, l’abilità può utilizzare uno scenario di esempio, ad esempio un webinar sul lancio di un prodotto, come base per il piano.

### Polacco di una descrizione o revisione di un piano {#polish-a-brief-or-revise-a-plan}

L&#39;abilità identifica il tipo di documento dal relativo contenuto, anziché basarsi solo sul testo della richiesta.

Un **riepilogo della campagna** descrive in genere obiettivi, pubblico, strategia di messaggistica, timeline e metriche di successo. Un **piano di installazione** contiene in genere dettagli di implementazione come le configurazioni dell&#39;elenco smart, i passaggi del flusso di Smart Campaign, le definizioni dei token, le specifiche e-mail e i requisiti tecnici.

Fornisci il documento e le modifiche richieste. Ad esempio, se chiedi di lucidare un piano ma fornisci una descrizione della campagna, l’abilità tratta il documento come una descrizione. Se si fornisce un piano di installazione e si richiede di modificare una descrizione, il documento viene considerato come un piano.

## Integrazione delle regole organizzative {#organizational-rules-integration}

I documenti di configurazione devono incorporare le regole della tua organizzazione dal contesto del sistema.

### Convenzioni di denominazione {#naming-conventions}

- Programmi: `{{REGION}}_FY{{YEAR}}_{{QUARTER}}_{{TYPE}}_{{DATE}}_{{NAME}}`
- E-mail: `{{PROGRAM_NAME}}_{{SEQUENCE}}_{{PURPOSE}}`
- Campagne avanzate: `{{NUMBER}}_{{TRIGGER_OR_BATCH}}_{{ACTION}}`

### Elementi richiesti {#required-elements}

- Tre cartelle locali (01 E-mail, 02 Campagne avanzate, 03 Rapporti)
- Quattro token richiesti (eventDate, eventTime, replyToEmail, senderName)
- Filtri di esclusione (annullamento dell’abbonamento, e-mail non valida, marketing sospeso,)
- Conformità e-mail (collegamento per annullare l’abbonamento, indirizzo fisico)

### Controllo di qualità pre-attivazione {#pre-activation-qa}

- Convalida pattern nome
- Conferma della struttura delle cartelle
- Verifica filtro di esclusione
- Controlli degli elementi di conformità

## Casi di utilizzo {#use-cases}

**Pianifica un programma di webinar:** Fornisci l&#39;obiettivo del webinar, il pubblico, la sequenza temporale degli eventi e le esigenze di messaggistica. Il piano di configurazione può delineare la struttura del programma, le specifiche e-mail, la sequenza della campagna, i token e i controlli di controllo qualità.

**Genera un riepilogo di esempio:** Richiedi un riepilogo di esempio per un tipo di campagna, quindi adattalo ai dettagli della campagna prima di richiedere un piano di programma.

**Aggiorna un piano di installazione esistente:** Fornisci il piano e specifica le modifiche, ad esempio l&#39;aggiornamento della timeline, l&#39;aggiunta di un passaggio della campagna o la revisione della logica del pubblico.

## Passaggi successivi {#next-steps}

Al termine di un&#39;operazione di pianificazione, le richieste di follow-up appropriate possono includere:

- &quot;Rivedi questo piano di installazione&quot;
- &quot;Ottieni un riepilogo della campagna di esempio&quot;
- &quot;Crea questo programma in Marketo&quot; (per creare un programma, è necessario utilizzare l&#39;abilità [generazione programmi](/help/marketo/product-docs/coworker-for-marketo/skills/build-programs.md)).
