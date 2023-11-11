---
description: Installazione di Marketo per Microsoft Dynamics 2016/Dynamics 365 on-premises 1 di 3 - Documentazione di Marketo - Documentazione del prodotto
title: Installazione di Marketo per Microsoft Dynamics 2016/Dynamics 365 on-premises Passaggio 1 di 3
exl-id: 0a494ae7-87da-4ff9-bb47-990b957533e1
feature: Microsoft Dynamics
source-git-commit: 15cb3ddcd82fa1ba60fae3aa1adaac3d5964a0fa
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---

# Passaggio 1 di 3: configurare l’utente Sync per Marketo (on-prem /Dynamics 365 on-premise 2016) {#step-of-configure-sync-user-for-marketo-on-premises-2016}

Prima di poter sincronizzare Microsoft Dynamics 2016 On-Prem/Dynamics 365 con Marketi Engage, è necessario installare la soluzione Marketo in Dynamics.

>[!NOTE]
>
>Dopo aver sincronizzato Marketo con un CRM, non è possibile sincronizzare un nuovo CRM con l&#39;istanza Marketo esistente.

>[!PREREQUISITES]
>
>Se utilizzi Microsoft Dynamics On-Premise, devi disporre di [Distribuzione con connessione Internet](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701){target="_blank"} (IFD) with [Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx){target="_blank"} 2.0+ (ADFS) configurato. Nota: il documento IFD viene scaricato automaticamente quando si fa clic sul collegamento.
>
>[Scarica la soluzione di gestione dei lead Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"} prima di iniziare.

>[!NOTE]
>
>**Autorizzazioni di amministrazione di Dynamics richieste**.
>
>Per eseguire questa sincronizzazione sono necessari privilegi di amministratore CRM.

1. Accedi a Dynamics. Fai clic su **[!UICONTROL Microsoft Dynamics CRM]** menu a discesa e selezionare **[!UICONTROL Impostazioni]**.

   ![](assets/image2015-3-19-8-33-29.png)

1. Sotto **[!UICONTROL Impostazioni]**, seleziona **[!UICONTROL Soluzioni]**.

   ![](assets/image2015-3-19-8-33-3.png)

1. Clic **[!UICONTROL Importa]**.

   ![](assets/image2015-3-19-8-34-8.png)

1. Clic **[!UICONTROL Sfoglia]** e seleziona la soluzione [scaricato](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md){target="_blank"}. Fai clic su **Avanti**.

   ![](assets/image2015-3-19-9-20-56.png)

1. Visualizzare le informazioni sulla soluzione e fare clic su **[!UICONTROL Visualizza dettagli pacchetto soluzione]**.

   ![](assets/image2015-11-18-11-12-8.png)

1. Dopo aver verificato tutti i dettagli, fai clic su **[!UICONTROL Chiudi]**.

   ![](assets/step6.png)

1. Torna alla pagina Informazioni soluzione, fai clic su **[!UICONTROL Successivo]**.

   ![](assets/image2015-3-19-9-21-50.png)

1. Assicurati che la casella di controllo dell’opzione SDK sia selezionata. Clic **[!UICONTROL Importa]**.

   ![](assets/image2015-3-19-9-19-12.png)

1. Attendere il completamento dell&#39;importazione.

   >[!TIP]
   >
   >Per completare il processo di installazione, è necessario abilitare i popup nel browser.

   ![](assets/image2015-3-11-11-34-9.png)

1. Scarica un file di registro (se lo desideri) e fai clic su **[!UICONTROL Chiudi]**.

   >[!NOTE]
   >
   >È possibile che venga visualizzato un messaggio di avviso che indica &quot;Gestione lead Marketo completata con avviso&quot;. Questo è del tutto previsto.

   ![](assets/image2015-3-13-9-54-39.png)

1. Marketo Lead Management verrà ora visualizzato nel **[!UICONTROL Tutte le soluzioni]** pagina.

   ![](assets/image2015-3-19-8-40-38.png)

1. Seleziona la soluzione Marketo e fai clic su **[!UICONTROL Pubblica tutte le personalizzazioni]**.

   ![](assets/image2015-3-19-8-41-21.png)

   Cinque in alto! L&#39;installazione è terminata.

   >[!CAUTION]
   >
   >Se si disabilita uno dei processi di messaggistica SDK di Marketo, l’installazione non funzionerà più.

   >[!MORELIKETHIS]
   >
   >[Installazione di Marketo per Dynamics 2015 On-Prem e 2016 365 On-Prem Passaggio 2 di 3](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2016-dynamics-365-on-premises/step-2-of-3-set-up.md){target="_blank"}
