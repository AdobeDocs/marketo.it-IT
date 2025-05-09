---
unique-page-id: 7504736
description: Installazione di Marketo per Microsoft Dynamics 2015 on-premises Passaggio 1 di 3 - Documentazione di Marketo - Documentazione del prodotto
title: Installazione di Marketo per Microsoft Dynamics 2015 on-premise - Passaggio 1 di 3
exl-id: c9b6d365-15c1-4eff-938c-8433b1fe7f24
feature: Microsoft Dynamics
source-git-commit: 821d69736b1cbeac0c80718c58a7a3c471387545
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 0%

---

# Passaggio 1 di 3: configurare l’utente Sync per Marketo (on-prem 2015) {#step-of-configure-sync-user-for-marketo-on-premises-2015}

Prima di poter sincronizzare Microsoft Dynamics 2015 On-Premises con il Marketo Engage, è necessario installare la soluzione Marketo in Dynamics.

>[!NOTE]
>
>Dopo aver sincronizzato Marketo con un CRM, non è possibile sincronizzare un nuovo CRM con l&#39;istanza Marketo esistente.

>[!PREREQUISITES]
>
>Se si utilizza Microsoft Dynamics On-Premise, è necessario configurare [Distribuzione con connessione Internet](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701){target="_blank"} (IFD) con [Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"} 2.0+ (ADFS). Nota: il documento IFD viene scaricato automaticamente quando si fa clic sul collegamento.
>
>[Scaricare la soluzione Marketo per la gestione dei lead](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"} prima di iniziare.

>[!NOTE]
>
>**Autorizzazioni amministratore Dynamics richieste**.
>
>Per eseguire questa sincronizzazione sono necessari privilegi di amministratore CRM.

1. Accedi a Dynamics. Fare clic sul menu a discesa **[!UICONTROL Microsoft Dynamics CRM]** e selezionare **[!UICONTROL Impostazioni]**.

   ![](assets/image2015-3-19-8-33-29.png)

1. In **[!UICONTROL Impostazioni]**, seleziona **[!UICONTROL Soluzioni]**.

   ![](assets/image2015-3-19-8-33-3.png)

1. Fai clic su **[!UICONTROL Importa]**.

   ![](assets/image2015-3-19-8-34-8.png)

1. Fai clic su **[!UICONTROL Sfoglia]** e seleziona la soluzione [scaricata](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Fai clic su **[!UICONTROL Avanti]**.

   ![](assets/image2015-3-19-9-20-56.png)

1. Visualizzare le informazioni sulla soluzione e fare clic su **[!UICONTROL Visualizza dettagli pacchetto soluzione]**.

   ![](assets/image2015-11-18-11-12-8.png)

1. Dopo aver verificato tutti i dettagli, fare clic su **[!UICONTROL Chiudi]**.

   ![](assets/step6.png)

1. Tornando alla pagina Informazioni sulla soluzione, fai clic su **[!UICONTROL Avanti]**.

   ![](assets/image2015-3-19-9-21-50.png)

1. Assicurati che la casella di controllo dell’opzione SDK sia selezionata. Fai clic su **[!UICONTROL Importa]**.

   ![](assets/image2015-3-19-9-19-12.png)

1. Attendere il completamento dell&#39;importazione.

   >[!TIP]
   >
   >Per completare il processo di installazione, è necessario abilitare i popup nel browser.

   ![](assets/image2015-3-11-11-34-9.png)

1. Scaricare un file di log (se si desidera) e fare clic su **[!UICONTROL Chiudi]**.

   >[!NOTE]
   >
   >È possibile che venga visualizzato un messaggio di avviso che indica &quot;Gestione lead Marketo completata con avviso&quot;. Questo è del tutto previsto.

   ![](assets/image2015-3-13-9-54-39.png)

1. Gestione lead Marketo verrà ora visualizzato nella pagina **[!UICONTROL Tutte le soluzioni]**.

   ![](assets/image2015-3-19-8-40-38.png)

1. Seleziona la soluzione Marketo e fai clic su **[!UICONTROL Tutte le personalizzazioni di Publish]**.

   ![](assets/image2015-3-19-8-41-21.png)

   Ottimo lavoro. L&#39;installazione è terminata.

   >[!CAUTION]
   >
   >Se si disabilita uno dei processi di messaggistica SDK di Marketo, l’installazione non funzionerà più.

   >[!MORELIKETHIS]
   >
   >[Installa Marketo per Microsoft Dynamics 2015 locale Passaggio 2 di 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-set-up-2015.md){target="_blank"}
