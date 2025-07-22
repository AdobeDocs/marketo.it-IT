---
unique-page-id: 4719306
description: Nascondere un campo Salesforce da Marketo Sync - Marketo Docs - Documentazione del prodotto
title: Nascondere un campo Salesforce da Marketo Sync
exl-id: 5d7229f0-43b0-4232-93ed-a9ca52ace401
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '155'
ht-degree: 2%

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

   Tutto qui. Questo campo non verrà più visualizzato in Marketo al termine della prossima sincronizzazione.

   >[!MORELIKETHIS]
   >
   >[Nascondi e scopri campo](/help/marketo/product-docs/administration/field-management/hide-and-unhide-a-field.md){target="_blank"}
