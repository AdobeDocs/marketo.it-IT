---
unique-page-id: 4719308
description: Aggiungere un campo Salesforce esistente a Sincronizzazione Marketo - Documenti Marketo - Documentazione del prodotto
title: Aggiungere un campo Salesforce esistente alla sincronizzazione Marketo
exl-id: 6030aedd-9c4b-411f-89c7-f35fd39b0066
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '146'
ht-degree: 6%

---

# Aggiungi un campo [!DNL Salesforce] esistente a Marketo Sync {#add-an-existing-salesforce-field-to-the-marketo-sync}

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

In genere, i nuovi campi personalizzati in Salesforce vengono sincronizzati automaticamente con Marketo Engage. In caso contrario, i campi potrebbero non essere visibili all&#39;utente di Marketo Sync. Ecco come si può risolvere il problema.

1. Fai clic sul tuo nome e seleziona **[!UICONTROL Setup]**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-1.png)

1. Immettere &quot;profile&quot; nella barra di ricerca a sinistra e fare clic su **[!UICONTROL Profiles]** in **[!UICONTROL Manage Users]**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-2.png)

1. Fai clic sul profilo dell’utente di sincronizzazione.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-3.png)

1. Nella sezione **[!UICONTROL Field-Level Security]**, fai clic su **[!UICONTROL View]** accanto all&#39;oggetto che contiene il campo.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-4.png)

1. Fai clic su **[!UICONTROL Edit]**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-5.png)

1. Selezionare la casella di controllo **[!UICONTROL Visible]** per il campo da aggiungere alla sincronizzazione e fare clic su **[!UICONTROL Save]**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-6.png)

   Al prossimo ciclo di sincronizzazione, Marketo visualizzerà il campo e avvierà la magia.

   >[!NOTE]
   >
   > Se il campo contiene già valori in [!DNL Salesforce], questi non verranno sincronizzati con Marketo fino al successivo aggiornamento del record.
