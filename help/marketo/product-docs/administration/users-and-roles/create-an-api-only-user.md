---
unique-page-id: 2360207
description: Creazione di un utente solo API - Documentazione di Marketo - Documentazione del prodotto
title: Creare un utente solo API
exl-id: 23c92255-07a8-41c2-b7b8-8e495d135671
feature: Users and Roles
source-git-commit: ab1ea483998d6cb37277b18adf2c1d3371bb40e6
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---

# Creare un utente solo API {#create-an-api-only-user}

Se desideri effettuare l’integrazione con Marketo tramite [API REST](https://developers.marketo.com/documentation/rest/){target="_blank"}, sarà necessario creare un utente solo API. Ecco come.

>[!IMPORTANT]
>
>Se crei solo utenti API in una sottoscrizione a cui è stato effettuato l’onboarding in Adobe Identity, i passaggi sono diversi e [si trova qui](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-api-only-user-for-adobe-ims-enabled-subscriptions.md){target="_blank"}.

>[!PREREQUISITES]
>
>[Creare un ruolo utente solo API](/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md){target="_blank"}

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

1. Vai a **[!UICONTROL Amministratore]** area.

   ![](assets/create-an-api-only-user-1.png)

1. Clic **[!UICONTROL Utenti e ruoli]**.

   ![](assets/create-an-api-only-user-2.png)

1. Clic **[!UICONTROL Invita nuovo utente]**.

   ![](assets/create-an-api-only-user-3.png)

1. Immetti e-mail, nome e cognome per l’utente API. Clic **[!UICONTROL Successivo]**.

   ![](assets/create-an-api-only-user-4.png)

   >[!TIP]
   >
   >Aggiungi un motivo facoltativo o una data di scadenza dell’accesso. Le date di scadenza dell’accesso sono utili per i dipendenti a breve termine.

1. Seleziona la **[!UICONTROL Solo API]** ruolo e verifica **[!UICONTROL Solo API]** casella di controllo. Clic **[!UICONTROL Successivo]**.

   ![](assets/create-an-api-only-user-5.png)

1. Clic **[!UICONTROL Invia]**.

   ![](assets/create-an-api-only-user-6.png)

>[!NOTE]
>
>Il pop-up dice, &quot;Un invito non è richiesto solo per API,&quot; ma questo non significa che hai fatto qualcosa di sbagliato. Significa semplicemente che creeremo il ruolo senza dover inviare un’e-mail di invito.

Bene, allora! Ora procediamo e creiamo il servizio personalizzato.

>[!MORELIKETHIS]
>
>[Creare un servizio personalizzato da utilizzare con l’API REST](/help/marketo/product-docs/administration/additional-integrations/create-a-custom-service-for-use-with-rest-api.md){target="_blank"}
