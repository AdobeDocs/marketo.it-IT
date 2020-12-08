---
unique-page-id: 4719308
description: Aggiungere un campo Salesforce esistente alla sincronizzazione Marketo - Marketo Docs - Documentazione prodotto
title: Aggiungere un campo Salesforce esistente alla sincronizzazione Marketo
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---


# Aggiungere un campo Salesforce esistente alla sincronizzazione Marketo {#add-an-existing-salesforce-field-to-the-marketo-sync}

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

Solitamente, i nuovi campi personalizzati in Salesforce si sincronizzano automaticamente su Marketo. In caso contrario, i campi potrebbero non essere visibili all’utente di Marketing Cloud Sync. Ecco come si può riparare questo.

1. Fate clic sul vostro nome e selezionate **Configurazione**.

   ![](assets/image2015-6-30-14-3a20-3a6.png)

1. Immettete il **profilo** nella barra di ricerca a sinistra e fate clic su **Profili** in **Gestisci utenti**.

   ![](assets/image2015-6-30-14-3a20-3a52.png)

1. Fate clic sul profilo dell&#39;utente per la sincronizzazione.

   ![](assets/image2015-6-30-14-3a23-3a41.png)

1. Nella sezione Protezione **a livello di** campo fare clic su **Visualizza** accanto all&#39;oggetto che contiene il campo.

   ![](assets/image2015-6-30-14-3a23-3a59.png)

1. Fate clic su **Modifica**.

   ![](assets/image2015-6-30-14-3a24-3a28.png)

1. Selezionate la casella **Visibile** per il campo da aggiungere alla sincronizzazione e fate clic su **Salva**.

   ![](assets/image2015-6-30-14-3a24-3a49.png)

   Dolce! Nel prossimo ciclo di sincronizzazione, Marketo vedrà il campo e inizierà la magia.

   >[!NOTE]
   >
   > Se nel campo sono già presenti valori in Salesforce, questi valori non si sincronizzano su Marketo fino al successivo aggiornamento del record.

