---
unique-page-id: 10092969
description: Filtro Microsoft Dynamics Sync -Merge - Documenti Marketo - Documentazione del prodotto
title: Filtro di sincronizzazione Microsoft Dynamics -Merge
exl-id: f8da9c3c-0f04-4f61-be03-7e7953d25afe
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 4%

---

# Filtro di sincronizzazione Microsoft Dynamics: Unisci {#microsoft-dynamics-sync-filter-merge}

L’unione dei lead in Microsoft Dynamics utilizza il tipo Due opzioni: Filtro di sincronizzazione = Sì (TRUE) e Filtro di sincronizzazione = No (FALSE). Quando si uniscono due record, il risultato varia a seconda del record True e False.

I record lead diventano true o false in base alle regole del flusso di lavoro definite dall’amministratore per determinare il vincitore. Il filtro di sincronizzazione per il record vincente è ciò che determina in ultima analisi se il record MS Dynamics si sincronizza con Marketo.

È quando un record è vero e uno è falso che diventa complicato.

| Se il filtro di sincronizzazione per il record di perdita è: | e il filtro di sincronizzazione per il record vincente è: | Questo è il risultato in Marketo |
|---|---|---|
| True | True | Il record vincente continua la sincronizzazione con Marketo |
| False | False | Il record vincente continua a **not** sincronizzazione con Marketo |
| False | True | Il record vincente verrà sincronizzato con Marketo |
| True | False | Il record vincente non verrà sincronizzato con Marketo |
