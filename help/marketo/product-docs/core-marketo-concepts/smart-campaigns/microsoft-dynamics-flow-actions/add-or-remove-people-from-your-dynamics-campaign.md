---
description: Aggiungere o rimuovere persone dalla tua Dynamics Campaign - Documentazione di Marketo - Documentazione del prodotto
title: Aggiungere o rimuovere persone da Dynamics Campaign
exl-id: 4fea2f7c-0655-4816-8640-76878f760b6e
feature: Smart Campaigns, Microsoft Dynamics
source-git-commit: 2eeb7ea7fd43ba75a3c802a91ce07c90dc8abd91
workflow-type: tm+mt
source-wordcount: '317'
ht-degree: 0%

---

# Aggiungere o rimuovere persone da Dynamics Campaign {#add-or-remove-people-from-your-dynamics-campaign}

## Aggiungi a Dynamics Campaign {#add-to-dynamics-campaign}

Questo passaggio di flusso può essere utilizzato nelle campagne intelligenti di Marketo Engage per aggiungere persone come lead o contatti in una campagna Microsoft. Se il lead non esiste ancora in Dynamics, verrà automaticamente sincronizzato e aggiunto alla campagna.

>[!NOTE]
>
>Questa azione di flusso è disponibile solo per Attivare campagne.

In Smart Campaign, individua e seleziona la campagna Dynamics a cui desideri aggiungere le persone.

![](assets/add-or-remove-people-from-your-dynamics-campaign-1.png)

>[!NOTE]
>
>Se non riesci a visualizzare una campagna Dynamics nell’elenco delle campagne:
>
>* Assicurati che Campaign Sync sia funzionante
>* La campagna non è attiva in [!DNL Microsoft Dynamics]

Il sistema crea automaticamente un elenco di marketing statico specifico per la campagna, ciascuno per lead e contatti, a cui aggiungere la persona. Si tratta di un’azione una tantum; per le successive sincronizzazioni con la campagna, viene utilizzato lo stesso elenco di marketing. Lo standard di denominazione adottato per il nome dell&#39;elenco di marketing statico è `Mkto-leads-<uniqueID>` per i lead e `Mkto-contacts-<uniqueID>` per i contatti.

L’associazione di questi elenchi di marketing generati da Marketo ad altre campagne potrebbe causare confusione. Ad esempio: l’aggiunta a una campagna determinerebbe anche l’aggiunta alla seconda campagna. Allo stesso modo, non è consigliabile dissociare l’elenco di marketing generato da Marketo dalla campagna in Dynamics.

## Rimuovi da Dynamics Campaign {#remove-from-dynamics-campaign}

Questo passaggio di flusso può essere utilizzato nelle campagne Marketo Smart per rimuovere utenti da una campagna Microsoft. In questo modo vengono rimossi da una campagna solo i lead precedentemente aggiunti alla campagna tramite l’azione di flusso &quot;Aggiunto a Microsoft Campaign&quot;.

>[!NOTE]
>
>Questa azione di flusso è disponibile solo per Attivare campagne.

In Smart Campaign, individua e seleziona la campagna Dynamics da cui desideri rimuovere le persone.

![](assets/add-or-remove-people-from-your-dynamics-campaign-2.png)

>[!NOTE]
>
>Se nell’elenco delle campagne non è presente una campagna Dynamics:
>
>* Assicurati che Campaign Sync sia funzionante
>* La campagna non è attiva in [!DNL Microsoft Dynamics]
