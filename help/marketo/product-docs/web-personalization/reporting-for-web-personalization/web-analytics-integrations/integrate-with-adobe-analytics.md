---
unique-page-id: 2949160
description: Integrare con Adobe Analytics - Documentazione Marketo - Documentazione del prodotto
title: Integrare con Adobe Analytics
exl-id: 6ea35811-6f3d-4dc8-91aa-877d613f8e93
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '1130'
ht-degree: 0%

---

# Integrare con Adobe Analytics {#integrate-with-adobe-analytics}

## Introduzione {#intro}

Analizza le tue analisi web da una prospettiva B2B visualizzando i dati della campagna RTP (Real-Time Personalization) di organizzazione, settore e Marketo all’interno del tuo account Adobe Analytics.

Questo documento abilita l’integrazione tra Marketo Real-Time Personalization (RTP) e Adobe Adobe Analytics. I dati provenienti da RTP ti consentiranno di rilevare e analizzare le tendenze in tutti i segmenti del settore e le organizzazioni che visitano il tuo sito e di misurare l’efficacia delle campagne RTP, fornendo informazioni approfondite e analisi per ottenere risultati ottimali.

Per ottenere questo risultato, puoi esaminare metriche quali il numero di visitatori nuovi rispetto a quelli di ritorno in ciascun segmento, analizzare i tassi di clic sulle campagne e scoprire quali settori, segmenti personalizzati e campagne in tempo reale hanno generato i lead di conversione migliori. Sfrutta questa possibilità per ottenere il massimo vantaggio dal tuo account RTP.

## AUDIENCE ANALYTICS RTP {#rtp-audience-analytics}

Con l’integrazione RTP - AA, hai una nuova dimensione all’interno dell’interfaccia di analisi web. RTP migliora automaticamente le tue dashboard di analisi web con:

1. Dati aziendali e di settore
1. Segmenti RTP personalizzati
1. Elenchi di account denominati (Account-Based Marketing)

Questo migliora i dati B2B e consente di concentrarsi sui visitatori rilevanti ottimizzando:

1. Canali in uscita
1. Contenuto
1. Retargeting

## Rapporto canale {#channel-report}

![](assets/image2014-11-29-12-3a0-3a26.png)

La dashboard RTP consente di comprendere la suddivisione dei visitatori in base ai segmenti verticali e RTP. Puoi visualizzare le prestazioni dei visitatori in base al settore e alle diverse campagne di marketing (a pagamento, organiche, sociali) correlate a tale settore. La dashboard offre anche una panoramica di alto livello delle sezioni del sito visualizzate dai visitatori in base al tipo di settore.

## Rapporto comportamentale {#behavioral-report}

In Adobe Analytics è possibile creare rapporti di comportamento diversi in base ai dati dell’organizzazione, del settore e del segmento RTP. Questi rapporti di flusso visualizzano il percorso seguito dai visitatori da una pagina o un evento all’altro. Questo rapporto può aiutarti a scoprire quale contenuto mantiene i visitatori coinvolti con il tuo sito.

## Prestazioni RTP {#rtp-performance}

Visualizza le impression e le conversioni della campagna RTP in Collegamenti personalizzati in Adobe Analytics.

Questo rapporto di collegamento personalizzato mostrerà le impression e le conversioni delle campagne nel seguente formato di denominazione:

* Impression ISegment: [Nome segmento RTP], Campagna IC: [Nome campagna RTP]
* Segmento IS di conversione: [Nome segmento RTP], Campagna IC: [Nome campagna RTP]

![](assets/custom-links-report.png)

## Configurazione in Adobe Analytics {#set-up-in-adobe-analytics}

L’integrazione utilizza l’API JavaScript offerta da Adobe Analytics. Nell’integrazione vengono utilizzate variabili di conversione personalizzate (eVar), eventi personalizzati (evento) e variabili di traffico. Tutte le funzioni devono essere abilitate dall’interno di un amministratore. Devi impostare le variabili di conversione, gli eventi personalizzati e le variabili di traffico in AAor non potrai visualizzare i dati nella suite anche se l’hai abilitata in RTP.

