---
description: Installare Marketo per Microsoft Dynamics 2016/Dynamics 365 On-Premises 1 di 3 - Documentazione Marketo - Documentazione del prodotto
title: Installazione di Marketo per Microsoft Dynamics 2016/Dynamics 365 on-premises Passaggio 1 di 3
exl-id: 0a494ae7-87da-4ff9-bb47-990b957533e1
feature: Microsoft Dynamics
source-git-commit: e3f61755dccd9bea1378a429fc428b440fc3ecb4
workflow-type: tm+mt
source-wordcount: '286'
ht-degree: 0%

---

# Passaggio 1 di 3: configurare l’utente Sync per Marketo (on-prem /Dynamics 365 on-premise 2016) {#step-of-configure-sync-user-for-marketo-on-premises-2016}

Prima di poter sincronizzare Microsoft Dynamics 2016 On-Prem/Dynamics 365 con Marketo Engage, è necessario installare la soluzione Marketo in Dynamics.

>[!NOTE]
>
>Dopo aver sincronizzato Marketo con un CRM, non è possibile sincronizzare un nuovo CRM con l&#39;istanza Marketo esistente.

>[!PREREQUISITES]
>
>Se si utilizza Microsoft Dynamics On-Premise, è necessario che sia configurato [Internet Facing Deployment](https://learn.microsoft.com/en-us/dynamics365/customerengagement/on-premises/deploy/configure-an-internet-facing-deployment){target="_blank"} (IFD) con [Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"} 2.0+ (ADFS). Nota: il documento IFD viene scaricato automaticamente quando si fa clic sul collegamento.
>
>[Scaricare la soluzione Marketo per la gestione dei lead](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"} prima di iniziare.

>[!NOTE]
>
>**Autorizzazioni amministratore Dynamics richieste**.
>
>Per eseguire questa sincronizzazione sono necessari privilegi di amministratore CRM.

1. Accedi a Dynamics. Fare clic sul menu a discesa **[!UICONTROL Microsoft Dynamics CRM]** e selezionare **[!UICONTROL Settings]**.

   ![](assets/image2015-3-19-8-33-29.png)

1. In **[!UICONTROL Settings]**, selezionare **[!UICONTROL Solutions]**.

   ![](assets/image2015-3-19-8-33-3.png)

1. Fai clic su **[!UICONTROL Import]**.

   ![](assets/image2015-3-19-8-34-8.png)

1. Fai clic su **[!UICONTROL Browse]** e seleziona la soluzione [scaricata](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"}. Fai clic su **Avanti**.

   ![](assets/image2015-3-19-9-20-56.png)

1. Visualizzare le informazioni sulla soluzione e fare clic su **[!UICONTROL View solution package details]**.

   ![](assets/image2015-11-18-11-12-8.png)

1. Dopo aver verificato tutti i dettagli, fare clic su **[!UICONTROL Close]**.

   ![](assets/step6.png)

1. Tornare alla pagina Informazioni sulla soluzione e fare clic su **[!UICONTROL Next]**.

   ![](assets/image2015-3-19-9-21-50.png)

1. Assicurati che la casella di controllo dell’opzione SDK sia selezionata. Fai clic su **[!UICONTROL Import]**.

   ![](assets/image2015-3-19-9-19-12.png)

1. Attendere il completamento dell&#39;importazione.

   >[!TIP]
   >
   >Per completare il processo di installazione, è necessario abilitare i popup nel browser.

   ![](assets/image2015-3-11-11-34-9.png)

1. Scaricare un file di log (se si desidera) e fare clic su **[!UICONTROL Close]**.

   >[!NOTE]
   >
   >È possibile che venga visualizzato un messaggio di avviso che indica &quot;Gestione lead Marketo completata con avviso&quot;. Questo è del tutto previsto.

   ![](assets/image2015-3-13-9-54-39.png)

1. Gestione lead Marketo verrà ora visualizzato nella pagina **[!UICONTROL All Solutions]**.

   ![](assets/image2015-3-19-8-40-38.png)

1. Selezionare la soluzione Marketo e fare clic su **[!UICONTROL Publish All Customizations]**.

   ![](assets/image2015-3-19-8-41-21.png)

   Cinque in alto! L&#39;installazione è terminata.

   >[!CAUTION]
   >
   >Se si disabilita uno dei processi di messaggistica di Marketo SDK, l&#39;installazione non funzionerà.

   >[!MORELIKETHIS]
   >
   >[Installa Marketo per Dynamics 2015 On-Prem e 2016 365 On-Prem Passaggio 2 di 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-2-of-3-set-up.md){target="_blank"}
