---
unique-page-id: 10092977
description: Filtro di sincronizzazione Microsoft Dynamics - Qualifica - Documentazione Marketo - Documentazione del prodotto
title: Filtro di sincronizzazione di Microsoft Dynamics - Qualifica
exl-id: 9b26795c-fc94-478e-a7f0-ac8e602792b1
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 6%

---

# Filtro sincronizzazione Microsoft Dynamics: qualificato {#microsoft-dynamics-sync-filter-qualify}

Quando si desidera convertire un lead in un contatto in Microsoft Dynamics, assicurarsi di utilizzare questo processo di qualificazione predefinito. Quindi, sincronizzalo con Marketo.

## Il processo di conversione {#the-conversion-process}

Ecco come funzionano i filtri durante il processo di conversione.

| Se il filtro di sincronizzazione del lead è: | e il filtro di sincronizzazione dei contatti è: | Questo è il risultato in Marketo |
|---|---|---|
| False | False | Non viene sincronizzato nulla in Marketo |
| True | True | Il contatto è sincronizzato in Marketo |
| False | True | Nuovo record contatto creato in Marketo |
| True | False | MS Dynamics aggiorna le informazioni del lead in Marketo, ma il record del contatto non è sincronizzato |

>[!CAUTION]
>
>Supportiamo solo il processo predefinito di conversione Qualify.
