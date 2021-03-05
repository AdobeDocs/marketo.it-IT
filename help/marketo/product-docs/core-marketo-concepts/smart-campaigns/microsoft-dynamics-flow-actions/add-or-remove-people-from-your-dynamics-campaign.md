---
description: Aggiungere o rimuovere persone dalla campagna Dynamics - Documenti Marketo - Documentazione del prodotto
title: Aggiungere o rimuovere persone da Dynamics Campaign
translation-type: tm+mt
source-git-commit: 1649aae540204bb5de205e3f5b75ec7e968a7da4
workflow-type: tm+mt
source-wordcount: '320'
ht-degree: 0%

---


# Aggiungere o rimuovere persone dalla campagna Dynamics {#add-or-remove-people-from-your-dynamics-campaign}

## Aggiungi a Dynamics Campaign {#add-to-dynamics-campaign}

Questo passaggio di flusso può essere utilizzato in Campagne avanzate di Marketo per aggiungere le persone come lead o contatti in una campagna Microsoft. Se in Dynamics non esiste ancora, il lead viene sincronizzato automaticamente e aggiunto alla campagna.

>[!NOTE]
>
>Questa azione di flusso è disponibile solo per le campagne trigger.

Nella campagna intelligente, individua e seleziona la campagna Dynamics a cui desideri aggiungere le tue persone.

![](assets/add-or-remove-people-from-your-dynamics-campaign-1.png)

>[!NOTE]
>
>Se non è possibile visualizzare una campagna Dynamics nell’elenco delle campagne:
>
>* Assicurati che la sincronizzazione di Campaign funzioni
>* La campagna non è attiva in Microsoft Dynamics


Il sistema crea automaticamente un elenco di marketing statico specifico per la campagna, ciascuno per lead e contatti, a cui aggiungere la persona. Si tratta di un’azione una tantum e una volta per le sincronizzazioni successive alla campagna, viene utilizzato lo stesso elenco di marketing. Lo standard di denominazione adottato per il nome statico dell’elenco di marketing è `Mkto-leads-<uniqueID>` per i lead e `Mkto-contacts-<uniqueID>` per i contatti.

L’associazione di queste liste di marketing generate da Marketo ad altre campagne potrebbe causare comportamenti confusi. Ad esempio: l’aggiunta a una campagna comporterebbe anche l’aggiunta alla seconda campagna. Allo stesso modo, non è consigliabile separare l’elenco di marketing generato da Marketo dalla campagna in Dynamics.

## Rimuovi da Dynamics Campaign {#remove-from-dynamics-campaign}

Questo passaggio di flusso può essere utilizzato in Marketo Smart Campaigns per rimuovere le persone da una campagna Microsoft. Questo rimuove solo i lead da una campagna che sono stati precedentemente aggiunti alla campagna tramite l’azione di flusso &quot;Aggiunto a Microsoft Campaign&quot;.

>[!NOTE]
>
>Questa azione di flusso è disponibile solo per le campagne trigger.

Nella campagna intelligente, individua e seleziona la campagna Dynamics da cui desideri rimuovere le persone.

![](assets/add-or-remove-people-from-your-dynamics-campaign-2.png)

>[!NOTE]
>
>Se nell’elenco delle campagne non viene visualizzata una campagna Dynamics:
>
>* Assicurati che la sincronizzazione di Campaign funzioni
>* La campagna non è attiva in Microsoft Dynamics