Per impostare queste variabili in AA, completa i passaggi seguenti:

1. Vai a **Strumenti di amministrazione** nel tuo account AA.
1. Seleziona la **Suite di rapporti** da utilizzare con l’integrazione.
1. Sotto **Modifica impostazioni**, vai a **Conversione** e seleziona **[Variabili di conversione](https://microsite.omniture.com/t2/help/en_US/reference/#Edit_conversion_variables)**.\
   Seleziona la [Variabile di conversione](https://microsite.omniture.com/t2/help/en_US/reference/#Conversion_Variables_eVar) numero (consigliato):

   1. Evar n. 20 per conversioni personalizzate del settore
   1. Evar n. 21 per conversioni personalizzate organizzazione

   >[!NOTE]
   >
   >Se si utilizzano questi #, selezionare un altro numero disponibile. Allineare questo numero al numero di slot nelle impostazioni account RTP.

   1. Cambia stato in _Abilitato_.

      1. Cambia nome in **Settore** e **Organizzazione**. (Questo è come apparirà nella suite di rapporti).

      1. Cambia campo Expire After a **Visita**.

1. Sotto **Modifica impostazioni** vai a **Conversione** e seleziona **[Eventi di successo](https://microsite.omniture.com/t2/help/en_US/reference/#Configure_success_events)**.

   1. Seleziona il numero evento di successo personalizzato (consigliato):

      1. event20 per campagne RTP
      1. event21 per segmenti RTP

      >[!NOTE]
      >
      >Se si utilizzano questi #, selezionare un altro numero disponibile. Allineare questo numero al numero di slot nelle impostazioni account RTP.

      1. Modifica i nomi dei due eventi in **Campagne RTP** e **Segmenti RTP**. Questo è il nome che verrà visualizzato nella suite di rapporti.

   1. Seleziona il campo Tipo da impostare **Contatore (nessuna relazione secondaria)**

1. Sotto **Modifica impostazioni** vai a **[Traffico](https://microsite.omniture.com/t2/help/en_US/reference/#Traffic_Variable)** e seleziona **[Variabili di traffico](https://microsite.omniture.com/t2/help/en_US/reference/#Enable_traffic_variable_reports)**.

   1. Seleziona la proprietà della variabile di traffico # (ti consigliamo):

      1. Proprietà n. 20 - Nome: organizzazione del segmento RTP
      1. Proprietà n. 21 - Nome: settore del segmento RTP
      1. Proprietà n. 25 - Nome: organizzazione della campagna
      1. Proprietà n. 26 - Nome: settore delle campagne RTP

      >[!NOTE]
      >
      >Se si utilizzano questi #, selezionare un altro numero disponibile. Allinea questo numero al numero di slot nelle impostazioni account RTP)

      1. Modifica i 4 nomi delle proprietà. Questo è il nome che verrà visualizzato nella suite di rapporti.

   1. Seleziona campo abilitato per **Abilitato**.

   1. Seleziona il campo Report percorso per **Abilitato**.

## Configurazione in Marketo Real-Time Personalization (RTP) {#set-up-in-marketo-real-time-personalization-rtp}

1. Nella piattaforma RTP, vai a **Impostazioni account**.

   ![](assets/image2014-11-29-11-3a27-3a7.png)

1. Sotto **Impostazioni account**, fai clic su **Dominio**.
1. Sotto **Analytics, fai clic su** **Adobe Analytics**.
1. Turno **On** le variabili Conversione, Personalizzato e Traffico vengono attivate/disattivate.
1. Assegnare le variabili di conversione, evento e traffico **numeri di slot** per far corrispondere i numeri di slot creati in AA
1. Clic **Salva**.

![](assets/image2014-11-29-12-3a24-3a42.png)

>[!NOTE]
>
>Le impostazioni consigliate per gli slot sono
>
>**Variabili di conversione**
>
>* Conversioni personalizzate settore - Slot 20
>* Conversioni personalizzate organizzazione - Slot 21
>
>**Eventi personalizzati**
>
>* Evento personalizzato campagna - Slot 20
>* Evento personalizzato segmento - Slot 21
>
>**Variabili di traffico**
>
>* Variabile traffico organizzazione segmento - Slot 20
>* Variabile di traffico del settore del segmento - Slot 21
>* Variabile di traffico organizzazione della campagna - Slot 22
>* Variabile di traffico del settore della campagna - Slot 23
>
>**Assicurati che questi numeri di slot siano allineati con le variabili e i numeri di eventi creati in AA.**

## Rapporti {#reports}

Creare rapporti avanzati di SiteAdobe Analytics in base ai nomi delle organizzazioni, ai settori e ai segmenti RTP e ai dati delle campagne in tempo reale.

Esempi di report e dashboard personalizzati in AA includono:

* Prestazioni per settore o segmento definito (elenchi denominati basati sull’account)
* Suddivisione del settore per prestazioni KPI
* Pagine visualizzate per organizzazione
* Prestazioni del canale di marketing in base a organizzazione, settore e segmenti

**-Esempi di report-**

**Rapporto Primi settori**

![](assets/top-industries-report.png)

**Rapporto Organizzazioni**

![](assets/image2014-11-29-12-3a29-3a42.png)

**Creazione del dashboard RTP**

Creare un [nuova dashboard](https://microsite.omniture.com/t2/help/en_US/sc/user/t_dashboard_add.html), chiamato **Dashboard RTP**. Questa dashboard ti aiuterà a comprendere la suddivisione dei visitatori in base ai segmenti verticali e RTP.

1. Clic **Dashboard,** click **Aggiungi dashboard**.

1. Denomina il dashboard **Dashboard RTP**.

1. Seleziona la **dimensione dashboard** 3 x 2, 2 x 2

1. Creare [reportlet](https://microsite.omniture.com/t2/help/en_US/sc/user/t_dashboard_add_report.html#task_EC3AFBBAA51C45CEBAF632F841C305B3) e aggiungi [contenuto alla dashboard](https://docs.marketo.com/Add%2520content%2520to%2520a%2520dashboard).

Aggiunta del reportlet Settori al dashboard

1. Vai a **Conversioni personalizzate**, fai clic su **Settore**.

1. Configura grafico in **Grafico a torta**.

1. Fai clic su **Dashboard**, aggiungi **Reportlet**.

1. Assegna un nome al rapporto **Settori principali**.

1. Inserisci nel dashboard **Dashboard RTP**.

1. Crea **Nuovo**.

Aggiunta del reportlet dei segmenti al dashboard

1. Vai a **Metriche del sito**. Fai clic su **Eventi personalizzati**, **Segmenti**.

1. Configura grafico in **Barra verticale**.

1. Fai clic su **Dashboard**, aggiungi **Reportlet**.

1. Assegna un nome al rapporto **Segmenti principali**.

1. Inserisci nel dashboard **Dashboard RTP**.

1. Crea **Nuovo**.

I reportlet verranno visualizzati nella dashboard.

## Visualizzare impressioni e clic (conversioni) in Adobe Analytics {#view-impressions-and-clicks-conversions-in-adobe-analytics}

1. Clic **Collegamenti personalizzati**.

   ![](assets/sitecatalyst1-1.png)

1. Cerca le impression per visualizzare i nomi dei segmenti e delle campagne che rappresentano il numero di impression per la campagna.\
   ![](assets/sitecatalyst1.png)

1. Cerca Conversione per visualizzare i nomi dei segmenti e delle campagne che rappresentano il numero di clic per la campagna.

   ![](assets/sitecatalyst2.png)
