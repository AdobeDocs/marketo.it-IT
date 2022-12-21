---
unique-page-id: 2949160
description: Integrare con Adobe Analytics - Documentazione Marketo - Documentazione del prodotto
title: Integrare con Adobe Analytics
exl-id: 6ea35811-6f3d-4dc8-91aa-877d613f8e93
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '1130'
ht-degree: 0%

---

# Integrare con Adobe Analytics {#integrate-with-adobe-analytics}

## Introduzione {#intro}

Analizza le tue analisi web da un punto di vista B2B visualizzando i dati delle campagne di organizzazione, settore e Marketo Real-Time Personalization (RTP) all’interno del tuo account Adobe Analytics.

Questo documento consente l’integrazione tra Marketo Real-Time Personalization (RTP) e Adobe Adobe Analytics. I dati RTP ti consentiranno di rilevare e analizzare le tendenze in tutti i segmenti di settore e le organizzazioni che visitano il tuo sito e di misurare l’efficacia delle tue campagne RTP, fornendo le informazioni e le analisi necessarie per ottenere risultati ottimali.

Puoi ottenere questo risultato osservando metriche quali il numero di visitatori nuovi rispetto a quelli di ritorno in ciascun segmento, analizzando i tassi di clic sulle campagne e scoprendo quali settori, segmenti personalizzati e campagne in tempo reale hanno generato la migliore conversione dei lead. Sfrutta questa capacità per trarre il massimo vantaggio dal tuo account RTP.

## Audience Analytics RTP {#rtp-audience-analytics}

Con l’integrazione RTP-AA, hai una nuova dimensione all’interno dell’interfaccia di analisi web. RTP migliora automaticamente le dashboard di analisi web con:

1. Dati aziendali e industriali
1. Segmenti RTP personalizzati
1. Elenchi account denominati (Account-Based Marketing)

Questo migliora i dati B2B e ti consente di concentrarti sui visitatori rilevanti ottimizzando:

1. Canali in uscita
1. Contenuto
1. Retargeting

## Rapporto canale {#channel-report}

![](assets/image2014-11-29-12-3a0-3a26.png)

La dashboard RTP ti aiuta a comprendere la suddivisione dei visitatori in base ai segmenti verticali e RTP. Puoi vedere le prestazioni dei visitatori in base al settore e a diverse campagne di marketing (a pagamento, organiche, social) relative a tale settore. Il dashboard fornisce inoltre una panoramica di alto livello delle sezioni del sito che i visitatori visualizzano in base al tipo di settore.

## Rapporto sul comportamento {#behavioral-report}

In Adobe Analytics è possibile creare diversi rapporti sul comportamento in base ai dati relativi a organizzazioni, settori e segmenti RTP. Questi rapporti di flusso visualizzano il percorso seguito dai visitatori da una pagina o un evento all’altra. Questo rapporto può aiutarti a scoprire quali contenuti mantengono i visitatori coinvolti nel tuo sito.

## Prestazioni RTP {#rtp-performance}

Visualizza le impression e le conversioni della campagna RTP in Custom Links in Adobe Analytics.

Questo rapporto di collegamento personalizzato mostra le impression e le conversioni di campagne nel seguente formato di denominazione:

* ISegment dell&#39;impression: [Nome del segmento RTP], ICCampaign: [Nome della campagna RTP]
* Componente di conversione: [Nome del segmento RTP], ICCampaign: [Nome della campagna RTP]

![](assets/custom-links-report.png)

## Configurazione in Adobe Analytics {#set-up-in-adobe-analytics}

L’integrazione utilizza l’API JavaScript offerta da Adobe Analytics. Nell’integrazione vengono utilizzate variabili di conversione personalizzate (eVar), eventi personalizzati (evento) e variabili di traffico. Tutto deve essere abilitato dall’interno dell’amministratore AA. Devi impostare le variabili di conversione, gli eventi personalizzati e le variabili di traffico in AA, altrimenti non potrai visualizzare i dati nella suite anche se lo hai abilitato in RTP.

