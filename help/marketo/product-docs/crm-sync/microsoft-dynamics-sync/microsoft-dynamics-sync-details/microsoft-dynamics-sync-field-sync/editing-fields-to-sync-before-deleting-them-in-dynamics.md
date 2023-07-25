---
description: Modifica dei campi da sincronizzare prima di eliminarli in Dynamics - Documenti Marketo - Documentazione del prodotto
title: Modifica dei campi da sincronizzare prima di eliminarli in Dynamics
exl-id: 6fa9f6c0-c69d-478f-b333-13a5c910f577
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '207'
ht-degree: 0%

---

# Modifica dei campi da sincronizzare prima di eliminarli in Dynamics {#editing-fields-to-sync-before-deleting-them-in-dynamics}

A volte può essere utile eliminare i campi in Dynamics. Marketo mantiene l’elenco dei campi come riferimento su cui basare la sincronizzazione. Se un campo viene eliminato in Dynamics mentre la sincronizzazione è attiva, potrebbero verificarsi errori di sincronizzazione. Prima di eliminare un campo, effettua le seguenti operazioni.

1. In Marketo, fai clic su **Amministratore**.

   ![](assets/sync-before-deleting-them-in-dynamics-1.png)

1. In Integrazione, fai clic su **Microsoft Dynamics**.

   ![](assets/sync-before-deleting-them-in-dynamics-2.png)

1. Clic **Disattiva sincronizzazione**.

   ![](assets/sync-before-deleting-them-in-dynamics-3.png)

1. In una nuova scheda del browser, accedi a Dynamics ed elimina i campi desiderati.

1. In Marketo, in Microsoft Dynamics, fai clic su **Modifica** accanto a &quot;Passaggio 2: selezionare i campi da sincronizzare&quot;.

   ![](assets/sync-before-deleting-them-in-dynamics-4.png)

1. Rivedi i campi e fai clic su **Salva**.

   ![](assets/sync-before-deleting-them-in-dynamics-5.png)

>[!CAUTION]
>
>Clic **Salva** è necessario per salvare lo schema aggiornato per la sincronizzazione, anche se non sono state apportate modifiche.

>[!NOTE]
>
>Se la sincronizzazione non viene interrotta prima di eliminare un campo in Dynamics, potrebbero verificarsi errori. In caso contrario, la sincronizzazione verrà interrotta. Prima di riprendere, l’amministratore di Marketo deve rivedere &quot;Seleziona campi da sincronizzare&quot; (discusso in precedenza) e fare clic su **Salva** affinché la sincronizzazione accetti le modifiche dello schema.

Ricordati di abilitare la sincronizzazione dopo il salvataggio delle modifiche.
