---
unique-page-id: 7514898
description: Impostazione di una campagna di attivazione per le vendite con "Campaign is Required" - Marketo Docs - Documentazione del prodotto
title: Impostazione di una campagna di attivazione per le vendite con "Campaign is Required"
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 0%

---


# Impostazione di una campagna di attivazione per le vendite con &quot;Campaign is Required&quot; {#setting-up-a-trigger-smart-campaign-for-sales-using-campaign-is-requested}

Una delle caratteristiche più interessanti di Marketo è la capacità di consentire alle persone di vendita di partecipare alle attività di marketing. Sono in prima linea, interagiscono con le persone. I rappresentanti delle vendite dovrebbero essere in grado di indirizzare il marketing nella direzione giusta.

>[!NOTE]
>
>**FYI**
>
>Marketo sta standardizzando la lingua tra tutte le iscrizioni, pertanto è possibile che nell&#39;abbonamento siano presenti lead/lead e persone in docs.marketo.com. Questi termini significano la stessa cosa; non influisce sulle istruzioni dell&#39;articolo. Ci sono anche altri cambiamenti. [Ulteriori](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)informazioni.

>[!NOTE]
>
>**Esempio**
>
>Esempi di campagne intelligenti da richiedere:
>
>1. **Allevamento** a lungo termine - quando non hanno un budget quest&#39;anno e si vuole solo rimanere sul radar
>1. **Ciclo** di vendita attivo - quando il venditore non desidera alcun messaggio alla persona tranne il proprio. (utilizzare il flag marketing sospeso per annullarne temporaneamente la sottoscrizione)

>
>
Siate creativi. Cosa vorrebbe automatizzare il venditore? Chiedilo a loro e lo cavi!

1. Create una **Smart Campaign.**

   ![](assets/image2015-5-20-16-3a3-3a25.png)

1. Trova e trascina la **campagna** **è** **Richiesto **nell&#39;area di lavoro.

   ![](assets/campaignfilterdrag.png)

1. Le scelte di origine indicano che tipo di richiesta sarà rispettata. Per la funzionalità Salesforce, accertati di scegliere **Sales** **Insight**.

   >[!TIP]
   >
   >Gli operatori di origine sono per la sicurezza. Potete limitare la campagna alle richieste effettuate solo da origini specifiche, come altre campagne intelligenti o sviluppatori. Scegliete **Qualsiasi** nella prima casella se desiderate consentire le richieste da tutte le origini.
   >
   >
   >**Ricordate**, scegliendo Vendite Insight, verrà magicamente visualizzato nella casella per le vendite. Non esagerate. Troppi verranno ignorati da loro.

   ![](assets/image2015-5-20-17-3a56-3a56.png)

Questo è un ottimo modo per estendere la portata del marketing ad altri reparti. Configurate tutti i tipi di campagne da automatizzare.

>[!TIP]
>
>Non dimenticare di assegnare chiaramente un nome alle campagne intelligenti. Verranno visualizzati in Sales Insight esattamente come li chiami.

