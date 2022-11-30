---
unique-page-id: 2360350
description: Creare un servizio personalizzato da utilizzare con l’API ReST - Marketo Docs - Documentazione del prodotto
title: Creare un servizio personalizzato da utilizzare con l’API ReST
exl-id: d94f723b-2e98-4350-a9e5-bd57aff2303b
source-git-commit: 5f509a7aa27692e54bf129b94c657aff0f645f2b
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 0%

---

# Creare un servizio personalizzato da utilizzare con l’API ReST {#create-a-custom-service-for-use-with-rest-api}

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
>Consulta la documentazione per i nostri sviluppatori per i dettagli sul [API ReST](https://developers.marketo.com/documentation/rest/). Abbiamo anche [API SOAP](https://developers.marketo.com/documentation/soap/) se è quello di cui hai bisogno.

## Crea servizio personalizzato {#create-custom-service}

1. Vai a **Amministratore** area.

   ![](assets/create-a-custom-service-for-use-with-rest-api-1.png)

1. Fai clic su **LaunchPoint**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-2.png)

1. Seleziona **Nuovo** e poi **Nuovo servizio**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-3.png)

1. Inserisci un **Nome visualizzato** per il servizio. Seleziona la **Utente solo API** [creato in precedenza](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md).

   ![](assets/create-a-custom-service-for-use-with-rest-api-4.png)

   >[!NOTE]
   >
   >Tieni presente che disponiamo già di un’integrazione nativa per i servizi webinar più popolari.

1. Fai clic su **Crea**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-5.png)

   Oh sì! Il servizio è stato creato, andiamo avanti e otteniamo tutte le credenziali per fornire l&#39;accesso.

## Credenziali per l&#39;accesso API {#credentials-for-api-access}

1. Vai a **Amministratore** area.

   ![](assets/create-a-custom-service-for-use-with-rest-api-6.png)

1. Fai clic su **LaunchPoint**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-7.png)

1. Fai clic su **Visualizza dettagli** per il servizio LaunchPoint personalizzato creato in precedenza.

   ![](assets/create-a-custom-service-for-use-with-rest-api-8.png)

1. Fai clic su **Ottieni token**.

   ![](assets/create-a-custom-service-for-use-with-rest-api-9.png)

1. Fornisci **ID client**, **Segreto client**, **Utente autorizzato** e **Token** alla persona incaricata di stabilire il collegamento.

   ![](assets/create-a-custom-service-for-use-with-rest-api-10.png)

>[!CAUTION]
>
>Non condividere queste informazioni; è il backdoor dei vostri dati. La tenga al sicuro!
