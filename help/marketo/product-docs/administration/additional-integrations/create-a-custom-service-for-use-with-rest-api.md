---
unique-page-id: 2360350
description: Creare un servizio personalizzato da utilizzare con l’API ReST - Marketo Docs - Documentazione del prodotto
title: Creare un servizio personalizzato da utilizzare con l’API ReST
exl-id: d94f723b-2e98-4350-a9e5-bd57aff2303b
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '224'
ht-degree: 0%

---

# Creare un servizio personalizzato da utilizzare con l&#39;API ReST {#create-a-custom-service-for-use-with-rest-api}

Se desideri integrare con Marketo tramite l’API ReST, crea un servizio personalizzato. Ecco come.

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
>Per informazioni dettagliate sull&#39; [API ReST](https://developers.marketo.com/documentation/rest/), consulta la documentazione per gli sviluppatori. Disponiamo anche dell’ [API SOAP](https://developers.marketo.com/documentation/soap/) se questo è ciò di cui hai bisogno.

>[!NOTE]
>
>Non puoi creare un servizio personalizzato se disponi del livello Spark di Marketo.

## Crea servizio personalizzato {#create-custom-service}

1. Vai a **Amministratore** e fai clic su **LaunchPoint**.

   ![](assets/image2014-9-19-10-3a38-3a15.png)

1. In **Nuovo**, fai clic su **Nuovo servizio**.

   ![](assets/image2014-9-19-10-3a38-3a22.png)

1. Immetti un **Nome visualizzato** per il servizio. Seleziona il **Solo API utente** [creato in precedenza](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md).

   >[!NOTE]
   >
   >Tieni presente che disponiamo già di un’integrazione nativa per i servizi webinar più popolari.

   ![](assets/image2014-9-19-10-3a38-3a32.png)

1. Fare clic su **Crea**.

   ![](assets/image2014-9-19-10-3a39-3a28.png)

   Oh sì! Il servizio è stato creato, andiamo avanti e otteniamo tutte le credenziali per fornire l&#39;accesso.

## Credenziali per l&#39;accesso API {#credentials-for-api-access}

1. Vai a **Amministratore** e fai clic su **LaunchPoint**.

   ![](assets/image2014-9-19-10-3a42-3a11.png)

1. Fai clic su **Visualizza dettagli** per il servizio LaunchPoint personalizzato creato sopra.

   ![](assets/image2014-9-19-10-3a42-3a16.png)

1. Fai clic su **Ottieni token**.

   ![](assets/image2014-9-19-10-3a42-3a24.png)

1. Fornisci il **ID client**, **Segreto client**, **Utente autorizzato** e **Token** alla persona incaricata di stabilire la connessione.

   ![](assets/image2014-9-19-10-3a42-3a38.png)

>[!CAUTION]
>
>Non condividere queste informazioni; è il backdoor dei vostri dati. La tenga al sicuro!
