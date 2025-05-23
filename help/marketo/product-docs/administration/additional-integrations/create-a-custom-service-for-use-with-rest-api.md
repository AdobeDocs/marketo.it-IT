---
unique-page-id: 2360350
description: Creare un servizio personalizzato da utilizzare con API ReST - Documentazione di Marketo - Documentazione del prodotto
title: Creare un servizio personalizzato da utilizzare con API ReST
exl-id: d94f723b-2e98-4350-a9e5-bd57aff2303b
feature: Administration
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '207'
ht-degree: 0%

---

# Creare un servizio personalizzato da utilizzare con API ReST {#create-a-custom-service-for-use-with-rest-api}

Se desideri effettuare l’integrazione con Marketo tramite l’API ReST, dovrai creare un servizio personalizzato. Ecco come.

>[!PREREQUISITES]
>
>* [Crea un ruolo utente solo API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md)
>* [Crea un utente solo API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md)
>

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

>[!TIP]
>
>Consulta la documentazione per gli sviluppatori per informazioni dettagliate sull&#39;[API REST](https://developer.adobe.com/marketo-apis/). Abbiamo anche l&#39;[API SOAP](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/soap/soap-api), se questo è ciò che ti serve.

## Crea servizio personalizzato {#create-custom-service}

1. Vai all&#39;area **[!UICONTROL Amministratore]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-1.png)

1. Fare clic su **LaunchPoint**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-2.png)

1. Selezionare **[!UICONTROL Nuovo]** e quindi **[!UICONTROL Nuovo servizio]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-3.png)

1. Immetti un **[!UICONTROL Nome visualizzato]** per il servizio. Seleziona l&#39;**[!UICONTROL utente solo API]** [creato in precedenza](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md).

   ![](assets/create-a-custom-service-for-use-with-rest-api-4.png)

   >[!NOTE]
   >
   >Tieni presente che disponiamo già dell’integrazione nativa per i servizi dei webinar più diffusi.

1. Fai clic su **[!UICONTROL Crea]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-5.png)

   Oh, sì! Ora che il servizio è stato creato, procediamo e ottieni tutte le credenziali per fornire l’accesso.

## Credenziali per l’accesso API {#credentials-for-api-access}

1. Vai all&#39;area **[!UICONTROL Amministratore]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-6.png)

1. Fare clic su **[!UICONTROL LaunchPoint]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-7.png)

1. Fai clic su **[!UICONTROL Visualizza dettagli]** per il servizio [!UICONTROL LaunchPoint] personalizzato creato in precedenza.

   ![](assets/create-a-custom-service-for-use-with-rest-api-8.png)

1. Fai clic su **[!UICONTROL Ottieni token]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-9.png)

1. Fornisci **[!UICONTROL ID client]**, **[!UICONTROL Segreto client]**, **[!UICONTROL Utente autorizzato]** e **[!UICONTROL Token]** alla persona responsabile di stabilire la connessione.

   ![](assets/create-a-custom-service-for-use-with-rest-api-10.png)

>[!CAUTION]
>
>Non condividere queste informazioni, è la porta di accesso ai tuoi dati. Tienilo al sicuro!
