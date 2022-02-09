---
unique-page-id: 2953384
description: Abilita sincronizzazione per un'entità personalizzata - Documentazione di Marketo - Documentazione del prodotto
title: Abilita sincronizzazione per un'entità personalizzata
exl-id: 4b075bf3-f10b-4725-8c8e-a6ecee63d756
source-git-commit: dadaf5bd8e887309d0e9ee8fc25fc58d1c4fbe97
workflow-type: tm+mt
source-wordcount: '204'
ht-degree: 0%

---

# Abilita sincronizzazione per un&#39;entità personalizzata {#enable-sync-for-a-custom-entity}

Se hai bisogno di dati di entità personalizzati da Dynamics per essere disponibili in Marketo, ecco come abilitare la sincronizzazione per questo.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

>[!NOTE]
>
>* Quando abiliti la sincronizzazione per un’entità personalizzata, Marketo esegue una sincronizzazione iniziale per inserire tutti i dati per l’oggetto personalizzato.
>* I membri della lista di marketing e della lista di marketing sono **non supportato** in questo momento.


1. Vai a **Amministratore** sezione .

   ![](assets/enable-sync-for-a-custom-entity-1.png)

1. Seleziona **Microsoft Dynamics** e fai clic su **Disattiva sincronizzazione**.

   ![](assets/enable-sync-for-a-custom-entity-2.png)

   >[!NOTE]
   >
   >È necessario disattivare temporaneamente la sincronizzazione globale per abilitare o disabilitare un&#39;entità personalizzata.

1. In Gestione database fare clic sul pulsante **Sincronizzazione entità Dynamics** link.

   ![](assets/enable-sync-for-a-custom-entity-3.png)

1. Fai clic sul pulsante **Schema di sincronizzazione** link.

   ![](assets/enable-sync-for-a-custom-entity-4.png)

1. Seleziona l’entità da sincronizzare e fai clic su **Abilita sincronizzazione**.

   ![](assets/enable-sync-for-a-custom-entity-5.png)

1. Seleziona i campi da sincronizzare o utilizzare come [vincoli](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md) e/o attivatori negli elenchi smart. Al termine, fai clic su **Abilita sincronizzazione**.

   ![](assets/enable-sync-for-a-custom-entity-6.png)

   >[!NOTE]
   >
   >Durante il processo di sincronizzazione, potresti notare che l’elemento &quot;Dynamic Entities Sync&quot; scompare dalla struttura di navigazione. Questo è il comportamento previsto e riapparirà al termine della sincronizzazione.

1. L’entità ora dispone di un segno di spunta verde.

   ![](assets/enable-sync-for-a-custom-entity-7.png)

1. Non dimenticare di riattivare la sincronizzazione globale.

   ![](assets/enable-sync-for-a-custom-entity-8.png)
