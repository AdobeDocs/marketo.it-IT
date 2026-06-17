---
description: Il programma Clone duplica un programma Marketo esistente in una nuova cartella con un nuovo nome, preservandone la struttura e consentendo la personalizzazione della nuova campagna.
title: Clona programma
badge: Beta
hide: true
source-git-commit: 408923e529bdfb2aa23f7d6acfb229cd7ee4c9d8
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---

# Clona programma {#clone-program}

L’agente del programma Clona copia un programma di lavoro, incluse le campagne intelligenti, i passaggi di flusso, le risorse e-mail e la configurazione, in una nuova posizione nell’ambiente Marketo.

>[!PREREQUISITES]
>
>* Per utilizzare questa funzione devi prima accettare i [termini Gen-AI di base e i termini supplementari](https://www.adobe.com/legal/terms/enterprise-licensing/genai-ww.html){target="_blank"}. Per informazioni, contatta il team dell’account di Adobe (il tuo account manager).
>
>* È necessario disporre dell&#39;autorizzazione per creare programmi nella cartella di destinazione.
>
>* Il programma di origine che si desidera clonare deve esistere già nell&#39;ambiente Marketo.

>[!AVAILABILITY]
>
>Questa funzione è attualmente in versione beta chiusa. Non divulgare questa documentazione.

## Come usare {#how-to-use}

1. In Il mio Marketo, fai clic sul riquadro **IA per Marketo**.
1. Nella finestra del prompt, digitare le istruzioni. Ad esempio, &quot;Clona il mio programma di webinar Q2 nella cartella Campagne Q3 e chiamalo Webinar dimostrativo del prodotto Q3.&quot;
1. Marketo AI conferma il programma di origine, la cartella di destinazione e il nuovo nome. Rivedi e conferma.
1. Il clone viene creato. L’intelligenza artificiale di Marketo conferma quando è completato e ti dice dove trovarlo.
1. Apri il nuovo programma in Marketo e aggiorna le differenze: contenuto e-mail, date, filtri del pubblico, token e così via.
1. Esegui l&#39;agente di controllo qualità [Programma](/help/marketo/product-docs/marketo-ai/skills/program-qa.md) prima dell&#39;attivazione.

## Casi d’uso {#use-cases}

**Riutilizzo campagna trimestrale**: un manager campagna esegue la stessa serie di webinar ogni trimestre. Chiedono ad Marketo AI di clonare il programma del webinar dell’ultimo trimestre nella cartella del nuovo trimestre con un nome aggiornato. Quindi aggiorna la copia e-mail, i token della data del webinar e il collegamento di registrazione, risparmiando ore di tempo per la configurazione.

**Creazione di un modello da un programma collaudato**: uno specialista di operazioni di marketing clona un programma di lancio di prodotto ad alte prestazioni in una cartella &quot;Modelli&quot; per fungere da punto di partenza per i lanci futuri. Il clone viene lasciato disattivato e utilizzato come copia di riferimento.

**Test A/B di un nuovo approccio**: un manager della campagna desidera testare una cadenza e-mail diversa senza modificare un programma in esecuzione. Clonano il programma attivo, modificano i passaggi di attesa nel clone e li attivano entrambi, eseguendoli su diversi segmenti di pubblico per confrontare i risultati.

## Aspetti da considerare {#things-to-note}

* I programmi clonati vengono creati in uno stato disattivato. Niente diventa attivo finché non attivi le campagne intelligenti.
* Le risorse e-mail nel clone sono copie, non condivise con l’originale. Le modifiche alle e-mail del clone non influiranno sul programma di origine.
* I token utilizzati nel programma di origine vengono copiati nel clone. Tuttavia, devono ancora essere aggiornati con i nuovi valori (date, URL, nomi di eventi).
* I filtri Smart Campaign nel clone fanno riferimento agli stessi elenchi e campi dell’originale. Rivedi e aggiorna il targeting del pubblico prima dell&#39;attivazione.
* Le risorse locali che fanno riferimento ad altri programmi o elenchi condivisi vengono copiate nel clone. Tali riferimenti devono essere rivisti prima dell’attivazione.
