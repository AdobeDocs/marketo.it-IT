---
unique-page-id: 4719308
description: Aggiungere un campo Salesforce esistente a Marketo Sync - Marketo Docs - Documentazione del prodotto
title: Aggiungi un campo Salesforce esistente a Marketo Sync
exl-id: 6030aedd-9c4b-411f-89c7-f35fd39b0066
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# Aggiungi un campo Salesforce esistente a Marketo Sync {#add-an-existing-salesforce-field-to-the-marketo-sync}

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

In genere, i nuovi campi personalizzati in Salesforce vengono sincronizzati automaticamente con Marketo. In caso contrario, i campi potrebbero non essere visibili all&#39;utente di Marketo Sync. Ecco come si può risolvere il problema.

1. Fai clic sul tuo nome e seleziona **Configurazione**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-1.png)

1. Invio **profilo** nella barra di ricerca a sinistra e fai clic su **Profili** in **Gestisci utenti**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-2.png)

1. Fai clic sul profilo dell’utente di sincronizzazione.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-3.png)

1. Sotto **Sicurezza a livello di campo** , fare clic su **Visualizza** accanto all&#39;oggetto che contiene il campo.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-4.png)

1. Clic **Modifica**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-5.png)

1. Controlla la **Visibile** casella di controllo per il campo da aggiungere alla sincronizzazione e fare clic su **Salva**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-6.png)

   Dolce! Al prossimo ciclo di sincronizzazione, Marketo visualizzerà il campo e avvierà la magia.

   >[!NOTE]
   >
   > Se il campo contiene già dei valori in Salesforce, questi non vengono sincronizzati con Marketo fino al successivo aggiornamento del record.
