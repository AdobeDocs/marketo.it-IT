---
unique-page-id: 3571846
description: Microsoft Dynamics Sync -Custom Entity Sync - Marketo Docs - Documentazione prodotto
title: Microsoft Dynamics Sync - Sincronizzazione entità personalizzata
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 0%

---


# Microsoft Dynamics Sync: Sincronizzazione entità personalizzata {#microsoft-dynamics-sync-custom-entity-sync}

Se devi abilitare la sincronizzazione entità personalizzata iniziale per rendere disponibili i dati di Dynamics in Marketo, ecco come farlo.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

>[!PREREQUISITES]
>
>Per utilizzare un oggetto personalizzato, deve essere associato a un oggetto [lead](microsoft-dynamics-sync-lead-sync.md), a un [contatto](microsoft-dynamics-sync-contact-sync.md)o a un [](microsoft-dynamics-sync-account-sync.md)oggetto account in Dynamics.

>[!CAUTION]
>
>Accertatevi che la sincronizzazione iniziale sia completata (riceverete una notifica via e-mail) prima di avviare la sincronizzazione per le entità personalizzate.

1. Andate alla sezione Admin.

   ![](assets/image2014-10-20-14-3a32-3a16.png)

1. Fate clic su **Disattiva sincronizzazione** per disattivare temporaneamente la sincronizzazione globale standard.

   ![](assets/image2015-11-10-9-3a0-3a6.png)

1. Installa una versione di Microsoft Dynamics che supporta la sincronizzazione di entità personalizzata (dopo 2_0_0_2). Consultate Rilasci plug-in [Marketo per Microsoft Dynamics](../../../../product-docs/crm-sync/microsoft-dynamics-sync/marketo-plugin-releases-for-microsoft-dynamics.md).
1. Consentite a Marketing Sync User di accedere in lettura alle entità che pianificate di sincronizzare.
1. In Gestione database, fai clic sul collegamento** Dynamics Entities Sync**.

   ![](assets/image2015-11-10-9-3a6-3a55.png)

1. Fate clic sul collegamento **Sincronizza schema** per riportare l&#39;elenco delle entità personalizzate disponibili.

   ![](assets/image2015-11-10-9-3a41-3a37.png)

1. Dopo la sincronizzazione dell&#39;elenco, selezionate i campi da sincronizzare e quelli da utilizzare come [vincoli](../../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md) e/o attivatori negli elenchi smart. Al termine, fate clic su **Abilita sincronizzazione**.

   ![](assets/image2014-10-20-14-3a32-3a55.png)

1. Riattivate la sincronizzazione globale.

   ![](assets/image2015-11-10-9-3a48-3a35.png)

   >[!NOTE]
   >
   >Marketo supporta solo entità personalizzate collegate a entità standard con uno o due livelli di profondità.

   >[!NOTE]
   >
   >I nomi delle entità possono contenere un massimo di** 33 caratteri*.

Sei buono!