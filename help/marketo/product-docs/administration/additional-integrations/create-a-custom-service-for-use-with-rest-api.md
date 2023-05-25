---
unique-page-id: 2360350
description: Creare un servizio personalizzato da utilizzare con API ReST - Documentazione di Marketo - Documentazione del prodotto
title: Creare un servizio personalizzato da utilizzare con API ReST
exl-id: d94f723b-2e98-4350-a9e5-bd57aff2303b
source-git-commit: 1f10e1fcdbd5cf91481f749236fd37050ade29f8
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---

# Creare un servizio personalizzato da utilizzare con API ReST {#create-a-custom-service-for-use-with-rest-api}

Se desideri effettuare l’integrazione con Marketo tramite l’API ReST, dovrai creare un servizio personalizzato. Ecco come.

>[!PREREQUISITES]
>
>* [Creare un ruolo utente solo API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md)
>* [Creare un utente solo API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md)
>


>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

>[!TIP]
>
>Consulta la documentazione per gli sviluppatori per informazioni dettagliate su [API ReST](https://developers.marketo.com/documentation/rest/). Inoltre, è possibile [API SOAP](https://developers.marketo.com/documentation/soap/) se è quello che ti serve.

## Crea servizio personalizzato {#create-custom-service}

1. Vai a **[!UICONTROL Amministratore]** area.

   ![](assets/create-a-custom-service-for-use-with-rest-api-1.png)

1. Clic **LaunchPoint**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-2.png)

1. Seleziona **[!UICONTROL Nuovo]** e poi **[!UICONTROL Nuovo servizio]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-3.png)

1. Immetti un **[!UICONTROL Nome visualizzato]** per il servizio. Seleziona la **[!UICONTROL Utente solo API]** [creato in precedenza](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md).

   ![](assets/create-a-custom-service-for-use-with-rest-api-4.png)

   >[!NOTE]
   >
   >Tieni presente che disponiamo già dell’integrazione nativa per i servizi dei webinar più diffusi.

1. Fai clic su **[!UICONTROL Crea]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-5.png)

   Oh, sì! Ora che il servizio è stato creato, procediamo e ottieni tutte le credenziali per fornire l’accesso.

## Credenziali per l’accesso API {#credentials-for-api-access}

1. Vai a **[!UICONTROL Amministratore]** area.

   ![](assets/create-a-custom-service-for-use-with-rest-api-6.png)

1. Clic **[!UICONTROL LaunchPoint]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-7.png)

1. Clic **[!UICONTROL Visualizza dettagli]** per il personalizzato [!UICONTROL LaunchPoint] servizio creato in precedenza.

   ![](assets/create-a-custom-service-for-use-with-rest-api-8.png)

1. Clic **[!UICONTROL Ottieni token]**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-9.png)

1. Fornisci **[!UICONTROL ID client]**, **[!UICONTROL Segreto client]**, **[!UICONTROL Utente autorizzato]**, e **[!UICONTROL Token]** alla persona incaricata di stabilire il collegamento.

   ![](assets/create-a-custom-service-for-use-with-rest-api-10.png)

>[!CAUTION]
>
>Non condividere queste informazioni, è la porta di accesso ai tuoi dati. Tienilo al sicuro!
