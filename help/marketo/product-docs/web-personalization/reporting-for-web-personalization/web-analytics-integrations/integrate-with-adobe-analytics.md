---
unique-page-id: 2949160
description: Integrazione con  Adobe Analytics - Marketo Docs - Documentazione prodotto
title: Integrazione con  Adobe Analytics
translation-type: tm+mt
source-git-commit: fbaf57ec4f3532c2d71acf23171d60873b1c997c
workflow-type: tm+mt
source-wordcount: '1130'
ht-degree: 0%

---


# Integrazione con  Adobe Analytics {#integrate-with-adobe-analytics}

## Introduzione {#intro}

Analizza le tue analisi web da un punto di vista B2B visualizzando i dati delle campagne aziendali, del settore e del marketing in tempo reale (Real-Time Personalization, RTP) nel tuo account Adobe Analytics .

Questo documento consente l&#39;integrazione tra  Adobe Analytics e la RTP (Real-Time Personalization) di Marketo. I dati RTP consentiranno di rilevare e analizzare le tendenze in tutti i segmenti e le organizzazioni del settore che visitano il sito e misurare l&#39;efficacia delle campagne RTP, fornendo informazioni e analisi per ottenere risultati ottimali.

A tal fine, puoi esaminare metriche quali il numero di visitatori nuovi o di ritorno in ciascun segmento, analizzare i tassi di clic sulle campagne e scoprire quali settori, quali segmenti personalizzati e quali campagne in tempo reale hanno generato i migliori lead di conversione. Sfruttate questa capacità per ottenere il massimo vantaggio dal vostro account RTP.

## Audience Analytics  RTP {#rtp-audience-analytics}

Con l&#39;integrazione RTP - AA, hai una nuova dimensione nell&#39;interfaccia di analisi Web. RTP ottimizza automaticamente le dashboard di analisi Web con:

1. Dati relativi all&#39;organizzazione e all&#39;industria
1. Segmenti RTP personalizzati
1. Elenchi Account denominati (Marketing basato su account)

Questo migliora i dati B2B e ti permette di concentrarti sui visitatori rilevanti ottimizzando:

1. Canali in uscita
1. Contenuto
1. Retargeting

## Rapporto canale {#channel-report}

![](assets/image2014-11-29-12-3a0-3a26.png)

Il pannello RTP consente di comprendere la suddivisione dei visitatori in base ai segmenti verticali e RTP. Puoi vedere le prestazioni dei visitatori in base al settore e alle diverse campagne di marketing (a pagamento, organiche, social) relative a tale settore. Il dashboard fornisce inoltre una panoramica di alto livello delle sezioni del sito che i visitatori visualizzano in base al tipo di settore.

## Rapporto comportamentale {#behavioral-report}

In  Adobe Analytics è possibile creare diversi rapporti sul comportamento in base ai dati di organizzazione, settore e segmento RTP. Questi rapporti sul flusso visualizzano il percorso che i visitatori passano da una pagina o un evento all’altra. Questo rapporto può aiutarvi a scoprire quali contenuti tengono i visitatori coinvolti nel sito.

## Prestazioni RTP {#rtp-performance}

Visualizza le impression e le conversioni delle campagne RTP in Collegamenti personalizzati in  Adobe Analytics.

Questo rapporto sui collegamenti personalizzati mostrerà le impression e le conversioni delle campagne nel seguente formato di denominazione:

* ISegment dell&#39;impressione: [Nome segmento RTP], ICamaging: [Nome campagna RTP]
* ISegment conversione: [Nome segmento RTP], ICamaging: [Nome campagna RTP]

![](assets/custom-links-report.png)

## Configurare in  Adobe Analytics {#set-up-in-adobe-analytics}

