---
unique-page-id: 12983390
description: Registrare un'app con Azure per acquisire l'ID client/ID app - Documentazione di Marketo - Documentazione del prodotto
title: Registrare un’app con Azure per acquisire l’ID client/ID app
exl-id: 006cd130-a2fc-41ce-b5ee-890ef6167b34
feature: Microsoft Dynamics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 8%

---

# Registrare un’app con Azure per acquisire l’ID client/ID app {#register-an-app-with-azure-to-acquire-your-client-id-app-id}

Azure Active Directory estende le directory locali nel cloud, fornendo il supporto per il CRM [!DNL MS Dynamics 365] con l&#39;autenticazione ADFS locale.

## Registrazione di una nuova app {#registering-a-new-app}

1. [Accedi](https://login.microsoftonline.com/){target="_blank"} al portale di gestione di Microsoft Azure utilizzando un account con autorizzazioni di amministratore. È inoltre possibile accedere al portale di Microsoft Azure tramite l&#39;Admin Center di Office 365 espandendo l&#39;elemento **[!UICONTROL Admin]** nel riquadro di spostamento a sinistra e selezionando **[!UICONTROL Azure AD]**.

   >[!CAUTION]
   >
   >È necessario utilizzare un account nello stesso abbonamento [!DNL Office 365] di quello con cui si intende registrare l&#39;app.

   >[!NOTE]
   >
   >Se non disponi di un account di Azure, puoi [iscriverti](https://azure.microsoft.com/en-us/free/){target="_blank"} per un account. Per ulteriori informazioni, consulta la documentazione di Microsoft o rivolgiti al tuo rappresentante Microsoft. Dopo aver creato un account di Azure, è possibile registrare una o più app utilizzando la procedura descritta di seguito.
   >
   >
   >Se disponi di un account di Azure ma la sottoscrizione di [!DNL Office 365] con [!DNL Microsoft Dynamics 365] non è disponibile nella sottoscrizione di Azure, segui [queste istruzioni](https://msdn.microsoft.com/office/office365/howto/setup-development-environment#bk_CreateAzureSubscription){target="_blank"} per associare i due account.

1. Trovare e fare clic su **[!UICONTROL Azure Active Directory]** nel riquadro di spostamento a sinistra.

   ![](assets/two.png)

1. In [!UICONTROL Manage], fare clic su **[!UICONTROL App registrations]**.

   ![](assets/three.png)

1. Fai clic su **[!UICONTROL New registration]** nella parte superiore della pagina.

   ![](assets/four.png)

1. Immetti un nome per l&#39;app, scegli il tipo di account applicabile e immetti un URL di reindirizzamento. Quindi fare clic su **[!UICONTROL Register]** nella parte inferiore della pagina.

   ![](assets/five.png)

1. Ora dovresti visualizzare l&#39;app nella scheda **[!UICONTROL App registrations]**.

   ![](assets/six.png)

## Configurazione delle autorizzazioni dell’app {#configuring-app-permissions}

1. Nella scheda **[!UICONTROL App registrations]** di Active Directory fare clic sull&#39;app per la quale si desidera configurare le autorizzazioni.

   ![](assets/seven.png)

1. In [!UICONTROL Manage], fare clic su **[!UICONTROL API permissions]**.

   ![](assets/eight.png)

1. Fare clic sul pulsante **[!UICONTROL Add a permission]**.

   ![](assets/nine.png)

1. Scegli **[!UICONTROL Dynamics CRM]**.

   ![](assets/ten.png)

1. Selezionare la casella **[!UICONTROL Access Common Data Service as organization users]**, quindi fare clic su **[!UICONTROL Add permissions].**

   ![](assets/eleven.png)

1. Una volta aggiunte correttamente le autorizzazioni, attendi almeno 10 secondi.

   ![](assets/twelve.png)

1. Fare clic sul pulsante **[!UICONTROL Grant admin consent]**.

   ![](assets/thirteen.png)

1. Fai clic su **[!UICONTROL Yes]** per confermare.

   ![](assets/fourteen.png)

   E hai finito!

   ![](assets/fifteen.png)
