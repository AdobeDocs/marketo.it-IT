---
description: L’agente lead di Investigate risponde alle domande che gli addetti al marketing si pongono più spesso. È più veloce e affidabile rispetto allo scavo manuale dei registri di attività, alla cronologia intelligente delle campagne e ai record di punteggio.
title: Indaga lead
beta: true
hide: true
hidefromtoc: true
source-git-commit: a2c170ced2119a86ffe1f2da1bde212afa4841f0
workflow-type: tm+mt
source-wordcount: '650'
ht-degree: 0%

---

# Indaga lead {#investigate-lead}

Scopri perché una persona/un lead specifico non ha raggiunto una fase cardine (come MQL, qualificazione del programma o una campagna) e ottieni una spiegazione semplice di ciò che è successo.

>[!PREREQUISITES]
>
>È necessario disporre dell&#39;accesso in visualizzazione al record del lead e al programma o alla fase cardine esaminati.

## Come funziona

Indica a Marketo AI quale società leader stai esaminando e quali sono le milestone o i risultati previsti. Marketo AI esamina la cronologia delle attività del lead, il record di punteggio, l’iscrizione al programma, la cronologia di qualificazione intelligente delle campagne ed eventuali filtri o regole di eliminazione rilevanti. Restituisce quindi una spiegazione chiara di cosa ha bloccato o ritardato il risultato previsto, ad esempio, &quot;Il punteggio di questo lead ha raggiunto 48 ma la soglia MQL è 50&quot; o &quot;Questo lead è stato escluso dalla campagna perché l’iscrizione è stata annullata il 3 marzo&quot;.

## Come usare {#how-to-use}

1. In Il mio Marketo, fai clic sul riquadro **Genera con IA**.

1. Nella finestra del prompt, descrivi ciò che stai esaminando. Includi il lead (per e-mail o nome) e ciò che prevedevi accadesse.

>[!NOTE]
>
>Alcuni esempi: &quot;Perché `john.smith@example.com` non ha raggiunto MQL il mese scorso?&quot; o &quot;Perché Brenda Gonzales non è stata aggiunta al programma del webinar Q3?&quot;

1. Marketo AI richiama il record del lead e la relativa cronologia.

1. Rivedi la spiegazione. Marketo AI indica il motivo specifico per cui la milestone non è stata raggiunta e, ove possibile, ciò che dovrebbe essere modificato affinché il lead sia idoneo.

1. Intervenire in base al risultato: correggere un problema di dati, regolare un filtro, aggiornare il punteggio del lead o accettare che il risultato sia corretto.

## Esempi

**Soglia MQL non raggiunta**
Un responsabile della gestione della domanda nota un lead che le vendite contrassegnano come interessato, ma che non ha mai raggiunto MQL. Chiede: &quot;Perché david.chen@techcorp.com non ha raggiunto MQL?&quot; Marketo AI rileva che il punteggio comportamentale del lead è di 42, 8 punti al di sotto della soglia MQL di 50, e elenca le attività che hanno contribuito con il punteggio. Lei riesce a vedere esattamente quali comportamenti spingerebbero il lead oltre la soglia.

**La campagna è stata saltata a causa dell&#39;eliminazione**
Un responsabile della campagna chiede perché un contatto specifico non ha ricevuto un&#39;e-mail di invito che è andata al resto del suo elenco. Marketo AI rileva che il contatto si trova nell’elenco di marketing sospeso, che lo esclude automaticamente da tutti gli invii di campagne. Il manager contatta direttamente il contatto per indagare sul motivo della soppressione.

**Errore di qualificazione del programma**
Uno specialista di operazioni di marketing sta cercando di risolvere il motivo per cui un lead che ha partecipato a un webinar non è stato aggiunto al programma di follow-up post-evento. Marketo AI traccia il problema: il lead registrato ma contrassegnato come &quot;No Show&quot; nel programma dell’evento e il filtro della campagna di follow-up richiede lo stato &quot;Partecipato&quot;. Lo stato non è stato impostato correttamente nell’integrazione.

**Piombo bloccato in un&#39;azienda agricola**
Un responsabile della generazione della domanda nota che un lead è stato nella stessa fase di sviluppo per 90 giorni senza progredire. Chiede a Marketo AI di indagare. Rileva che il punteggio di coinvolgimento del lead è sceso al di sotto della soglia necessaria per passare alla fase successiva e che il lead non ha aperto un’e-mail in 60 giorni, qualificandosi invece per il ramo di ricoinvolgimento.

## Suggerimenti e limitazioni

* Lead Investigation spiega cosa è successo in base all&#39;attività e alla configurazione registrate da Marketo: non può spiegare le decisioni prese al di fuori di Marketo (ad esempio, perché un lead è stato rimosso manualmente da un collega).
* Se la cronologia delle attività di un lead è molto lunga, Marketo AI si concentra sugli eventi più recenti e rilevanti correlati alla domanda.
* L&#39;investigazione del lead è di sola lettura: indica l&#39;accaduto ma non apporta modifiche al record del lead o all&#39;iscrizione al programma.
* Per i problemi che si rivelano problemi di qualità dei dati (valori di campo mancanti, origine lead errata), la correzione dovrà essere eseguita manualmente nel record del lead.
* Se l’indagine rivela un problema di logica della campagna intelligente che interessa molti lead, utilizza il Controllo qualità del programma per rivedere la configurazione completa del programma.
