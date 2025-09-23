---
unique-page-id: 4719302
description: Abilita sincronizzazione oggetti personalizzati non in inglese - Documentazione di Marketo - Documentazione del prodotto
title: Abilitare la sincronizzazione oggetti personalizzati non inglese
exl-id: 5d1c5b52-5323-4f68-847b-7d24e6acd6c4
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '138'
ht-degree: 8%

---

# Abilitare la sincronizzazione oggetti personalizzati non inglese {#enable-non-english-custom-object-sync}

Se l&#39;utente di Marketo Sync è impostato su una lingua diversa dall&#39;inglese, è possibile che si verifichi un errore quando si tenta di abilitare una sincronizzazione oggetto personalizzata.

## L&#39;errore {#the-error}

![](assets/image2014-12-10-13-3a17-3a51.png)

## Come aggirare il problema {#getting-around-it}

1. Accedere a [!DNL Salesforce] utilizzando l&#39;utente marketo sync.

   ![](assets/image2014-12-10-13-3a18-3a1.png)

1. Sotto il nome utente, vai a **[!UICONTROL Setup]**.

   ![](assets/image2014-12-10-13-3a18-3a11.png)

1. In **[!UICONTROL Personal Information]**, fare clic su **[!UICONTROL My Personal Information]**.

   ![](assets/image2014-12-10-13-3a18-3a22.png)

1. Fai clic su **[!UICONTROL Edit]**.

   ![](assets/image2014-12-10-13-3a18-3a32.png)

1. Cambia **[!UICONTROL Language]** in **[!UICONTROL English]**.

   ![](assets/image2014-12-10-13-3a18-3a45.png)

1. Fai clic su **[!UICONTROL Save]**.

   ![](assets/image2014-12-10-13-3a18-3a55.png)

1. In Marketo, in **[!UICONTROL Admin]** > **[!UICONTROL Salesforce]** > **[!UICONTROL Objects]**, fare clic su **[!UICONTROL Refresh Schema]**.

   ![](assets/image2014-12-10-13-3a19-3a6.png)

1. L&#39;elenco degli oggetti verrà richiamato in inglese. Selezionare l&#39;oggetto desiderato e fare clic su **[!UICONTROL Enable Sync]**.

   ![](assets/image2014-12-10-13-3a19-3a16.png)

1. Osserva che l’oggetto personalizzato è ora abilitato e sincronizzato.

   ![](assets/image2014-12-10-13-3a19-3a26.png)

1. Ora torna a [!DNL Salesforce] e utilizza i passaggi precedenti per ripristinare la lingua preferita dell&#39;utente di sincronizzazione.

>[!NOTE]
>
>Non dimenticare di aggiornare lo schema un&#39;ultima volta per richiamare gli oggetti nella lingua.
