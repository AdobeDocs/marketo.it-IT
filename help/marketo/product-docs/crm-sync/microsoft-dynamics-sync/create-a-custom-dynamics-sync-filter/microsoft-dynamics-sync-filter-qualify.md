---
unique-page-id: 10092977
description: Filtro di sincronizzazione Microsoft Dynamics - Qualifica - Documenti Marketo - Documentazione prodotto
title: Filtro di sincronizzazione Microsoft Dynamics - Qualifica
translation-type: tm+mt
source-git-commit: 96cc6a30c63c8e8dca793a52e4bf7ecaef8c08dc
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 0%

---


# Filtro di sincronizzazione Microsoft Dynamics: Qualifica {#microsoft-dynamics-sync-filter-qualify}

Per convertire un lead in un contatto in Microsoft Dynamics, assicurarsi di utilizzare il processo Qualifica predefinito. Quindi, sincronizzala con Marketo.

## Il processo di conversione {#the-conversion-process}

Ecco come funzionano i filtri durante il processo di conversione.

| Se il filtro di sincronizzazione dei lead è: | e il filtro di sincronizzazione dei contatti è: | Questo è il risultato in Marketo |
|---|---|---|
| False | False | Nessuna sincronizzazione in Marketo |
| True | True | Il contatto è sincronizzato in Marketo |
| False | True | Nuovo record di contatto creato in Marketo |
| True | False | MS Dynamics aggiorna le informazioni lead in Marketo, ma il record di contatto non è sincronizzato |

>[!CAUTION]
>
>Supportiamo solo il processo di conversione Qualifica fornito.

