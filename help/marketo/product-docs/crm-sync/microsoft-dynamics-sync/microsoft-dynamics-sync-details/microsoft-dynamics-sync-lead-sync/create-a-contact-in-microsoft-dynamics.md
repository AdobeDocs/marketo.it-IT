---
unique-page-id: 10095389
description: Scopri come creare un contatto in Microsoft Dynamics da Marketo. Utilizza l’azione di flusso Sincronizza persona con Microsoft in una campagna di attivazione per la creazione di contatti in tempo reale.
title: Creare un contatto in Microsoft Dynamics
exl-id: 66cb26c0-f383-4d1e-be22-e7f8c6b266fb
feature: Microsoft Dynamics
TQID: 'https://experienceleague.adobe.com/5q84B57P88MNhaYHluCKKCYLwOonW2xj7hAUNDOmXl8'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
    internal-label: Integrations
subfeature_v2:
  - id: d5c7388a-594e-4d15-9b39-98d6ce479e8b
    internal-label: Microsoft Dynamics
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '120'
ht-degree: 5%
---
# Crea un contatto in [!DNL Microsoft Dynamics] {#create-a-contact-in-microsoft-dynamics}

1. Seleziona la persona solo Marketo Engage (il tipo di Microsoft è vuoto) che desideri creare come contatto in Dynamics.

   ![](assets/one.png)

1. Fare clic su **[!UICONTROL Person Actions]** e **[!DNL Microsoft]** e selezionare **[!UICONTROL Sync Person to Microsoft]**.

   ![](assets/two.png)

1. Fare clic su **[!UICONTROL Sync As]** e selezionare **[!UICONTROL Contact]**. Fai clic su **[!UICONTROL Run Now]**.

   ![](assets/three.png)

   >[!NOTE]
   >
   >Quando si utilizza l&#39;azione di flusso &quot;[!UICONTROL Sync Person to Microsoft]&quot; (solo in una campagna Trigger), il lead/contatto verrà creato in tempo reale in Dynamics.

1. Marketo qualifica il record Lead in [!DNL Dynamics] come contatto non associato ad alcun account in [!DNL Dynamics].

   ![](assets/image2015-10-23-9-3a43-3a33.png)

1. È ora possibile selezionare **[!UICONTROL Contact]** quando si utilizza il vincolo Sincronizza con nome in un filtro Smart Campaign.

   ![](assets/five.png)
