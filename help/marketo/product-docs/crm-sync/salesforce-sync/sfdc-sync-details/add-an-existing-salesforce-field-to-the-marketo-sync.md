---
unique-page-id: 4719308
description: Aggiungere un campo Salesforce esistente a Marketo Sync - Marketo Docs - Documentazione del prodotto
title: Aggiungi un campo Salesforce esistente a Marketo Sync
exl-id: 6030aedd-9c4b-411f-89c7-f35fd39b0066
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 0%

---

# Aggiungi un campo Salesforce esistente a Marketo Sync {#add-an-existing-salesforce-field-to-the-marketo-sync}

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

In genere, i nuovi campi personalizzati in Salesforce vengono sincronizzati automaticamente con il Marketo Engage. In caso contrario, i campi potrebbero non essere visibili all&#39;utente di Marketo Sync. Ecco come si può risolvere il problema.

1. Fai clic sul tuo nome e seleziona **[!UICONTROL Configurazione]**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-1.png)

1. Immetti &quot;profile&quot; nella barra di ricerca a sinistra e fai clic su **[!UICONTROL Profiles]** in **[!UICONTROL Manage Users]**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-2.png)

1. Fai clic sul profilo dell’utente di sincronizzazione.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-3.png)

1. Nella sezione **[!UICONTROL Sicurezza a livello di campo]**, fai clic su **[!UICONTROL Visualizza]** accanto all&#39;oggetto che contiene il campo.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-4.png)

1. Fai clic su **[!UICONTROL Modifica]**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-5.png)

1. Selezionare la casella di controllo **[!UICONTROL Visibile]** per il campo che si desidera aggiungere alla sincronizzazione e fare clic su **[!UICONTROL Salva]**.

   ![](assets/add-an-existing-salesforce-field-to-the-marketo-sync-6.png)

   Al prossimo ciclo di sincronizzazione, Marketo visualizzerà il campo e avvierà la magia.

   >[!NOTE]
   >
   > Se il campo contiene già dei valori in Salesforce, questi non vengono sincronizzati con Marketo fino al successivo aggiornamento del record.
