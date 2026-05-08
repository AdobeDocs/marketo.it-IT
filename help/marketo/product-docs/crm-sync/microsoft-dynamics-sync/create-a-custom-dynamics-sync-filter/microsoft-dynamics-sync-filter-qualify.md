---
unique-page-id: 10092977
description: Scopri il processo di qualificazione del filtro di sincronizzazione Dynamics durante la conversione di un lead in un contatto. Comprendere in che modo i valori dei filtri di sincronizzazione lead e contatti influiscono sulla sincronizzazione di Marketo.
title: Filtro di sincronizzazione Microsoft Dynamics - Qualifica
exl-id: 9b26795c-fc94-478e-a7f0-ac8e602792b1
feature: Microsoft Dynamics
source-git-commit: d20c398cd1f5ed2646f56995c35a57630c3f2e95
workflow-type: tm+mt
source-wordcount: '116'
ht-degree: 0%

---

# Filtro di sincronizzazione [!DNL Microsoft Dynamics]: qualificato {#microsoft-dynamics-sync-filter-qualify}

Per convertire un lead in un contatto in [!DNL Microsoft Dynamics], utilizzare questo processo di qualificazione predefinito. Quindi, sincronizzalo con Marketo.

## Il processo di conversione {#the-conversion-process}

| Se il filtro di sincronizzazione del lead è: | e il filtro di sincronizzazione dei contatti è: | Questo è il risultato in Marketo |
|---|---|---|
| [!UICONTROL False] | [!UICONTROL False] | Non viene sincronizzato nulla in Marketo |
| [!UICONTROL True] | [!UICONTROL True] | Il contatto è sincronizzato in Marketo |
| [!UICONTROL False] | [!UICONTROL True] | Nuovo record contatto creato in Marketo |
| [!UICONTROL True] | [!UICONTROL False] | [!DNL MS Dynamics] aggiorna le informazioni del lead in Marketo, ma il record del contatto non è sincronizzato |

>[!CAUTION]
>
>Supportiamo solo il processo predefinito di conversione Qualify.
