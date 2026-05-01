---
unique-page-id: 4719306
description: Scopri come nascondere un campo Salesforce dalla sincronizzazione Marketo per ottimizzare le prestazioni. Utilizza la sicurezza a livello di campo nel profilo utente di sincronizzazione per escludere i campi non necessari.
title: Nascondere un campo Salesforce da Marketo Sync
exl-id: 5d7229f0-43b0-4232-93ed-a9ca52ace401
feature: Salesforce Integration
source-git-commit: f4ac42384a47d4b5e1ca139f1580ab475c58f543
workflow-type: tm+mt
source-wordcount: '166'
ht-degree: 10%

---

# Nascondi un campo [!DNL Salesforce] da Marketo Sync {#hide-a-salesforce-field-from-the-marketo-sync}

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

Non tutti i campi in Salesforce sono utili per il marketing. È possibile ottimizzare le prestazioni di sincronizzazione includendo solo i campi necessari. Ecco come nascondere un campo da Marketo Engage.

1. Fare clic sul menu del proprio nome e selezionare **[!UICONTROL Setup]**.

   ![](assets/image2015-6-30-15-3a11-3a23.png)

1. Immettere &quot;profiles&quot; nella barra di ricerca e fare clic su **[!UICONTROL Profiles]** in **[!UICONTROL Manage Users]**.

   ![](assets/image2015-6-30-15-3a12-3a46.png)

1. Fai clic sul profilo dell’utente di sincronizzazione.

   ![](assets/image2015-6-30-15-3a17-3a38.png)

1. Nella sezione **[!UICONTROL Field-Level Security]**, fare clic su **[!UICONTROL View]** accanto all&#39;oggetto che contiene il campo di destinazione.

   ![](assets/image2015-6-30-15-3a24-3a32.png)

1. Fai clic su **[!UICONTROL Edit]**.

   ![](assets/image2015-6-30-15-3a25-3a42.png)

1. Deselezionare la casella di controllo **[!UICONTROL Visible]** accanto al campo che si desidera nascondere. Fai clic su **[!UICONTROL Save]**.

   ![](assets/image2015-6-30-15-3a27-3a16.png)

   >[!NOTE]
   >
   >Se il campo nascosto in [!DNL Salesforce] è già stato sincronizzato con Marketo, è necessario nasconderlo anche in Marketo se non si desidera utilizzarlo.

   Questo campo non viene più visualizzato in Marketo al termine della sincronizzazione successiva.

   >[!MORELIKETHIS]
   >
   >[Nascondere e mostrare un campo](/help/marketo/product-docs/administration/field-management/hide-and-unhide-a-field.md){target="_blank"}
