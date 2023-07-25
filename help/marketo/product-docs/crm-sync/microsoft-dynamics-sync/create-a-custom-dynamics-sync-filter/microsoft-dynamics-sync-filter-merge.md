---
unique-page-id: 10092969
description: Filtro di sincronizzazione Microsoft Dynamics - Unione - Documenti Marketo - Documentazione del prodotto
title: Filtro sincronizzazione Microsoft Dynamics - Unione
exl-id: f8da9c3c-0f04-4f61-be03-7e7953d25afe
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 4%

---

# Filtro sincronizzazione Microsoft Dynamics: Unisci {#microsoft-dynamics-sync-filter-merge}

L’unione di lead in Microsoft Dynamics utilizza il tipo Due opzioni: filtro di sincronizzazione = Sì (TRUE) e filtro di sincronizzazione = No (FALSE). Quando si uniscono due record, il risultato varia a seconda del record True e del False.

I record dei lead diventano true o false in base alle regole del flusso di lavoro definite dall&#39;amministratore per determinare il vincitore. Il filtro di sincronizzazione per il record vincente è ciò che determina in ultima analisi se il record MS Dynamics si sincronizza con Marketo.

È quando un record è vero e uno è falso che diventa difficile.

| Se il filtro di sincronizzazione per il record perdente è: | e il filtro di sincronizzazione per il record vincente è: | Questo è il risultato in Marketo |
|---|---|---|
| True | True | Il record vincente continua la sincronizzazione con Marketo |
| False | False | Il record vincente continua a **non** sincronizza con Marketo |
| False | True | Il record vincente verrà sincronizzato con Marketo |
| True | False | Il record vincente non verrà sincronizzato con Marketo |
