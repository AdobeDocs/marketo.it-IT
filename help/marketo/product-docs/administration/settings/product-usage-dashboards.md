---
description: Dashboard di utilizzo del prodotto - Documentazione di Marketo - Documentazione del prodotto
title: Dashboard utilizzo prodotto
hide: true
hidefromtoc: true
feature: Administration
source-git-commit: f3bc58c0d65e8110c5366269fdb4abf817370aee
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 0%

---

# Dashboard utilizzo prodotto {#product-usage-dashboards}

I dashboard di utilizzo dei prodotti Marketo Engage consentono di visualizzare l’utilizzo di prodotti e piattaforme in relazione a determinati limiti o backlog di dati, flussi di dati, utilizzo rispetto a quote giornaliere e metriche chiave in un abbonamento. L&#39;infrastruttura viene allocata per fornire i limiti di prestazioni definiti per i livelli di prodotto per attributi specifici. Alcuni di questi limiti, come l’utilizzo dell’API, sono limiti contrattuali acquistati come parte del pacchetto o del livello di prodotto.

## Come accedere {#how-to-access}

1. In Marketo Engage, fai clic su **Amministratore**.

   ![](assets/product-usage-dashboards-1.png)

1. Nella struttura a sinistra, scorri verso il basso e seleziona **Dashboard di utilizzo del prodotto**.

   ![](assets/product-usage-dashboards-2.png)

## Dashboard utilizzo attività {#activity-usage-dashboard}

### Attività settimanali medie {#average-weekly-activities}

Il dashboard Utilizzo attività settimanale fornisce un conteggio settimanale dei tipi di attività in un periodo continuo di 52 settimane. Le attività settimanali sono un buon indicatore della quantità di marketing che si sta facendo in Marketo Engage. Le attività fungono da proxy per i vari processi di sistema e gli eventi tracciabili che si svolgono all’interno di Marketo.

I tipi di attività includono sia i conteggi delle attività acquisite quando le persone interagiscono con eventi di marketing, sia le attività basate sul sistema attivate dalle azioni di flusso. Alcuni esempi di attività avviate da una persona si verificano quando una persona apre un’e-mail o fa clic su un collegamento in un’e-mail. Un esempio di attività basate sul sistema attivate da un’azione di flusso è &quot;Send to SFDC&quot; (Invia a) quando il trigger viene avviato. Per visualizzare un conteggio dei tipi di attività per una settimana particolare, passa il cursore del mouse su una settimana e visualizza il conteggio.

![](assets/product-usage-dashboards-3.png){width="800" zoomable="yes"}

#### Domande frequenti {#faq}

**Quali tipi di attività vengono conteggiati?**

Dipende dalle attività incluse nella pipeline.

**L&#39;attività lead/persona nota e anonima è inclusa?**

Solo persone/lead noti.

**Con quale frequenza vengono aggiornati i dati?**

I conteggi delle attività vengono aggiornati ogni mattina.

## Raggruppamento attività {#activity-breakdown}

Qui riceviamo i conteggi delle attività dei sette giorni precedenti in base a sezioni significative dei dati. Raggruppa le attività in base ai tipi di attività più comuni osservati negli ultimi sette giorni. Questo può includere categorie come &quot;Modifica valore dati&quot;, &quot;Aggiungi all’elenco&quot; o &quot;Invia e-mail&quot;. Questo consente di vedere quali tipi di attività si verificano più spesso nel sistema. L’utilizzo del tipo di attività è un indicatore chiave per determinare la crescita o se sono necessarie ottimizzazioni per ridurre l’utilizzo.

>[!NOTE]
>
>* Tutte le suddivisioni seguenti sono una somma &quot;continua di sette giorni&quot; e **non** includono il giorno corrente. Pensateci come &quot;ieri + sei giorni prima&quot;.
>
>* Il dashboard mostra solo i primi 20 tipi di attività, mentre gli altri sono ordinati in una categoria denominata &quot;Altro&quot;.

![](assets/product-usage-dashboards-4.png){width="800" zoomable="yes"}

L’utilizzo dell’attività è un indicatore chiave della quantità di marketing condotto e aiuta a visualizzare la crescita rispetto al livello di prodotto contrattuale per il quale è stato identificato. Le dashboard possono essere utilizzate anche come guida per determinare il livello di ottimizzazione che può/deve essere eseguito riducendo i campi da aggiornare.

### Per tipo {#by-type}

Raggruppa le attività in base ai tipi di attività più comuni osservati negli ultimi sette giorni. Questo può includere categorie come _Modifica valore dati_, _Aggiungi all&#39;elenco_ o _Invia e-mail_. Questo consente di vedere quali tipi di attività si verificano più spesso in Marketo Engage.

### Per modifica attributo valore dati {#by-change-data-value-attribute}

_Modifica valore dati_ è il tipo di attività più comune. Indica quando vengono aggiornate le informazioni di un record persona/lead. In questo caso, eseguiamo il raggruppamento in base ai campi che vengono modificati più spesso, in modo da poter determinare se le informazioni sono utili per le operazioni di marketing, se vi sono opportunità per ottimizzare l’utilizzo della piattaforma e così via.

### Per campagna {#by-campaign}

Gruppo in base al quale le campagne producono il maggior numero di attività. Questo offre ad insight la possibilità di vedere se sono presenti campagne particolarmente &quot;rumorose&quot; che creano più attività del necessario. Scopri rapidamente le campagne che devono essere disattivate o quelle che stanno facendo più lavoro di quanto previsto.

### Di Source (DISPONIBILE A BREVE) {#by-source}

Raggruppa in base all&#39;origine delle attività (_Sincronizzazione CRM_, _Azione di flusso campagna_, _Caricamento API_, _Riempimento modulo pagina di destinazione_, ecc.). Questo ti aiuta a capire se la maggior parte delle attività è prodotta da azioni di marketing, sincronizzazioni CRM o dalle persone/dai lead stessi.
