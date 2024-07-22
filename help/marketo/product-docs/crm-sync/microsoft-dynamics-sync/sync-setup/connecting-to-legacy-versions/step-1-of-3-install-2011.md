---
unique-page-id: 3571805
description: 'Passaggio 1 di 3: installare la soluzione Marketo (on-premise 2011) - Documentazione di Marketo - Documentazione del prodotto'
title: 'Passaggio 1 di 3: installazione della soluzione Marketo (on-premise 2011)'
exl-id: 6e559b10-5273-4dc2-b98d-49c509cbeff7
feature: Microsoft Dynamics
source-git-commit: 821d69736b1cbeac0c80718c58a7a3c471387545
workflow-type: tm+mt
source-wordcount: '285'
ht-degree: 0%

---

# Passaggio 1 di 3: installare la soluzione Marketo (on-premise 2011) {#step-of-install-the-marketo-solution-on-premises}

Prima di poter sincronizzare Microsoft Dynamics On-Premises e Marketo Engage, è necessario installare la soluzione Marketo in Dynamics.

>[!NOTE]
>
>Dopo aver sincronizzato Marketo con un CRM, non è possibile eseguire una nuova sincronizzazione senza sostituire l&#39;istanza.

>[!PREREQUISITES]
>
>È necessario che sia configurato [Internet Facing Deployment](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701){target="_blank"} (IFD) con [Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"} 2.0, 2.1 o 3.0 (ADFS). **Nota**: il documento IFD viene scaricato automaticamente quando si fa clic sul collegamento.
>
>[Scaricare la soluzione Marketo per la gestione dei lead](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"} prima di iniziare.

>[!NOTE]
>
>**Autorizzazioni amministratore Dynamics richieste**.
>
>Per eseguire questa sincronizzazione sono necessari privilegi di amministratore CRM.

1. Accedi a Dynamics e seleziona **[!UICONTROL Impostazioni]** nel menu in basso a sinistra.

   ![](assets/image2015-4-2-11-3a32-3a53.png)

1. Seleziona **[!UICONTROL Soluzioni]** nella struttura.

   ![](assets/image2015-4-2-11-3a35-3a28.png)

1. Fai clic su **[!UICONTROL Importa]**.

   ![](assets/image2015-4-2-11-3a37-3a33.png)

1. Fare clic su **[!UICONTROL Sfoglia]**. Selezionare la soluzione di gestione dei lead di Marketo [scaricata](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"}. Fai clic su **[!UICONTROL Avanti]**.

   ![](assets/image2015-4-2-11-3a40-3a33.png)

1. Visualizzare le informazioni sulla soluzione e fare clic su **[!UICONTROL Visualizza dettagli pacchetto soluzione]**.

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. Dopo aver verificato tutti i dettagli, fare clic su **[!UICONTROL Chiudi]**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. Tornando alla pagina Informazioni sulla soluzione, fai clic su **[!UICONTROL Avanti]**.

   ![](assets/image2015-4-2-11-3a41-3a48.png)

1. Assicurati che la casella di controllo dell’opzione del messaggio SDK sia selezionata. Fai clic su **[!UICONTROL Avanti]**.

   ![](assets/image2015-4-2-11-3a42-3a37.png)

   >[!TIP]
   >
   >Per completare il processo di installazione, è necessario abilitare i popup nel browser.

1. Ora attendi il completamento dell’importazione. Alzati e fai qualche tratto.

   ![](assets/image2015-4-2-11-3a43-3a51.png)

1. Fai clic su **[!UICONTROL Chiudi]**.

   >[!NOTE]
   >
   >È possibile che venga visualizzato un messaggio di avviso che indica &quot;Gestione lead Marketo completata con avviso&quot;. Questo è del tutto previsto.

   ![](assets/image2015-4-2-11-3a44-3a44.png)

1. Gestione lead Marketo verrà ora visualizzato nella pagina **Tutte le soluzioni**.

   ![](assets/image2015-4-2-11-3a46-3a55.png)

1. Selezionare Gestione lead Marketo e fare clic su **[!UICONTROL Tutte le personalizzazioni di Publish]**.

   ![](assets/image2015-4-2-11-3a48-3a21.png)

>[!CAUTION]
>
>Se si disabilita uno dei processi di messaggistica SDK di Marketo, l’installazione non funzionerà più.

>[!MORELIKETHIS]
>
>[Passaggio 2 di 3: configurazione utente di Marketo Sync in Dynamics (2011 on-premise)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-set-up-2011.md){target="_blank"}