L&#39;integrazione utilizza l&#39;API JavaScript offerta  Adobe Analytics. Nell&#39;integrazione vengono utilizzate variabili di conversione personalizzate ( eVar), eventi personalizzati (evento) e variabili di traffico. Tutto deve essere attivato dall&#39;interno di un amministratore AA. È necessario impostare le variabili di conversione, gli eventi personalizzati e le variabili di traffico in Acrobat, altrimenti non sarà possibile visualizzare i dati nella suite anche se l&#39;hai abilitata in RTP.

Per impostare queste variabili in AA, effettua i seguenti passaggi:

1. Accedi a **Strumenti di amministrazione** nel tuo account AA.
1. Selezionare la **Suite di rapporti** da utilizzare con l&#39;integrazione.
1. In **Edit Settings** (Modifica impostazioni), andare su **Conversion** e selezionare **[Conversion Variables](https://microsite.omniture.com/t2/help/en_US/reference/#Edit_conversion_variables)**.\
   Selezionare il numero [Variabile di conversione](https://microsite.omniture.com/t2/help/en_US/reference/#Conversion_Variables_eVar) (consigliato):

   1. Evar # 20 per le conversioni personalizzate del settore
   1. Evar # 21 per le conversioni personalizzate dell&#39;organizzazione

   >[!NOTE]
   >
   >Se si sceglie #, selezionare un altro numero disponibile. Allineare questo numero con il numero di slot in Impostazioni account RTP.

   1. Cambia stato in _Abilitato_.

      1. Cambia nome in **Industria** e **Organizzazione**. (Questo è come apparirà nella Suite di rapporti.)

      1. Cambia il campo Scade dopo in **Visita**.


1. In **Edit Settings** (Modifica impostazioni), andate a **Conversion** e selezionate **[Success Events](https://microsite.omniture.com/t2/help/en_US/reference/#Configure_success_events)**.

   1. Selezionate il numero evento di successo personalizzato (consigliato):

      1. event20 per le campagne RTP
      1. event21 per i segmenti RTP

      >[!NOTE]
      >
      >Se si sceglie #, selezionare un altro numero disponibile. Allineare questo numero con il numero di slot in Impostazioni account RTP.

      1. Modificate i nomi dei due eventi in **Campagne RTP** e **Segmenti RTP**. Questo è il nome che verrà visualizzato nella Suite di rapporti.
   1. Selezionare il campo Tipo come **Contatore (nessuna sottorelazione)**



1. In **Edit Settings** (Modifica impostazioni), andate a **[Traffic](https://microsite.omniture.com/t2/help/en_US/reference/#Traffic_Variable)** e selezionate **[Traffic Variables](https://microsite.omniture.com/t2/help/en_US/reference/#Enable_traffic_variable_reports)** (Variabili di traffico).

   1. Selezionate la proprietà Variabile traffico # (consigliato):

      1. Proprietà # 20 - Nome: Organizzazione segmento RTP
      1. Proprietà # 21 - Nome: Settore dei segmenti RTP
      1. Proprietà # 25 - Nome: Organizzazione campagna
      1. Proprietà # 26 - Nome: Settore delle campagne RTP

      >[!NOTE]
      >
      >Se si sceglie #, selezionare un altro numero disponibile. Allineare questo numero con il numero di slot in Impostazioni account RTP)

      1. Modificate i nomi delle proprietà 4. Questo è il nome che verrà visualizzato nella Suite di rapporti.
   1. Selezionare il campo Abilitato su **Abilitato**.

   1. Selezionare il campo Report percorso su **Abilitato**.




## Configurazione in Real-Time Personalization (RTP) di Marketo {#set-up-in-marketo-real-time-personalization-rtp}

1. Nella piattaforma RTP, andate a **Impostazioni account**.

   ![](assets/image2014-11-29-11-3a27-3a7.png)

1. In **Impostazioni account**, fare clic su **Dominio**.
1. In **Analytics, fare clic su** **Adobe Analytics**.
1. Attivare **su** le variabili Conversione, Personalizzato e Traffico.
1. Assegnare le variabili di conversione, evento e traffico **numeri di slot** in modo che corrispondano ai numeri di slot creati in AA
1. Fare clic su **Salva**.

![](assets/image2014-11-29-12-3a24-3a42.png)

>[!NOTE]
>
>Le impostazioni consigliate per gli slot sono:
>
>**Variabili di conversione**
>
>* Conversioni personalizzate del settore - Slot 20
>* Conversioni personalizzate organizzazione - Slot 21

>
>
**Eventi personalizzati**
>
>* Evento personalizzato campagna - Slot 20
>* Evento personalizzato segmento - Slot 21

>
>
**Variabili di traffico**
>
>* Variabile di traffico organizzazione segmento - Slot 20
>* Variabile di traffico del settore del segmento - Slot 21
>* Variabile di traffico organizzazione campagna - Slot 22
>* Variabile Traffico Campagna - Slot 23

>
>
**Accertatevi che questi numeri di slot siano allineati con le variabili e i numeri di eventi creati in AA.**

## Rapporti {#reports}

Creazione di report SiteAdobe Analytics ottimizzati in base ai nomi dell&#39;organizzazione, ai settori e ai segmenti RTP e ai dati delle campagne in tempo reale.

Esempi di rapporti e dashboard personalizzati in AA includono:

* Prestazioni per settore o segmento definito (elenchi denominati in base al conto)
* Suddivisione del settore per prestazioni KPI
* Pagine visualizzate per organizzazione
* Prestazioni del canale di marketing in base a Organizzazione, Industria, Segmenti

**-Esempi di rapporti-**

**Report principali settori**

![](assets/top-industries-report.png)

**Rapporto Organizzazioni**

![](assets/image2014-11-29-12-3a29-3a42.png)

**Creazione del dashboard RTP**

Create un [nuovo dashboard](https://microsite.omniture.com/t2/help/en_US/sc/user/t_dashboard_add.html) denominato **dashboard RTP**. Questa dashboard aiuterà a comprendere la suddivisione dei visitatori in base ai segmenti verticali e RTP.

1. Fare clic su **Dashboard,** fare clic su **Aggiungi dashboard**.

1. Denominate il dashboard **Dashboard RTP**.

1. Selezionare la **dimensione del dashboard** 3 x 2, 2 x 2.

1. Creare il [minirapporto](https://microsite.omniture.com/t2/help/en_US/sc/user/t_dashboard_add_report.html#task_EC3AFBBAA51C45CEBAF632F841C305B3) e aggiungere [contenuto al dashboard](https://docs.marketo.com/Add%2520content%2520to%2520a%2520dashboard).

Aggiunta del rapporto Industrie al dashboard

1. Vai a **Conversioni personalizzate**, fai clic su **Industria**.

1. Configurare il grafico su **Grafico a torta**.

1. Fare clic su **Dashboard**, aggiungere **Reportlet**.

1. Denominate il report **Top Industries**.

1. Posizionare nel dashboard **Dashboard RTP**.

1. Create **New**.

Aggiunta del minirapporto Segmenti al dashboard

1. Vai a **Metriche del sito**. Fare clic su **Eventi personalizzati**, **Segments**.

1. Configurare il grafico su **Barra verticale**.

1. Fare clic su **Dashboard**, aggiungere **Reportlet**.

1. Denominate il report **Segmenti principali**.

1. Posizionare nel dashboard **Dashboard RTP**.

1. Create **New**.

I minirapporti verranno visualizzati nel dashboard.

## Visualizza impressioni e clic (conversioni) in  Adobe Analytics {#view-impressions-and-clicks-conversions-in-adobe-analytics}

1. Fare clic su **Collegamenti personalizzati**.

   ![](assets/sitecatalyst1-1.png)

1. Cercate Impressioni per visualizzare i nomi dei segmenti e delle campagne che rappresentano il numero di impression per la campagna.\
   ![](assets/sitecatalyst1.png)

1. Cerca Conversione per visualizzare i nomi dei segmenti e delle campagne che rappresentano il numero di clic per la campagna.

   ![](assets/sitecatalyst2.png)
