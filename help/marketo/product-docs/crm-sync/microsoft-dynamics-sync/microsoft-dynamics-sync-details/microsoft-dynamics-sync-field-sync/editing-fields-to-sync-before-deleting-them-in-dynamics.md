---
description: Modifica dei campi da sincronizzare prima di eliminarli in Dynamics - Documenti Marketo - Documentazione del prodotto
title: Modifica dei campi da sincronizzare prima di eliminarli in Dynamics
exl-id: 6fa9f6c0-c69d-478f-b333-13a5c910f577
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 0%

---

# Modifica dei campi da sincronizzare prima di eliminarli in Dynamics {#editing-fields-to-sync-before-deleting-them-in-dynamics}

A volte può essere utile eliminare i campi in Dynamics. Il Marketo Engage mantiene l&#39;elenco dei campi come riferimento su cui basare la sincronizzazione. Se un campo viene eliminato in Dynamics mentre la sincronizzazione è attiva, potrebbero verificarsi errori di sincronizzazione. Prima di eliminare un campo, effettua le seguenti operazioni.

1. In Marketo, fai clic su **[!UICONTROL Amministratore]**.

   ![](assets/sync-before-deleting-them-in-dynamics-1.png)

1. In Integrazione fare clic su **[!UICONTROL Microsoft Dynamics]**.

   ![](assets/sync-before-deleting-them-in-dynamics-2.png)

1. Fare clic su **[!UICONTROL Disattiva sincronizzazione]**.

   ![](assets/sync-before-deleting-them-in-dynamics-3.png)

1. In una nuova scheda del browser, accedi a Dynamics ed elimina i campi desiderati.

1. In Marketo, in Microsoft Dynamics, fare clic su **[!UICONTROL Modifica]** accanto a &quot;Passaggio 2: Seleziona campi da sincronizzare&quot;.

   ![](assets/sync-before-deleting-them-in-dynamics-4.png)

1. Rivedi i campi e fai clic su **[!UICONTROL Salva]**.

   ![](assets/sync-before-deleting-them-in-dynamics-5.png)

>[!CAUTION]
>
>È necessario fare clic su **[!UICONTROL Salva]** per salvare lo schema aggiornato per la sincronizzazione, anche se non sono state apportate modifiche.

>[!NOTE]
>
>Se la sincronizzazione non viene interrotta prima di eliminare un campo in Dynamics, potrebbero verificarsi errori. In caso contrario, la sincronizzazione verrà interrotta. Prima di riprendere, l&#39;amministratore di Marketo deve rivedere &quot;Seleziona campi da sincronizzare&quot; (discusso in precedenza) e fare clic su **[!UICONTROL Salva]** per consentire alla sincronizzazione di accettare le modifiche allo schema.

Ricordati di abilitare la sincronizzazione dopo il salvataggio delle modifiche.
