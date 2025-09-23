---
unique-page-id: 10092977
description: Filtro di sincronizzazione Microsoft Dynamics - Qualifica - Documentazione Marketo - Documentazione del prodotto
title: Filtro di sincronizzazione Microsoft Dynamics - Qualifica
exl-id: 9b26795c-fc94-478e-a7f0-ac8e602792b1
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '108'
ht-degree: 0%

---

# Filtro di sincronizzazione [!DNL Microsoft Dynamics]: qualificato {#microsoft-dynamics-sync-filter-qualify}

Quando si desidera convertire un lead in un contatto in [!DNL Microsoft Dynamics], assicurarsi di utilizzare questo processo di qualificazione predefinito. Quindi, sincronizzalo con Marketo.

## Il processo di conversione {#the-conversion-process}

Ecco come funzionano i filtri durante il processo di conversione.

| Se il filtro di sincronizzazione del lead è: | e il filtro di sincronizzazione dei contatti è: | Questo è il risultato in Marketo |
|---|---|---|
| [!UICONTROL False] | [!UICONTROL False] | Non viene sincronizzato nulla in Marketo |
| [!UICONTROL True] | [!UICONTROL True] | Il contatto è sincronizzato in Marketo |
| [!UICONTROL False] | [!UICONTROL True] | Nuovo record contatto creato in Marketo |
| [!UICONTROL True] | [!UICONTROL False] | [!DNL MS Dynamics] aggiorna le informazioni del lead in Marketo, ma il record del contatto non è sincronizzato |

>[!CAUTION]
>
>Supportiamo solo il processo predefinito di conversione Qualify.
