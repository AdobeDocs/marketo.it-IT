---
description: Modifica dei campi da sincronizzare prima di eliminarli in Dynamics - Documenti Marketo - Documentazione del prodotto
title: Modifica dei campi da sincronizzare prima di eliminarli in Dynamics
exl-id: 6fa9f6c0-c69d-478f-b333-13a5c910f577
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
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

1. Fai clic su **Disattiva sincronizzazione**.

   ![](assets/sync-before-deleting-them-in-dynamics-3.png)

1. In una nuova scheda del browser, accedi a Dynamics ed elimina i campi desiderati.

1. In Marketo, in Microsoft Dynamics fai clic su **Modifica** accanto a &quot;Passaggio 2: Selezionare i campi da sincronizzare.&quot;

   ![](assets/sync-before-deleting-them-in-dynamics-4.png)

1. Esamina i campi e fai clic su **Salva**.

   ![](assets/sync-before-deleting-them-in-dynamics-5.png)

>[!CAUTION]
>
>Clic **Salva** è necessario per salvare lo schema aggiornato per la sincronizzazione, anche se non sono state apportate modifiche.

>[!NOTE]
>
>Se la sincronizzazione non viene arrestata prima di eliminare un campo in Dynamics, la sincronizzazione potrebbe incontrare errori. Se lo fa, la sincronizzazione si arresta. Prima di riprendere, l’amministratore di Marketo dovrebbe rivedere &quot;Seleziona campi da sincronizzare&quot; (discusso in precedenza) e fare clic su **Salva** affinché la sincronizzazione accetti le modifiche dello schema.

Ricorda di abilitare la sincronizzazione dopo il salvataggio delle modifiche.
