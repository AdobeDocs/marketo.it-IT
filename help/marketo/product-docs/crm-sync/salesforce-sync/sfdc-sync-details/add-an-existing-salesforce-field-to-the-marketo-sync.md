---
unique-page-id: 4719308
description: Aggiungi un campo Salesforce esistente a Marketo Sync - Marketo Docs - Documentazione del prodotto
title: Aggiungi un campo Salesforce esistente alla sincronizzazione Marketo
exl-id: 6030aedd-9c4b-411f-89c7-f35fd39b0066
source-git-commit: 81bc90bcccc8073511c9f331471c0cda9f4147cb
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# Aggiungi un campo Salesforce esistente alla sincronizzazione Marketo {#add-an-existing-salesforce-field-to-the-marketo-sync}

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

Di solito, i nuovi campi personalizzati in Salesforce si sincronizzano automaticamente con Marketo. In caso contrario, i campi potrebbero non essere visibili all’utente di Marketo Sync. Ecco come si può riparare questo.

1. Fai clic sul nome e seleziona **Configurazione**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-1.png)

1. Invio **profilo** nella barra di ricerca a sinistra e fai clic su **Profili** sotto **Gestione utenti**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-2.png)

1. Fai clic sul profilo dell’utente di sincronizzazione.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-3.png)

1. Sotto la **Sicurezza a livello di campo** sezione, fai clic su **Visualizza** accanto all’oggetto contenente il campo .

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-4.png)

1. Fai clic su **Modifica**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-5.png)

1. Controlla la **Visibile** per il campo da aggiungere alla sincronizzazione e fai clic su **Salva**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-6.png)

   Dolce! Nel prossimo ciclo di sincronizzazione, Marketo vedrà il campo e avvierà la magia.

   >[!NOTE]
   >
   > Se nel campo sono già presenti valori in Salesforce, questi non si sincronizzano con Marketo fino al prossimo aggiornamento del record.
