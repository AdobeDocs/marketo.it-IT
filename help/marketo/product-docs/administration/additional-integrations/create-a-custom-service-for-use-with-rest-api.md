---
unique-page-id: 2360350
description: Crea un servizio LaunchPoint personalizzato collegato a un utente solo API per l’integrazione con API ReST.
title: Creare un servizio personalizzato da utilizzare con API ReST
exl-id: d94f723b-2e98-4350-a9e5-bd57aff2303b
feature: Administration
source-git-commit: 40f06a5391f2f7263bea0c5b8cefc1f3a607c68c
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 24%

---

# Creare un servizio personalizzato da utilizzare con API ReST {#create-a-custom-service-for-use-with-rest-api}

Se desideri effettuare l’integrazione con Marketo tramite l’API ReST, crea un servizio personalizzato.

>[!PREREQUISITES]
>
>* [Crea un ruolo utente solo API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md)
>* [Crea un utente solo API](/help/marketo/product-docs/administration/users-and-roles/create-api-only-user.md)
>

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

>[!TIP]
>
>Per informazioni dettagliate sull&#39;[API REST](https://developer.adobe.com/marketo-apis/), consulta la documentazione per gli sviluppatori.

## Crea servizio personalizzato {#create-custom-service}

1. Passa alla schermata **[!UICONTROL Admin]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-1.png)

1. Fai clic su **[!UICONTROL LaunchPoint]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-2.png)

1. Selezionare **[!UICONTROL New]** e quindi **[!UICONTROL New Service]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-3.png)

1. Immettere **[!UICONTROL Display Name]** per il servizio. Seleziona **[!UICONTROL API Only User]** [creato in precedenza](/help/marketo/product-docs/administration/users-and-roles/create-api-only-user.md).

   ![](assets/create-a-custom-service-for-use-with-rest-api-4.png)

1. Fai clic su **[!UICONTROL Create]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-5.png)

   Il servizio è stato creato. Recupera le credenziali da fornire per l’accesso.

## Credenziali per l’accesso API {#credentials-for-api-access}

1. Passa alla schermata **[!UICONTROL Admin]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-6.png)

1. Fai clic su **[!UICONTROL LaunchPoint]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-7.png)

1. Fare clic su **[!UICONTROL View Details]** per il servizio [!UICONTROL LaunchPoint] personalizzato creato in precedenza.

   ![](assets/create-a-custom-service-for-use-with-rest-api-8.png)

1. Fai clic su **[!UICONTROL Get Token]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-9.png)

1. Fornisci **[!UICONTROL Client Id]**, **[!UICONTROL Client Secret]**, **[!UICONTROL Authorized User]** e **[!UICONTROL Token]** alla persona responsabile di stabilire la connessione.

   ![](assets/create-a-custom-service-for-use-with-rest-api-10.png)

>[!CAUTION]
>
>Non condividere queste informazioni, poiché consentono di accedere ai dati.
