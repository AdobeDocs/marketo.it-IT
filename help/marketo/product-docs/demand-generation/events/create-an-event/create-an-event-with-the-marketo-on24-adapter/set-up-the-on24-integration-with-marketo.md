---
description: Configurare l'integrazione ON24 con Marketo - Documentazione Marketo - Documentazione del prodotto
title: Configurare l’integrazione ON24 con Marketo
exl-id: 395ffa37-b87d-4eb4-bf9f-72aa96dc819c
feature: Events
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 8%

---

# Configurare l’integrazione ON24 con Marketo{#set-up-the-on24-integration-with-marketo}

Ecco come configurare l’integrazione dell’evento ON24.

## Creare un ruolo solo API {#create-an-api-only-role}

1. Da Il mio Marketo, fare clic su **[!UICONTROL Admin]**.

   ![](assets/set-up-the-on24-integration-with-marketo-1.png)

1. In [!UICONTROL Security], fare clic su **[!UICONTROL Users & Roles]**.

   ![](assets/set-up-the-on24-integration-with-marketo-2.png)

1. Fare clic sulla scheda **[!UICONTROL Roles]** e quindi su **[!UICONTROL New Role]**.

   ![](assets/set-up-the-on24-integration-with-marketo-3.png)

1. Immetti [!UICONTROL Role Name]. Aprire il menu **[!UICONTROL Access API]** e selezionare &quot;[!UICONTROL Read-Write Custom Object]&quot; e &quot;[!UICONTROL Read-Write Person]&quot;.&quot; Fai clic su **[!UICONTROL Create]**.

   ![](assets/set-up-the-on24-integration-with-marketo-4.png)

## Crea un nuovo utente {#create-a-new-user}

1. Sempre in [!UICONTROL Users & Roles], fare clic sulla scheda **[!UICONTROL Users]** e quindi su **[!UICONTROL Invite New User]**.

   ![](assets/set-up-the-on24-integration-with-marketo-5.png)

1. Immettere le informazioni del nuovo utente e fare clic su **[!UICONTROL Next]**.

   ![](assets/set-up-the-on24-integration-with-marketo-6.png)

1. Seleziona [!UICONTROL ON24 API Only Role (all workspaces)] appena creato. Selezionare la casella di controllo **[!UICONTROL API Only]**. Fai clic su **[!UICONTROL Next]**.

   ![](assets/set-up-the-on24-integration-with-marketo-7.png)

1. Fai clic su **[!UICONTROL Send]**.

   ![](assets/set-up-the-on24-integration-with-marketo-8.png)

>[!NOTE]
>
>Non è necessario un invito per gli utenti solo API.

## Configura connessione ON24 {#set-up-on24-connection}

1. Sempre nella sezione [!UICONTROL Admin], fare clic su **[!UICONTROL LaunchPoint]**.

   ![](assets/set-up-the-on24-integration-with-marketo-9.png)

1. Fare clic su **[!UICONTROL New]** e quindi su **[!UICONTROL New Service]**.

   ![](assets/set-up-the-on24-integration-with-marketo-10.png)

1. Scegli un [!UICONTROL display name]. Fare clic sul menu a discesa **[!UICONTROL Service]** e selezionare **[!UICONTROL Custom]**. Immetti [!UICONTROL description]. Fai clic sul menu a discesa [!UICONTROL API Only User] e seleziona l&#39;utente che hai creato [&#x200B; nei passaggi precedenti](#create-a-new-user). Fai clic su **[!UICONTROL Create]**.

   ![](assets/set-up-the-on24-integration-with-marketo-11.png)

1. Trovare il servizio [!DNL LaunchPoint] personalizzato appena creato e fare clic su [!UICONTROL View Details].

   ![](assets/set-up-the-on24-integration-with-marketo-12.png)

1. Evidenziare, fare clic con il pulsante destro del mouse, copiare e salvare [!UICONTROL Client ID] (sarà necessario in seguito). Ripeti per [!UICONTROL Client Secret].

   ![](assets/set-up-the-on24-integration-with-marketo-13.png)

1. Nell&#39;albero a sinistra fare clic su **[!UICONTROL Web Services]**.

   ![](assets/set-up-the-on24-integration-with-marketo-14.png)

1. In &quot;[!UICONTROL REST API],&quot; evidenziare, fare clic con il pulsante destro del mouse, copiare e salvare la prima parte di [!UICONTROL Identity] (fino alla &#39;m&#39; in .com).

   ![](assets/set-up-the-on24-integration-with-marketo-15.png)

1. Con l&#39;ID client, il segreto client e l&#39;identità salvati, accedi all&#39;account ON24. I passaggi rimanenti vengono eseguiti qui ed è possibile trovarli nella [documentazione ON24](https://support.on24.com/hc/en-us/articles/21420762650523-Data-Integration-Setup-Instructions-When-Using-Marketo-Registration-Option-1){target="_blank"}.
