---
unique-page-id: 10092969
description: Filtro di sincronizzazione Microsoft Dynamics -Merge - Documentazione Marketo - Documentazione del prodotto
title: Filtro di sincronizzazione Microsoft Dynamics - Unione
exl-id: f8da9c3c-0f04-4f61-be03-7e7953d25afe
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '159'
ht-degree: 0%

---

# [!DNL Microsoft] filtro di sincronizzazione Dynamics: unione {#microsoft-dynamics-sync-filter-merge}

L&#39;unione dei lead in [!DNL Microsoft Dynamics] utilizza il tipo Due opzioni: filtro di sincronizzazione = Sì (TRUE) e filtro di sincronizzazione = No (FALSE). Quando si uniscono due record, il risultato varia a seconda del record True e del False.

I record dei lead diventano true o false in base alle regole del flusso di lavoro definite dall&#39;amministratore per determinare il vincitore. Il filtro di sincronizzazione per il record vincente è ciò che determina in ultima analisi se il record [!DNL MS Dynamics] si sincronizza con Marketo.

È quando un record è vero e uno è falso che diventa difficile.

| Se il filtro di sincronizzazione per il record perdente è: | e il filtro di sincronizzazione per il record vincente è: | Questo è il risultato in Marketo |
|---|---|---|
| [!UICONTROL True] | [!UICONTROL True] | Il record vincente continua la sincronizzazione con Marketo |
| [!UICONTROL False] | [!UICONTROL False] | Il record vincente continua con la sincronizzazione di **not** con Marketo |
| [!UICONTROL False] | [!UICONTROL True] | Il record vincente verrà sincronizzato con Marketo |
| [!UICONTROL True] | [!UICONTROL False] | Il record vincente non verrà sincronizzato con Marketo |
