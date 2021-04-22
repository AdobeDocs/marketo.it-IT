---
unique-page-id: 10092977
description: Filtro Microsoft Dynamics Sync - Qualifica - Documenti Marketo - Documentazione del prodotto
title: Filtro di sincronizzazione Microsoft Dynamics - Qualifica
exl-id: 9b26795c-fc94-478e-a7f0-ac8e602792b1
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 0%

---

# Filtro di sincronizzazione Microsoft Dynamics: Qualifica {#microsoft-dynamics-sync-filter-qualify}

Per convertire un lead in un contatto in Microsoft Dynamics, assicurati di utilizzare questo processo di qualificazione predefinito. Quindi, sincronizzalo con Marketo.

## Processo di conversione {#the-conversion-process}

Ecco come funzionano i filtri durante il processo di conversione.

| Se il filtro di sincronizzazione lead è: | e il filtro di sincronizzazione dei contatti è: | Questo è il risultato in Marketo |
|---|---|---|
| False | False | Nessun elemento sincronizzato in Marketo |
| True | True | Il contatto viene sincronizzato in Marketo |
| False | True | Nuovo record di contatto creato in Marketo |
| True | False | MS Dynamics aggiorna le informazioni sui lead in Marketo ma il record di contatto non è sincronizzato |

>[!CAUTION]
>
>Supportiamo solo il processo di conversione Qualifica preconfigurato.
