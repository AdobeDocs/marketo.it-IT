---
unique-page-id: 12983390
description: Registrazione di un'app con Azure per acquisire l'ID client/ID app - Documenti Marketo - Documentazione prodotto
title: Registrazione di un'app con Azure per acquisire l'ID client/app
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---


# Registrazione di un&#39;app con Azure per acquisire l&#39;ID client/app {#register-an-app-with-azure-to-acquire-your-client-id-app-id}

Azure Active Directory estende le directory locali nel cloud, fornendo supporto per MS Dynamics 365 CRM con autenticazione ADFS locale.

## Registrazione di una nuova app {#registering-a-new-app}

1. [Accedere ](https://manage.windowsazure.com/) al portale di gestione di Microsoft Azure utilizzando un account con autorizzazioni di amministratore. È inoltre possibile accedere al portale di Microsoft Azure tramite l&#39;Admin Center di Office 365 espandendo l&#39;elemento **Admin** nel riquadro di navigazione a sinistra e selezionando **Azure AD**.

   >[!CAUTION]
   >
   >Dovete utilizzare un account nella stessa iscrizione a Office 365 con cui desiderate registrare l&#39;app.

   >[!NOTE]
   >
   >Se non disponete di un account Azure, potete [registrarvi](https://azure.microsoft.com/en-us/free/) per uno. Per ulteriori informazioni, consulta la documentazione di Microsoft o rivolgiti al rappresentante Microsoft. Dopo aver creato un account Azure, è possibile registrare una o più app utilizzando la procedura descritta di seguito.
   >
   >
   >Se si dispone di un account Azure ma la sottoscrizione di Office 365 con Microsoft Dynamics 365 non è disponibile nella sottoscrizione di Azure, seguire [le istruzioni ](https://msdn.microsoft.com/office/office365/howto/setup-development-environment#bk_CreateAzureSubscription) per associare i due account.

1. Trovare e fare clic su **Azure Active Directory** nel riquadro di navigazione a sinistra.

   ![](assets/two.png)

1. In Gestisci, fai clic su **Registrazioni app**.

   ![](assets/three.png)

1. Fare clic su **Nuova registrazione** nella parte superiore della pagina.

   ![](assets/four.png)

1. Immettete un nome per l&#39;app, scegliete il tipo di account appropriato e immettete un URL di reindirizzamento. Fate clic su **Register** nella parte inferiore della pagina.

   ![](assets/five.png)

1. Dovresti ora visualizzare l&#39;app nella scheda **Registrazioni app**.

   ![](assets/six.png)

## Configurazione delle autorizzazioni dell&#39;app {#configuring-app-permissions}

1. Nella scheda **Registrazioni app** in Active Directory, fai clic sull&#39;app per la quale vuoi configurare le autorizzazioni.

   ![](assets/seven.png)

1. In Gestisci, fai clic su **Autorizzazioni API**.

   ![](assets/eight.png)

1. Fare clic sul pulsante **Aggiungi un&#39;autorizzazione**.

   ![](assets/nine.png)

1. Scegliere **Dynamics CRM**.

   ![](assets/ten.png)

1. Selezionare la casella **Accedi al servizio dati comune come utente organizzazione****s**, quindi fare clic su **Aggiungi autorizzazioni.**

   ![](assets/eleven.png)

1. Dopo aver aggiunto le autorizzazioni, attendete almeno 10 secondi.

   ![](assets/twelve.png)

1. Fare clic sul pulsante **Concedi consenso amministratore**.

   ![](assets/thirteen.png)

1. Fare clic su **Sì** per confermare.

   ![](assets/fourteen.png)

   E hai finito!

   ![](assets/fifteen.png)

