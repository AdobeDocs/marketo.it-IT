---
unique-page-id: 2953384
description: Abilita sincronizzazione per un'entità personalizzata - Documentazione di Marketo - Documentazione del prodotto
title: Abilita sincronizzazione per un'entità personalizzata
exl-id: 4b075bf3-f10b-4725-8c8e-a6ecee63d756
translation-type: tm+mt
source-git-commit: d81a4a3caa12c5ec642afadf9328b3825bde6fed
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 0%

---

# Abilita sincronizzazione per un&#39;entità personalizzata {#enable-sync-for-a-custom-entity}

Se hai bisogno di dati di entità personalizzati da Dynamics per essere disponibili in Marketo, ecco come abilitare la sincronizzazione per questo:

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

>[!NOTE]
>
>Quando abiliti la sincronizzazione per un’entità personalizzata, Marketo esegue una sincronizzazione iniziale per inserire tutti i dati per l’oggetto personalizzato.

1. Vai alla sezione **Amministratore** .

   ![](assets/image2014-10-20-14-3a32-3a16.png)

1. Seleziona **Microsoft Dynamics** e fai clic su **Disattiva sincronizzazione**.

   È necessario disattivare temporaneamente la sincronizzazione globale per abilitare o disabilitare un&#39;entità personalizzata.

   ![](assets/image2015-11-10-9-3a0-3a6.png)

1. In Gestione database fare clic sul collegamento **Sincronizzazione entità Dynamics**.

   ![](assets/image2015-11-10-9-3a6-3a55.png)

1. Fare clic sul collegamento **Sincronizza schema**.

   ![](assets/image2015-11-10-9-3a41-3a37.png)

1. Seleziona l&#39;entità da sincronizzare e fai clic su **Abilita sincronizzazione**.

   ![](assets/image2015-11-10-9-3a44-3a35.png)

1. Seleziona i campi da sincronizzare o utilizzare come [vincoli](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md) e/o attivatori negli elenchi smart. Al termine, fai clic su **Abilita sincronizzazione**.

   ![](assets/image2014-10-20-14-3a32-3a55.png)

   >[!NOTE]
   >
   >Durante il processo di sincronizzazione, potresti notare che l’elemento &quot;Dynamic Entities Sync&quot; scompare dalla struttura di navigazione. Questo è il comportamento previsto e riapparirà al termine della sincronizzazione.

1. L’entità ora dispone di un segno di spunta verde.

   ![](assets/image2014-10-20-14-3a33-3a4.png)

1. Non dimenticare di riattivare la sincronizzazione globale.

   ![](assets/image2015-11-10-9-3a48-3a35.png)

Oh sì! Roba potente.
