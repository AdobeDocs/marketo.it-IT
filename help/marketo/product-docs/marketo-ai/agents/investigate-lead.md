---
description: L’agente lead di Investigate risponde alle domande che gli addetti al marketing si pongono più spesso. È più veloce e affidabile rispetto allo scavo manuale dei registri di attività, alla cronologia intelligente delle campagne e ai record di punteggio.
title: Indaga lead
beta: true
hide: true
hidefromtoc: true
source-git-commit: f552c0b0219aede39e0742466ab2473e8e924e55
workflow-type: tm+mt
source-wordcount: '536'
ht-degree: 0%

---

# Indaga lead {#investigate-lead}

Scopri perché una persona/un lead specifico non ha raggiunto una fase cardine (come MQL, qualificazione del programma o una campagna) e ottieni una spiegazione semplice di ciò che è successo.

>[!PREREQUISITES]
>
>* Per utilizzare questa funzione devi prima accettare i [termini Gen-AI di base e i termini supplementari](https://www.adobe.com/legal/terms/enterprise-licensing/genai-ww.html){target="_blank"}. Per informazioni, contatta il team dell’account di Adobe (il tuo account manager).
>
>* È necessario disporre dell&#39;accesso in visualizzazione al record del lead e al programma o alla fase cardine esaminati.

## Come usare {#how-to-use}

1. In Il mio Marketo, fai clic sul riquadro **Genera con IA**.

1. Nella finestra del prompt, descrivi ciò che stai esaminando. Includi il lead (per e-mail o nome) e ciò che prevedevi accadesse.

   >[!NOTE]
   >
   >Alcuni esempi: &quot;Perché `john.smith@example.com` non ha raggiunto MQL il mese scorso?&quot; o &quot;Perché Sato Hanako non è stato aggiunto al programma del webinar Q3?&quot;

1. Marketo AI richiama il record del lead e la relativa cronologia.

1. Rivedi la spiegazione. Marketo AI indica il motivo specifico per cui la milestone non è stata raggiunta e, ove possibile, ciò che dovrebbe essere modificato affinché il lead sia idoneo.

1. Intervenire in base al risultato: correggere un problema di dati, regolare un filtro, aggiornare il punteggio del lead o accettare che il risultato sia corretto.

## Casi d’uso {#use-cases}

**Soglia MQL non raggiunta**: un responsabile della generazione della domanda rileva un lead contrassegnato come interessato dalle vendite, ma che non ha mai raggiunto MQL. Viene chiesto: &quot;Perché `david.chen@techcorp.com` non ha raggiunto MQL?&quot; Marketo AI rileva che il punteggio comportamentale del lead è 42 (8 punti al di sotto della soglia MQL di 50) e elenca le attività di punteggio che hanno contribuito. Possono vedere esattamente quali comportamenti spingerebbero il lead oltre la soglia.

**Ignora campagna a causa dell&#39;eliminazione**: un manager della campagna chiede perché un contatto specifico non ha ricevuto un&#39;e-mail di invito che è andata al resto dell&#39;elenco. Marketo AI rileva che il contatto si trova nell’elenco di marketing sospeso, che lo esclude automaticamente da tutti gli invii di campagne. Il manager si rivolge direttamente a loro per indagare sul motivo della loro soppressione.

**Errore di qualificazione del programma**: uno specialista di operazioni di marketing sta cercando di risolvere il problema relativo al motivo per cui un lead che ha partecipato a un webinar non è stato aggiunto al programma di follow-up post-evento. Marketo AI traccia il problema: il lead registrato ma contrassegnato come &quot;No Show&quot; nel programma dell’evento e il filtro della campagna di follow-up richiede lo stato &quot;Partecipato&quot;. Lo stato non è stato impostato correttamente nell’integrazione.

## Aspetti da considerare {#things-to-note}

* Lead Investigation spiega cosa è successo in base all&#39;attività e alla configurazione registrate di Marketo. Non può spiegare le decisioni prese al di fuori di Marketo (ad esempio, il motivo per cui un lead è stato rimosso manualmente da un collega).
* Se la cronologia delle attività di un lead è molto lunga, Marketo AI si concentra sugli eventi più recenti e rilevanti correlati alla domanda.
* Indagine lead di sola lettura. Indica l&#39;accaduto, ma non apporta modifiche al record del lead o all&#39;iscrizione al programma.
* Per i problemi che si rivelano problemi di qualità dei dati (valori di campo mancanti, origine lead errata), la correzione deve essere eseguita manualmente nel record del lead.
* Se l’indagine rivela un problema di logica della campagna intelligente che interessa molti lead, utilizza il Controllo qualità del programma per rivedere la configurazione completa del programma.
