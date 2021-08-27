---
unique-page-id: 4719308
description: Aggiungi un campo Salesforce esistente a Marketo Sync - Marketo Docs - Documentazione del prodotto
title: Aggiungi un campo Salesforce esistente alla sincronizzazione Marketo
exl-id: 6030aedd-9c4b-411f-89c7-f35fd39b0066
source-git-commit: 7376804bda915d7ff25cdc50cb78a6686bd36882
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# Aggiungi un campo Salesforce esistente alla sincronizzazione Marketo {#add-an-existing-salesforce-field-to-the-marketo-sync}

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

Di solito, i nuovi campi personalizzati in Salesforce si sincronizzano automaticamente con Marketo. In caso contrario, i campi potrebbero non essere visibili all’utente di Marketo Sync. Ecco come si può riparare questo.

1. Fai clic sul tuo nome e seleziona **Configurazione**.

   ![](assets/image2015-6-30-14-3a20-3a6.png)

1. Inserisci **profilo** nella barra di ricerca a sinistra e fai clic su **Profili** in **Gestisci utenti**.

   ![](assets/image2015-6-30-14-3a20-3a52.png)

1. Fai clic sul profilo dell’utente di sincronizzazione.

   ![](assets/image2015-6-30-14-3a23-3a41.png)

1. Nella sezione **Sicurezza a livello di campo**, fai clic su **Visualizza** accanto all’oggetto che contiene il campo.

   ![](assets/image2015-6-30-14-3a23-3a59.png)

1. Fare clic su **Modifica**.

   ![](assets/image2015-6-30-14-3a24-3a28.png)

1. Seleziona la casella di controllo **Visibile** relativa al campo da aggiungere alla sincronizzazione e fai clic su **Salva**.

   ![](assets/image2015-6-30-14-3a24-3a49.png)

   Dolce! Nel prossimo ciclo di sincronizzazione, Marketo vedrà il campo e avvierà la magia.

   >[!NOTE]
   >
   > Se nel campo sono già presenti valori in Salesforce, questi non si sincronizzano con Marketo fino al prossimo aggiornamento del record.
