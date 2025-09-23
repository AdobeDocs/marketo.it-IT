---
description: Modifica dei campi da sincronizzare prima di eliminarli in Dynamics - Documenti Marketo - Documentazione del prodotto
title: Modifica dei campi da sincronizzare prima di eliminarli in Dynamics
exl-id: 6fa9f6c0-c69d-478f-b333-13a5c910f577
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 5%

---

# Modifica dei campi da sincronizzare prima di eliminarli in [!DNL Dynamics] {#editing-fields-to-sync-before-deleting-them-in-dynamics}

A volte può essere utile eliminare i campi in [!DNL Dynamics]. Marketo mantiene l’elenco dei campi come riferimento su cui basare la sincronizzazione. Se un campo viene eliminato in [!DNL Dynamics] mentre la sincronizzazione è attiva, potrebbero verificarsi errori di sincronizzazione. Prima di eliminare un campo, effettua le seguenti operazioni.

1. In Marketo, fare clic su **[!UICONTROL Admin]**.

   ![](assets/sync-before-deleting-them-in-dynamics-1.png)

1. In [!UICONTROL Integration], fare clic su **[!UICONTROL Microsoft Dynamics]**.

   ![](assets/sync-before-deleting-them-in-dynamics-2.png)

1. Fai clic su **[!UICONTROL Disable Sync]**.

   ![](assets/sync-before-deleting-them-in-dynamics-3.png)

1. In una nuova scheda del browser, accedi a [!DNL Dynamics] ed elimina i campi desiderati.

1. In Marketo, in [!DNL Microsoft Dynamics], fare clic su **[!UICONTROL Edit]** accanto a &quot;[!UICONTROL Step 2: Select Fields to Sync]&quot;.

   ![](assets/sync-before-deleting-them-in-dynamics-4.png)

1. Rivedere i campi e fare clic su **[!UICONTROL Save]**.

   ![](assets/sync-before-deleting-them-in-dynamics-5.png)

>[!CAUTION]
>
>È necessario fare clic su **[!UICONTROL Save]** per salvare lo schema aggiornato per la sincronizzazione, anche se non sono state apportate modifiche.

>[!NOTE]
>
>Se la sincronizzazione non viene interrotta prima di eliminare un campo in [!DNL Dynamics], potrebbero verificarsi errori. In caso contrario, la sincronizzazione verrà interrotta. Prima di riprendere, l&#39;amministratore di Marketo deve rivedere &quot;[!UICONTROL Select Fields to Sync]&quot; (discusso in precedenza) e fare clic su **[!UICONTROL Save]** per consentire alla sincronizzazione di accettare le modifiche allo schema.

Ricordati di abilitare la sincronizzazione dopo il salvataggio delle modifiche.
