---
unique-page-id: 4719308
description: Aggiungere un campo Salesforce esistente alla sincronizzazione Marketo - Marketo Docs - Documentazione prodotto
title: Aggiungere un campo Salesforce esistente alla sincronizzazione Marketo
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---


# Aggiungi un campo Salesforce esistente alla sincronizzazione di Marketo {#add-an-existing-salesforce-field-to-the-marketo-sync}

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

Solitamente, i nuovi campi personalizzati in Salesforce si sincronizzano automaticamente su Marketo. In caso contrario, i campi potrebbero non essere visibili all’utente di Marketing Cloud Sync. Ecco come si può riparare questo.

1. Fate clic sul vostro nome, quindi selezionate **Setup**.

   ![](assets/image2015-6-30-14-3a20-3a6.png)

1. Immettere **profile** nella barra di ricerca a sinistra e fare clic su **Profili** in **Gestisci utenti**.

   ![](assets/image2015-6-30-14-3a20-3a52.png)

1. Fate clic sul profilo dell&#39;utente per la sincronizzazione.

   ![](assets/image2015-6-30-14-3a23-3a41.png)

1. Nella sezione **Sicurezza a livello di campo**, fare clic su **Visualizza** accanto all&#39;oggetto che contiene il campo.

   ![](assets/image2015-6-30-14-3a23-3a59.png)

1. Fare clic su **Modifica**.

   ![](assets/image2015-6-30-14-3a24-3a28.png)

1. Selezionare la casella **Visible** per il campo da aggiungere alla sincronizzazione e fare clic su **Save**.

   ![](assets/image2015-6-30-14-3a24-3a49.png)

   Dolce! Nel prossimo ciclo di sincronizzazione, Marketo vedrà il campo e inizierà la magia.

   >[!NOTE]
   >
   > Se nel campo sono già presenti valori in Salesforce, questi valori non si sincronizzano su Marketo fino al successivo aggiornamento del record.
