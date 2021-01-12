---
unique-page-id: 2360354
description: Aggiungi Munchkin Tracking Code al tuo sito web - Marketo Docs - Documentazione del prodotto
title: Aggiungi Munchkin Tracking Code al tuo sito Web
translation-type: tm+mt
source-git-commit: 78961a3e163ce903facf955a9dda6909b5e85bad
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---


# Aggiungi il codice di monitoraggio Munchkin al tuo sito Web {#add-munchkin-tracking-code-to-your-website}

Il codice di tracciamento JavaScript personalizzato di Marketo, chiamato Munchkin, tiene traccia di tutti gli utenti che visitano il sito Web e potrai reagire alle loro visite con campagne di marketing automatizzate. Anche i visitatori anonimi vengono tracciati con i loro indirizzi IP e altre informazioni. **Senza questo codice di tracciamento, non potrai monitorare visite o altre attività sul tuo sito Web**!

>[!PREREQUISITES]
>
>Assicuratevi di avere accesso a uno sviluppatore JavaScript esperto. Il supporto tecnico di Marketo non è configurato per la risoluzione dei problemi relativi a JavaScript personalizzati.

## Aggiungi codice di tracciamento al tuo sito Web {#add-tracking-code-to-your-website}

>[!NOTE]
>
>I clienti Adobe Experience Cloud possono inoltre utilizzare l&#39;integrazione di Marketo  Launch Adobe per includere nelle proprie pagine Web lo script Munchkin. Scarica l&#39;app [qui](https://www.adobeexchange.com/experiencecloud.details.101054.html).

1. Accedete a **Admin** e fate clic su **Munchkin** nella struttura ad albero a sinistra.

   ![](assets/image2015-8-25-16-3a21-3a14.png)

   Selezionare Asincrono per Tipo di codice di tracciamento.

   ![](assets/image2015-8-25-16-3a24-3a33.png)

   >[!NOTE]
   >
   >In quasi tutti i casi, è necessario utilizzare il codice asincrono. [Ulteriori informazioni.](#types-of-munchkin-tracking-codes)

   Fai clic su e copia il codice di tracciamento JavaScript da inserire nel tuo sito Web.

   ![](assets/image2015-8-25-16-3a26-3a12.png)

   >[!CAUTION]
   >
   >Non utilizzate il codice mostrato in questa schermata; dovete usare il codice univoco che appare nel vostro account!

   >[!TIP]
   >
   >Inserite il codice di tracciamento nelle pagine Web da monitorare. Può trattarsi di ogni pagina per siti più piccoli, o solo di pagine chiave per siti con molte pagine Web generate in modo dinamico, forum utenti e così via.

   Per risultati ottimali, usate il codice Munchkin asincrono e inseritelo negli elementi `<head>` delle pagine. Se si utilizza il codice semplice (non consigliato), questo è immediatamente prima del tag `</body>`.
   ![](assets/image2015-8-25-16-3a5-3a20.png)

>[!TIP]
>
>Per i siti che visualizzano un elevato volume di traffico (ovvero centinaia di migliaia di visite al mese), si consiglia di non monitorare persone anonime. [Ulteriori](https://developers.marketo.com/documentation/websites/lead-tracking-munchkin-js/) informazioni.

## Aggiungi codice di tracciamento quando si utilizzano più aree di lavoro {#add-tracking-code-when-using-multiple-workspaces}

Se utilizzate Workspaces nell’account Marketo, probabilmente avrete anche diverse presentazioni Web che corrispondono alle vostre aree di lavoro. In tal caso, potete utilizzare il Javascript di tracciamento Munchkin per assegnare le persone anonime al workspace e alla partizione corretti.

1. Accedete a **Admin** e fate clic su **Munchkin** nella struttura ad albero a sinistra.

![](assets/image2015-8-25-16-3a28-3a41.png)

1. Selezionate l’area di lavoro appropriata per le pagine Web da monitorare.

   ![](assets/image2015-8-25-16-3a30-3a32.png)

>[!NOTE]
>
>Se non si utilizza il codice speciale dell&#39;area di lavoro Munchkin, le persone verranno assegnate alla partizione predefinita creata al momento della configurazione dell&#39;account. Inizialmente si chiama &quot;Default&quot;, ma potreste averlo modificato nel vostro account Marketo.

1. Selezionare **Asynchronous** per il tipo di codice di tracciamento.

   ![](assets/image2015-8-25-16-3a32-3a42.png)

1. Fate clic su e copiate il codice di tracciamento JavaScript da inserire nel sito Web.

   ![](assets/image2015-8-25-16-3a34-3a7.png)

   >[!CAUTION]
   >
   >Non utilizzate il codice mostrato in questa schermata; dovete usare il codice univoco che appare nel vostro account!

1. Inserite il codice di tracciamento nelle pagine Web nell&#39;elemento `<head>`. Le nuove persone che visitano questa pagina verranno assegnate a questa partizione.

   ![](assets/image2015-8-25-16-3a5-3a20.png)

>[!CAUTION]
>
>È possibile utilizzare un solo script di tracciamento Munchkin per una singola partizione e area di lavoro su una pagina. Non includete script di tracciamento per più partizioni/aree di lavoro nel sito Web.

>[!NOTE]
>
>Le pagine di destinazione create in Marketo contengono automaticamente il codice di tracciamento, pertanto non è necessario inserirvi questo codice.

## Tipi di codici di monitoraggio Munchkin {#types-of-munchkin-tracking-codes}

Potete scegliere tra tre tipi di codici di monitoraggio Munchkin. Ogni aspetto ha un impatto diverso sui tempi di caricamento delle pagine Web.

1. **Semplice**: contiene il numero minimo di righe di codice, ma non viene ottimizzata per il tempo di caricamento della pagina Web. Questo codice carica la libreria jQuery ogni volta che viene caricata una pagina Web.
1. **Asincrono**: riduce il tempo di caricamento della pagina Web.
1. **jQuery** asincrona: riduce i tempi di caricamento delle pagine Web e migliora anche le prestazioni del sistema. Questo codice presuppone che sia già presente jQuery e non controlla per caricarlo.

## Verifica se il codice Munchkin funziona {#test-if-your-munchkin-code-is-working}

Per verificare che il codice Munchkin funzioni dopo averlo aggiunto:

1. Visita la tua pagina Web.

1. Vai a **Analytics**.

   ![](assets/mainnav-analytics-hand.png)

1. Fare clic su **Attività pagina Web**.

   ![](assets/webanalytics.png)

1. Fare clic sulla scheda **Configurazione**, fare doppio clic su **Origine attività** e modificarla in **Visitatori anonimi (inclusi ISP)**.

   ![](assets/analytics-activity-source.png)

   ![](assets/activitysource.png)

1. Fare clic sulla scheda **Report**. Se non visualizzi alcun dato, attendi alcuni minuti, quindi fai clic sull&#39;icona di aggiornamento in basso.
