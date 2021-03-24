---
description: Modifica dei campi da sincronizzare prima di eliminarli in Dynamics - Documenti Marketo - Documentazione del prodotto
title: Modifica dei campi da sincronizzare prima di eliminarli in Dynamics
translation-type: tm+mt
source-git-commit: ed9399396c82a3b2fb93c83ffdaa1dc7b0827306
workflow-type: tm+mt
source-wordcount: '207'
ht-degree: 0%

---


# Modifica dei campi da sincronizzare prima di eliminarli in Dynamics {#editing-fields-to-sync-before-deleting-them-in-dynamics}

A volte può essere utile eliminare i campi in Dynamics. Marketo mantiene l’elenco dei campi come riferimento su cui basare la sincronizzazione. Se un campo viene eliminato in Dynamics mentre la sincronizzazione è attiva, la sincronizzazione potrebbe incontrare errori. Prima di eliminare qualsiasi campo, segui la procedura seguente.

1. In Marketo, fai clic su **Amministratore**.

   ![](assets/sync-before-deleting-them-in-dynamics-1.png)

1. In Integrazione, fai clic su **Microsoft Dynamics**.

   ![](assets/sync-before-deleting-them-in-dynamics-2.png)

1. Fare clic su **Disattiva sincronizzazione**.

   ![](assets/sync-before-deleting-them-in-dynamics-3.png)

1. In una nuova scheda del browser, accedi a Dynamics ed elimina i campi desiderati.

1. Torna a Marketo, in Microsoft Dynamics fai clic su **Modifica** accanto a &quot;Passaggio 2: Selezionare i campi da sincronizzare.&quot;

   ![](assets/sync-before-deleting-them-in-dynamics-4.png)

1. Rivedi i campi e fai clic su **Salva**.

   ![](assets/sync-before-deleting-them-in-dynamics-5.png)

>[!CAUTION]
>
>Per salvare lo schema aggiornato per la sincronizzazione, è necessario fare clic su **Salva** anche se non sono state apportate modifiche.

>[!NOTE]
>
>Se la sincronizzazione non viene arrestata prima di eliminare un campo in Dynamics, la sincronizzazione potrebbe incontrare errori. Se lo fa, la sincronizzazione si arresta. Prima di riprendere, l’amministratore di Marketo deve rivedere &quot;Select Fields to Sync&quot; (descritto in precedenza) e fare clic su **Save** per consentire la sincronizzazione per accettare le modifiche dello schema.

Ricorda di abilitare la sincronizzazione dopo il salvataggio delle modifiche.
