---
unique-page-id: 10092969
description: Filtro di sincronizzazione di Microsoft Dynamics - Unisci - Documenti Marketo - Documentazione prodotto
title: Filtro di sincronizzazione di Microsoft Dynamics - Unisci
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 0%

---


# Filtro di sincronizzazione Microsoft Dynamics: Unisci {#microsoft-dynamics-sync-filter-merge}

L&#39;unione dei lead in Microsoft Dynamics utilizza il tipo due opzioni: filtro di sincronizzazione = Sì (TRUE) e filtro di sincronizzazione = No (FALSE). Quando si uniscono due record, il risultato varia a seconda del record vero e falso.

I record lead diventano veri o falsi in base alle regole del flusso di lavoro definite dall’amministratore per determinare il vincitore. Il filtro di sincronizzazione per il record vincente è ciò che determina in ultima analisi se il record MS Dynamics si sincronizza con Marketo.

È quando un record è vero e uno è falso che diventa complicato.

| Se il filtro di sincronizzazione per il record di perdita è: | e il filtro di sincronizzazione per il record vincente è: | Questo è il risultato in Marketo |
|---|---|---|
| True | True | Il record vincente continua a sincronizzarsi con Marketo |
| False | False | Il record vincente continua a **non** sincronizzarsi con Marketo |
| False | True | Il record vincente si sincronizzerà con Marketo |
| True | False | Il record vincente non verrà sincronizzato con Marketo |