Completa i seguenti passaggi per impostare queste variabili in AA:

1. Vai a **Strumenti di amministrazione** nel tuo account AA.
1. Seleziona la **Suite di rapporti** da utilizzare con l’integrazione.
1. Sotto **Modifica impostazioni**, vai a **Conversione** e seleziona **[Variabili di conversione](https://microsite.omniture.com/t2/help/en_US/reference/#Edit_conversion_variables)**.\
   Seleziona la [Variabile di conversione](https://microsite.omniture.com/t2/help/en_US/reference/#Conversion_Variables_eVar) numero (consigliato):

   1. Evar # 20 per conversioni personalizzate di settore
   1. Evar # 21 per le conversioni personalizzate dell&#39;organizzazione

   >[!NOTE]
   >
   >Se vengono presi questi #, selezionare un altro numero disponibile. Allinea questo numero con il numero di slot in Impostazioni account RTP.

   1. Cambia stato in _Abilitato_.

      1. Cambia nome in **Industria** e **Organizzazione**. (Questo è come apparirà nella suite di rapporti.)

      1. Cambia il campo Dopo a **Visita**.


1. Sotto **Modifica impostazioni** vai a **Conversione** e seleziona **[Eventi di successo](https://microsite.omniture.com/t2/help/en_US/reference/#Configure_success_events)**.

   1. Seleziona il numero evento di successo personalizzato (consigliato):

      1. evento20 per le campagne RTP
      1. event21 per i segmenti RTP

      >[!NOTE]
      >
      >Se vengono presi questi #, selezionare un altro numero disponibile. Allinea questo numero con il numero di slot in Impostazioni account RTP.

      1. Modificare i nomi dei due eventi in **Campagne RTP** e **Segmenti RTP**. Questo è il nome che verrà visualizzato nella suite di rapporti.
   1. Selezionare il campo Tipo da specificare **Contatore (nessuna sottorelazione)**



1. Sotto **Modifica impostazioni** vai a **[Traffico](https://microsite.omniture.com/t2/help/en_US/reference/#Traffic_Variable)** e seleziona **[Variabili di traffico](https://microsite.omniture.com/t2/help/en_US/reference/#Enable_traffic_variable_reports)**.

   1. Seleziona il n. proprietà variabile traffico (consigliato):

      1. Proprietà n. 20 - Nome: Organizzazione del segmento RTP
      1. Proprietà n. 21 - Nome: Settore dei segmenti RTP
      1. Proprietà n. 25 - Nome: Organizzazione della campagna
      1. Proprietà n. 26 - Nome: Settore delle campagne RTP

      >[!NOTE]
      >
      >Se vengono presi questi #, selezionare un altro numero disponibile. Allinea questo numero con il numero di slot in Impostazioni account RTP)

      1. Modificare i 4 nomi delle proprietà. Questo è il nome che verrà visualizzato nella suite di rapporti.
   1. Seleziona campo abilitato a **Abilitato**.

   1. Selezionare il campo Report percorso da **Abilitato**.



## Configurazione in Marketo Real-Time Personalization (RTP) {#set-up-in-marketo-real-time-personalization-rtp}

1. Nella piattaforma RTP, vai a **Impostazioni account**.

   ![](assets/image2014-11-29-11-3a27-3a7.png)

1. Sotto **Impostazioni account**, fai clic su **Dominio**.
1. Sotto **Analytics, fai clic su** **Adobe Analytics**.
1. Girare **On** le variabili Conversione, Personalizzato e Traffico sono attivate.
1. Assegnare le variabili di conversione, evento e traffico **numeri di slot** per far corrispondere i numeri degli slot creati in AA
1. Fai clic su **Salva**.

![](assets/image2014-11-29-12-3a24-3a42.png)

>[!NOTE]
>
>Le impostazioni consigliate per gli slot sono:
>
>**Variabili di conversione**
>
>* Conversioni personalizzate del settore - Slot 20
>* Conversioni personalizzate dell&#39;organizzazione - Slot 21
>
>**Eventi personalizzati**
>
>* Evento personalizzato campagna - Slot 20
>* Evento personalizzato segmento - Fessura 21
>
>**Variabili di traffico**
>
>* Variabile traffico organizzazione segmento - Slot 20
>* Variabile di traffico del settore dei segmenti - Slot 21
>* Variabile di traffico dell’organizzazione campagna - Slot 22
>* Variabile di traffico dell&#39;industria delle campagne - Slot 23
>
>**Assicurati che questi numeri di slot siano allineati con le variabili e i numeri di eventi creati in AA.**

## Rapporti {#reports}

Crea report SiteAdobe Analytics migliorati in base ai nomi dell&#39;organizzazione, ai segmenti di settore e RTP e ai dati delle campagne in tempo reale.

Esempi di rapporti e dashboard personalizzati in AA includono:

* Prestazioni per settore o segmento definito (elenchi denominati in base al conto)
* Disaggregazione settoriale per prestazioni KPI
* Pagine visualizzate per organizzazione
* Prestazioni del canale di marketing in base a organizzazione, settore, segmenti

**- Esempi di report-**

**Report dei principali settori**

![](assets/top-industries-report.png)

**Rapporto Organizzazioni**

![](assets/image2014-11-29-12-3a29-3a42.png)

**Creazione del dashboard RTP**

Crea un [nuovo dashboard](https://microsite.omniture.com/t2/help/en_US/sc/user/t_dashboard_add.html), chiamato **Dashboard RTP**. Questa dashboard ti aiuterà a comprendere la suddivisione dei visitatori in base ai segmenti verticali e RTP.

1. Fai clic su **Dashboard** click **Aggiungi dashboard**.

1. Assegna un nome al dashboard **Dashboard RTP**.

1. Seleziona la **dimensione del dashboard** 3 x 2, 2 x 2

1. Crea il [reportlet](https://microsite.omniture.com/t2/help/en_US/sc/user/t_dashboard_add_report.html#task_EC3AFBBAA51C45CEBAF632F841C305B3) e aggiungere [contenuto nel dashboard](https://docs.marketo.com/Add%2520content%2520to%2520a%2520dashboard).

Aggiunta del Reportlet Industrie al Dashboard

1. Vai a **Conversioni personalizzate**, fai clic su **Industria**.

1. Configurare Graph per **Grafico a torta**.

1. Fai clic su **Dashboard**, aggiungi **Report**.

1. Denomina il report **Settori principali**.

1. Posiziona nel dashboard **Dashboard RTP**.

1. Crea **Nuovo**.

Aggiunta del reportlet Segmenti al dashboard

1. Vai a **Metriche del sito**. Fai clic su **Eventi personalizzati**, **Segmenti**.

1. Configurare Graph per **Barre verticali**.

1. Fai clic su **Dashboard**, aggiungi **Report**.

1. Denomina il report **Segmenti principali**.

1. Posiziona nel dashboard **Dashboard RTP**.

1. Crea **Nuovo**.

I minirapporti verranno visualizzati nel dashboard.

## Visualizzare impression e clic (conversioni) in Adobe Analytics {#view-impressions-and-clicks-conversions-in-adobe-analytics}

1. Fai clic su **Collegamenti personalizzati**.

   ![](assets/sitecatalyst1-1.png)

1. Cerca impressioni per visualizzare i nomi dei segmenti e delle campagne che rappresentano il numero di impression per la campagna.\
   ![](assets/sitecatalyst1.png)

1. Cerca Conversione per visualizzare i nomi dei segmenti e delle campagne che rappresentano il numero di clic per la campagna.

   ![](assets/sitecatalyst2.png)
