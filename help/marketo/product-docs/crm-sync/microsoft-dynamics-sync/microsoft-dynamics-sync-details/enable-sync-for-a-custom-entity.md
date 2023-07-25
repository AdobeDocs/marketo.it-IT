---
unique-page-id: 2953384
description: Abilitare la sincronizzazione per un’entità personalizzata - Documentazione di Marketo - Documentazione del prodotto
title: Abilitare la sincronizzazione per un'entità personalizzata
exl-id: 4b075bf3-f10b-4725-8c8e-a6ecee63d756
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '224'
ht-degree: 0%

---

# Abilitare la sincronizzazione per un&#39;entità personalizzata {#enable-sync-for-a-custom-entity}

Se hai bisogno che i dati di entità personalizzati da Dynamics siano disponibili in Marketo, ecco come abilitare la sincronizzazione per esso.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

>[!NOTE]
>
>* Quando abiliti la sincronizzazione per un’entità personalizzata, Marketo esegue una sincronizzazione iniziale per inserire tutti i dati per l’oggetto personalizzato.
>* I membri dell’elenco di marketing e dell’elenco di marketing sono **non supportato** in questo momento.

>[!IMPORTANT]
>
>L&#39;utente di Marketo Sync ha bisogno dell&#39;accesso in lettura all&#39;oggetto personalizzato per elencarlo ed eseguire una sincronizzazione.

1. Vai a **Amministratore** sezione.

   ![](assets/enable-sync-for-a-custom-entity-1.png)

1. Seleziona **Microsoft Dynamics** e fai clic su **Disattiva sincronizzazione**.

   ![](assets/enable-sync-for-a-custom-entity-2.png)

   >[!NOTE]
   >
   >Per abilitare o disabilitare un’entità personalizzata, è necessario disabilitare temporaneamente la sincronizzazione globale.

1. In Gestione database fare clic su **Sincronizzazione entità Dynamics** collegamento.

   ![](assets/enable-sync-for-a-custom-entity-3.png)

1. Fai clic su **Sincronizza schema** collegamento.

   ![](assets/enable-sync-for-a-custom-entity-4.png)

1. Seleziona l’entità da sincronizzare e fai clic su **Abilita sincronizzazione**.

   ![](assets/enable-sync-for-a-custom-entity-5.png)

1. Selezionare i campi da sincronizzare o utilizzare come [vincoli](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-a-constraint-to-a-smart-list-filter.md) e/o trigger negli elenchi smart. Al termine, fai clic su **Abilita sincronizzazione**.

   ![](assets/enable-sync-for-a-custom-entity-6.png)

   >[!NOTE]
   >
   >Durante il processo di sincronizzazione, è possibile che l&#39;elemento &quot;Sincronizzazione entità dinamiche&quot; scompaia dalla struttura di navigazione. Si tratta di un comportamento previsto che verrà visualizzato nuovamente al termine della sincronizzazione.

1. L’entità ora presenta un segno di spunta verde.

   ![](assets/enable-sync-for-a-custom-entity-7.png)

1. Non dimenticare di riattivare la sincronizzazione globale.

   ![](assets/enable-sync-for-a-custom-entity-8.png)
