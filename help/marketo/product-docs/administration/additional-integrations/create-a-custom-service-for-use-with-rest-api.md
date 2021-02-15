---
unique-page-id: 2360350
description: Creare un servizio personalizzato da utilizzare con l'API ReST - Marketo Docs - Documentazione prodotto
title: Creare un servizio personalizzato da utilizzare con l'API ReST
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '224'
ht-degree: 0%

---


# Creare un servizio personalizzato da utilizzare con l&#39;API ReST {#create-a-custom-service-for-use-with-rest-api}

Se desiderate integrare Marketo tramite l&#39;API ReST, desiderate creare un servizio personalizzato. Ecco come.

>[!PREREQUISITES]
>
>* [Creare un ruolo utente solo API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md)
>* [Creazione di un utente solo API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md)

>



>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

>[!TIP]
>
>Consulta la documentazione per gli sviluppatori per informazioni su [ReST API](https://developers.marketo.com/documentation/rest/). Abbiamo anche l&#39; [SOAP API](https://developers.marketo.com/documentation/soap/) se questo è ciò che ti serve.

>[!NOTE]
>
>Non puoi creare un servizio personalizzato se hai il livello Spark di Marketo.

## Crea servizio personalizzato {#create-custom-service}

1. Accedete a **Admin** e fate clic su **LaunchPoint**.

   ![](assets/image2014-9-19-10-3a38-3a15.png)

1. In **New**, fare clic su **New Service**.

   ![](assets/image2014-9-19-10-3a38-3a22.png)

1. Immettere un **nome visualizzato** per il servizio. Selezionare l&#39; **API Only User** [creato in precedenza](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md).

   >[!NOTE]
   >
   >È già disponibile l&#39;integrazione nativa per i servizi webinar più diffusi.

   ![](assets/image2014-9-19-10-3a38-3a32.png)

1. Fare clic su **Crea**.

   ![](assets/image2014-9-19-10-3a39-3a28.png)

   Oh si&#39;! Il servizio è stato creato, andiamo avanti e otteniamo tutte le credenziali per fornire l&#39;accesso.

## Credenziali per accesso API {#credentials-for-api-access}

1. Accedete a **Admin** e fate clic su **LaunchPoint**.

   ![](assets/image2014-9-19-10-3a42-3a11.png)

1. Fare clic su **Visualizza dettagli** per il servizio LaunchPoint personalizzato creato sopra.

   ![](assets/image2014-9-19-10-3a42-3a16.png)

1. Fare clic su **Ottieni token**.

   ![](assets/image2014-9-19-10-3a42-3a24.png)

1. Fornire l&#39; **ID client**, **Segreto client**, **Utente autorizzato** e **Token** alla persona incaricata di stabilire la connessione.

   ![](assets/image2014-9-19-10-3a42-3a38.png)

>[!CAUTION]
>
>Non condividere queste informazioni; è il backdoor dei tuoi dati. Tienila al sicuro!
