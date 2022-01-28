---
description: Panoramica della chat dinamica - Documenti Marketo - Documentazione del prodotto
title: Panoramica della chat dinamica
hide: true
hidefromtoc: true
exl-id: 73ab651e-bb11-459d-aa6a-39d9e208d512
source-git-commit: 9ab6640ae30bd5ad653b5936a01ec3b0e19d595b
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 0%

---

# Panoramica della chat dinamica {#dynamic-chat-overview}

La chat dinamica consente di sfruttare un&#39;interfaccia di facile utilizzo per eseguire il targeting sia per le persone che per gli account che visitano il tuo sito web. Raccogli contenuti pertinenti quali nome, informazioni di contatto e testo libero. I visitatori del sito possono anche prenotare riunioni con il team di vendita. I dati di attività e coinvolgimento della chat dinamica possono essere utilizzati per aggiungere membri ai programmi Marketo e attivare attività cross-channel.

>[!NOTE]
>
>La chat dinamica sta per essere implementata gradualmente ed è attualmente a disponibilità limitata. Questa pagina verrà aggiornata con i dettagli di disponibilità generale (GA) man mano che diventano disponibili.

>[!TIP]
>
>Visita [questa pagina](https://dcweb.z20.web.core.windows.net/) per visualizzare video tutorial e una demo registrata di Dynamic Chat.

## Integrazioni {#integrations}

Un componente chiave della chat dinamica è la sua capacità di interfaccia nativa con il tuo abbonamento Marketo. Per sfruttare appieno la funzionalità di questa integrazione, è innanzitutto necessario avviare la sincronizzazione dei dati. A seconda delle dimensioni del database Marketo, potrebbero essere necessarie fino a 24 ore per i dati iniziali, [sincronizzazione una tantum](/help/marketo/product-docs/demand-generation/dynamic-chat/connect-dynamic-chat-to-marketo.md) da completare.

Viene sincronizzato quanto segue:

* Dati del campo Persona
* Dati sul campo dell&#39;azienda
* Dati attività

## Finestre di dialogo {#dialogues}

Le finestre di dialogo rappresentano un singolo coinvolgimento di chat. Immaginalo come un contenitore con tutte le cose necessarie per avere un dialogo chat coinvolgente con i visitatori del tuo sito web. In ciascuna finestra di dialogo è possibile specificare le pagine sulle quali si desidera visualizzare la finestra di dialogo, le relative pagine e il contenuto e il flusso della finestra stessa. Inoltre, puoi trovare le metriche per vedere le prestazioni della finestra di dialogo. [Ulteriori informazioni sulle finestre di dialogo](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues.md).

## Configurazione {#configuration}

Nella scheda Configurazione, personalizzare l&#39;aspetto delle varie finestre di dialogo. Cambia font, colori, tempo di risposta e altro ancora! [Ulteriori informazioni sulla configurazione](/help/marketo/product-docs/demand-generation/dynamic-chat/configuration.md).

## Calendario {#calendar}

Nella scheda Calendario, collegare il calendario (Outlook o Gmail) per l&#39;utilizzo nella pianificazione degli appuntamenti nel chatbot. Una volta che il calendario di un utente è connesso a Dynamic Chat, tale utente verrà aggiunto alla coda e il suo calendario sarà disponibile per i visitatori del sito web a pianificare gli appuntamenti in.

Puoi anche personalizzare il corpo dell’invito inviato al visitatore quando questo pianifica un appuntamento sul calendario dell’utente.

## Riunioni {#meetings}

Qui puoi vedere tutti gli appuntamenti pianificati dai visitatori del sito web attraverso le varie finestre di dialogo. Qui trovi l&#39;indirizzo e-mail della persona che ha prenotato l&#39;appuntamento, con quale agente ha prenotato l&#39;appuntamento, quando l&#39;appuntamento è programmato e se la riunione è avvenuta o meno.

## Indirizzamento {#routing}

Qui puoi vedere un elenco di tutti gli agenti che hanno collegato i loro calendari e l&#39;ordine in cui verranno presentati ai visitatori del sito web. Le riunioni vanno in stile robin, quindi se avete cinque agenti e l&#39;agente tre ha preso l&#39;ultima riunione, l&#39;agente quattro avrà quello successivo, seguito dall&#39;agente cinque, poi di nuovo all&#39;agente uno.

## Domande frequenti {#faq}

**La chat dinamica consente la chat dal vivo?**

No, utilizza solo risposte predeterminate.

**Come posso indirizzare le persone anonime?**

Nella finestra di dialogo, devi utilizzare il _L&#39;e-mail della persona è vuota_ attributo.

**Supporta la funzionalità AI/NLP?**

Non è supportata la funzionalità AI/NLP.

**Per quanto tempo vengono memorizzati i dati per il reporting?**

90 giorni.

**Dynamic Chat offre altre lingue oltre all&#39;inglese?**

Non in questo momento.
