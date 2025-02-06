---
title: Documento Connect Experience Manager
description: Scopri come collegare i Cloud Service Adobe Experience Manager a Adobe Marketo Engage per sfruttare le risorse AEM.
source-git-commit: 92404e10771920862cd147c09e2ada37484e6118
workflow-type: tm+mt
source-wordcount: '224'
ht-degree: 0%

---

# Connetti Cloud Service Adobe Experience Manager {#connect-adobe-experience-manager-cloud-services}

Scopri come collegare l’account di Cloud Service AEM Assets all’istanza di Adobe Marketo Engage in modo da poter sfruttare l’archivio di risorse AEM nel Designer e-mail del Marketo Engage.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

1. In Marketo Engage, vai all&#39;area **Amministratore** e seleziona **Adobe Experience Manager** nella struttura di navigazione a sinistra.

   ![Seleziona Adobe Experience Manager nella sezione Amministratore](assets/connect-adobe-experience-manager-cloud-services-1.png){width="800"}

1. Fai clic su **Modifica** accanto a _Cloud Service Adobe Experience Manager_.

   ![Fare clic su MODIFICA](assets/connect-adobe-experience-manager-cloud-services-2.png){width="400"}

1. Seleziona uno o più archivi.

   ![Selezionare un repository](assets/connect-adobe-experience-manager-cloud-services-3.png){width="800"}

   >[!NOTE]
   >
   >Vengono elencati solo gli archivi associati alla stessa organizzazione IMS del tuo abbonamento di Marketo Engage.

1. Per configurare l&#39;archivio è necessario aggiungere un certificato di credenziali del servizio [](https://experienceleague.adobe.com/it/docs/experience-manager-learn/getting-started-with-aem-headless/authentication/service-credentials). Fare clic sul pulsante **+ Aggiungi certificato**.

   ![Aggiungi un certificato](assets/connect-adobe-experience-manager-cloud-services-4.png){width="800"}

1. Trascina e rilascia il certificato (solo file JSON) o selezionalo dal computer. Al termine, fai clic su **Aggiungi**.

   ![Individua il certificato nel computer](assets/connect-adobe-experience-manager-cloud-services-5.png){width="600"}

1. L’archivio configurato viene visualizzato di seguito insieme a stato e scadenza. Fare clic sul pulsante con i puntini di sospensione (**...**) per visualizzare il certificato. Altrimenti, hai finito.

   ![Certificato aggiunto](assets/connect-adobe-experience-manager-cloud-services-5.png){width="600"}

Ora tutte le immagini della libreria di gestione delle risorse digitali nell’archivio sono accessibili dal Designer e-mail di Marketo Engage.

>[!MORELIKETHIS]
>
>[Utilizzare risorse Experience Manager](/help/marketo/product-docs/email-marketing/email-designer/aem-assets.md)
