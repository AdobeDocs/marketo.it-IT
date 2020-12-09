---
unique-page-id: 2360350
description: Creare un servizio personalizzato da utilizzare con l'API ReST - Marketo Docs - Documentazione prodotto
title: Creare un servizio personalizzato da utilizzare con l'API ReST
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---


# Creare un servizio personalizzato da utilizzare con l&#39;API ReST {#create-a-custom-service-for-use-with-rest-api}

Se desiderate integrare Marketo tramite l&#39;API ReST, desiderate creare un servizio personalizzato. Ecco come.

>[!PREREQUISITES]
>
>* [Creare un ruolo utente solo API](../../../product-docs/administration/users-and-roles/create-an-api-only-user-role.md)
>* [Creazione di un utente solo API](../../../product-docs/administration/users-and-roles/create-an-api-only-user.md)

>



>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

>[!NOTE]
>
>**Tubo profondo**
>
>Per informazioni dettagliate sull&#39;API [ReST, consulta la documentazione per gli sviluppatori](http://developers.marketo.com/documentation/rest/). Abbiamo anche l&#39;API [](http://developers.marketo.com/documentation/soap/) SOAP se questo è ciò di cui hai bisogno.

>[!NOTE]
>
>Non puoi creare un servizio personalizzato se hai il livello Spark di Marketo.

## Crea servizio personalizzato {#create-custom-service}

1. Vai ad **Admin** e fai clic su **LaunchPoint**.

   ![](assets/image2014-9-19-10-3a38-3a15.png)

1. In **Nuovo**, fate clic su **Nuovo servizio**.

   ![](assets/image2014-9-19-10-3a38-3a22.png)

1. Immettere un nome **** visualizzato per il servizio. Selezionate **API Only User** (Utente solo API) [creato](../../../product-docs/administration/users-and-roles/create-an-api-only-user.md)in precedenza.

   >[!NOTE]
   >
   >**Promemoria**
   >
   >È già disponibile l&#39;integrazione nativa per i servizi webinar più diffusi.

   ![](assets/image2014-9-19-10-3a38-3a32.png)

1. Fate clic su **Crea**.

   ![](assets/image2014-9-19-10-3a39-3a28.png)

   Oh si&#39;! Il servizio è stato creato, andiamo avanti e otteniamo tutte le credenziali per fornire l&#39;accesso.

## Credenziali per accesso API {#credentials-for-api-access}

1. Vai ad **Admin** e fai clic su **LaunchPoint**.

   ![](assets/image2014-9-19-10-3a42-3a11.png)

1. Fare clic su **Visualizza dettagli** per il servizio LaunchPoint personalizzato creato sopra.

   ![](assets/image2014-9-19-10-3a42-3a16.png)

1. Fate clic su **Ottieni token**.

   ![](assets/image2014-9-19-10-3a42-3a24.png)

1. Fornite l&#39;ID client***, il Segreto **** cliente, l&#39;Utente **** autorizzato e **il Token** alla persona incaricata di stabilire la connessione.

   ![](assets/image2014-9-19-10-3a42-3a38.png)

>[!CAUTION]
>
>Non condividere queste informazioni; è il backdoor dei tuoi dati. Tienila al sicuro!

