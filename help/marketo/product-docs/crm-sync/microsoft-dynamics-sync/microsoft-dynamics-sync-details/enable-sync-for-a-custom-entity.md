---
unique-page-id: 2953384
description: Abilitare la sincronizzazione per un’entità personalizzata - Documentazione di Marketo - Documentazione del prodotto
title: Abilitare la sincronizzazione per un'entità personalizzata
exl-id: 4b075bf3-f10b-4725-8c8e-a6ecee63d756
feature: Microsoft Dynamics
source-git-commit: 4f36194fb76fd8e26c2fd6fe49526d88d355a24a
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 0%

---

# Abilitare la sincronizzazione per un&#39;entità personalizzata {#enable-sync-for-a-custom-entity}

Se sono necessari dati di entità personalizzati da [!DNL Dynamics] per essere disponibili in Marketo Engage, di seguito viene illustrato come abilitare la sincronizzazione per tale entità.

>[!PREREQUISITES]
>
>Per utilizzare un oggetto personalizzato, è necessario associarlo a un oggetto [lead](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-lead-sync.md){target="_blank"}, [contact](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-contact-sync.md){target="_blank"} o [account](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/microsoft-dynamics-sync-details/microsoft-dynamics-sync-account-sync.md){target="_blank"} in Microsoft Dynamics.

>[!NOTE]
>
>* Quando abiliti la sincronizzazione per un’entità personalizzata, Marketo esegue una sincronizzazione iniziale per inserire tutti i dati per l’oggetto personalizzato.
>* Al momento, i membri dell&#39;elenco di marketing e dell&#39;elenco di marketing sono _non supportati_.

>[!IMPORTANT]
>
>L&#39;utente di Marketo Sync ha bisogno dell&#39;accesso in lettura all&#39;oggetto personalizzato per elencarlo ed eseguire una sincronizzazione.

1. Passare alla sezione **[!UICONTROL Admin]**.

   ![](assets/enable-sync-for-a-custom-entity-1.png)

1. Selezionare **[!UICONTROL Microsoft Dynamics]** e fare clic su **[!UICONTROL Disable Sync]**.

   ![](assets/enable-sync-for-a-custom-entity-2.png)

   >[!NOTE]
   >
   >È necessario disattivare temporaneamente la sincronizzazione globale per abilitare o disabilitare un&#39;entità personalizzata.

1. In [!UICONTROL Database Management], fare clic sul collegamento **[!UICONTROL Dynamics Entities Sync]**.

   ![](assets/enable-sync-for-a-custom-entity-3.png)

1. Fare clic sul collegamento **[!UICONTROL Sync schema]**.

   ![](assets/enable-sync-for-a-custom-entity-4.png)

1. Selezionare l&#39;entità da sincronizzare e fare clic su **[!UICONTROL Enable Sync]**.

   ![](assets/enable-sync-for-a-custom-entity-5.png)

1. Selezionare i campi da sincronizzare o utilizzare come [vincoli](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md) e/o trigger negli elenchi smart. Al termine, fare clic su **[!UICONTROL Enable Sync]**.

   ![](assets/enable-sync-for-a-custom-entity-6.png)

   >[!NOTE]
   >
   >Durante il processo di sincronizzazione, è possibile che l&#39;elemento &quot;[!UICONTROL Dynamic Entities Sync]&quot; scompaia dalla struttura di navigazione. Si tratta di un comportamento previsto che verrà visualizzato nuovamente al termine della sincronizzazione.

1. L’entità ora dispone di un segno di spunta verde.

   ![](assets/enable-sync-for-a-custom-entity-7.png)

1. Non dimenticare di riattivare la sincronizzazione globale.

   ![](assets/enable-sync-for-a-custom-entity-8.png)

   >[!NOTE]
   >
   >* Marketo supporta solo entità personalizzate collegate a entità standard profonde uno o due livelli.
   >
   >* La struttura ad oggetti personalizzata può mostrare lo stesso oggetto più di una volta, a causa delle sue connessioni dirette con uno degli oggetti principali (ad esempio lead, contatti o account o connessioni indirette attraverso un oggetto intermedio). In questi casi, scegliere l&#39;oggetto più vicino all&#39;oggetto principale e sceglierne solo uno. La scelta dello stesso oggetto più volte può ostacolare la sincronizzazione dell&#39;oggetto personalizzato.
