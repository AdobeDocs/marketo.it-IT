---
unique-page-id: 12983390
description: Registrare un’app con Azure per acquisire l’ID client/ID app - Documenti Marketo - Documentazione del prodotto
title: Registra un’app con Azure per acquisire l’ID client/ID app
exl-id: 006cd130-a2fc-41ce-b5ee-890ef6167b34
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---

# Registra un&#39;app con Azure per acquisire il tuo ID client/ID app {#register-an-app-with-azure-to-acquire-your-client-id-app-id}

Azure Active Directory estende le directory locali nel cloud, fornendo il supporto per MS Dynamics 365 CRM con autenticazione ADFS on-premise.

## Registrazione di una nuova app {#registering-a-new-app}

1. [Accedi ](https://manage.windowsazure.com/) al portale di gestione di Microsoft Azure utilizzando un account con autorizzazioni di amministrazione. È inoltre possibile accedere al portale di Microsoft Azure tramite l&#39;Admin Center di Office 365 espandendo la voce **Admin** nel riquadro di navigazione a sinistra e selezionando **Azure AD**.

   >[!CAUTION]
   >
   >È necessario utilizzare un account nello stesso abbonamento a Office 365 di quello con cui si intende registrare l’app.

   >[!NOTE]
   >
   >Se non disponi di un account Azure, puoi [registrarti](https://azure.microsoft.com/en-us/free/) per uno. Per ulteriori informazioni, consulta la documentazione di Microsoft o rivolgiti al tuo rappresentante Microsoft. Dopo aver creato un account Azure, puoi registrare una o più app utilizzando la procedura descritta di seguito.
   >
   >
   >Se disponi di un account Azure ma la sottoscrizione di Office 365 con Microsoft Dynamics 365 non è disponibile nella sottoscrizione di Azure, segui [queste istruzioni](https://msdn.microsoft.com/office/office365/howto/setup-development-environment#bk_CreateAzureSubscription) per associare i due account.

1. Trova e fai clic su **Azure Active Directory** nel riquadro di navigazione a sinistra.

   ![](assets/two.png)

1. In Gestione, fai clic su **Registrazioni app**.

   ![](assets/three.png)

1. Fai clic su **Nuova registrazione** nella parte superiore della pagina.

   ![](assets/four.png)

1. Immetti un nome per la tua app, scegli il tipo di account applicabile e immetti un URL di reindirizzamento. Quindi fai clic su **Registra** in fondo alla pagina.

   ![](assets/five.png)

1. Ora dovresti visualizzare la tua app nella scheda **Registrazioni app** .

   ![](assets/six.png)

## Configurazione delle autorizzazioni dell&#39;app {#configuring-app-permissions}

1. Nella scheda **Registrazioni app** in Active Directory, fai clic sull’app per la quale desideri configurare le autorizzazioni.

   ![](assets/seven.png)

1. In Gestione, fai clic su **Autorizzazioni API**.

   ![](assets/eight.png)

1. Fai clic sul pulsante **Aggiungi un&#39;autorizzazione** .

   ![](assets/nine.png)

1. Scegli **Dynamics CRM**.

   ![](assets/ten.png)

1. Seleziona la casella **Accedi al servizio dati comune come utente dell&#39;organizzazione***s** , quindi fai clic su **Aggiungi autorizzazioni.**

   ![](assets/eleven.png)

1. Una volta aggiunte le autorizzazioni, attendi almeno 10 secondi.

   ![](assets/twelve.png)

1. Fai clic sul pulsante **Concedi consenso amministratore** .

   ![](assets/thirteen.png)

1. Fare clic su **Sì** per confermare.

   ![](assets/fourteen.png)

   E hai finito!

   ![](assets/fifteen.png)
