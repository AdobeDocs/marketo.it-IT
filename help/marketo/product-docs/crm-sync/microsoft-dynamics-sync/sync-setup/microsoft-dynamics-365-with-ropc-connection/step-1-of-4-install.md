---
description: Passaggio 1 di 4 - Installare la soluzione Marketo con la connessione per il controllo della password del proprietario della risorsa - Documentazione di Marketo - Documentazione del prodotto
title: Passaggio 1 di 4 - Installare la soluzione Marketo con la connessione di controllo della password del proprietario della risorsa
exl-id: aab3bbb8-4e52-4c40-94d1-631af1d63f9f
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 0%

---

# Passaggio 1 di 4: installare la soluzione Marketo con la connessione di controllo della password del proprietario della risorsa {#step-1-of-4-install-the-marketo-solution-ropc}

Prima di poter sincronizzare Microsoft Dynamics 365 e Marketo, è necessario installare la soluzione Marketo in Dynamics. **Sono necessarie le autorizzazioni di amministrazione di Dynamics.**

>[!CAUTION]
>
>* Non abilitare la sincronizzazione di entità personalizzata prima del completamento della sincronizzazione iniziale. Al termine della sincronizzazione iniziale, riceverai una notifica via e-mail.
>* Se per Dynamics Sync è abilitato Multi-Factor Authentication (MFA), è necessario disattivarlo per consentire la corretta sincronizzazione di Dynamics con Marketo. Per ulteriori informazioni, contattare [Supporto Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

>[!NOTE]
>
>Dopo aver sincronizzato Marketo con un CRM, non è possibile eseguire una nuova sincronizzazione senza sostituire l&#39;istanza.

>[!PREREQUISITES]
>
>[Scarica la soluzione di gestione dei lead Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)

1. Accedi a **[Microsoft Office 365](https://login.microsoftonline.com/)**.

   ![](assets/image2015-3-16-15-3a58-3a55.png)

1. Clic ![](assets/image2015-3-16-16-3a1-3a13.png) menu e seleziona **CRM**.

   ![](assets/image2015-3-16-16-3a0-3a10.png)

1. Clic ![](assets/image2015-5-13-10-3a5-3a8.png) menu. Nel menu a discesa seleziona **Impostazioni** quindi seleziona **Soluzioni**.

   ![](assets/image2015-5-13-10-3a4-3a1.png)

1. Clic **Importa.**

   ![](assets/image2015-3-19-8-3a34-3a8.png)

1. Clic **Scegliere File.** Selezionare la soluzione di gestione dei lead Marketo [scaricato](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Clic **Successivo**.

   ![](assets/image2015-10-9-14-3a44-3a14.png)

1. Visualizzare le informazioni sulla soluzione e fare clic su **Visualizza dettagli pacchetto soluzione**.

   ![](assets/image2015-10-9-15-3a4-3a16.png)

1. Dopo aver verificato tutti i dettagli, fai clic su **Chiudi**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. Ora, tornando alla pagina Informazioni sulla soluzione, fai clic su **Successivo**.

   ![](assets/image2015-10-9-14-3a59-3a24.png)

1. Assicurati che la casella di controllo dell’opzione SDK sia selezionata. Clic **Importa**.

   ![](assets/image2015-10-9-15-3a7-3a12.png)

   >[!TIP]
   >
   >Per completare il processo di installazione, è necessario abilitare i popup nel browser.

1. Ora attendi il completamento dell’importazione. Alzati e fai qualche tratto.

   ![](assets/image2015-3-11-11-3a34-3a9.png)

1. Fai clic su **Chiudi.**

   >[!NOTE]
   >
   >È possibile che venga visualizzato un messaggio di avviso che indica &quot;Gestione lead Marketo completata con avviso&quot;. Questo è del tutto previsto.

   ![](assets/image2015-3-13-9-3a54-3a39.png)

1. Gestione lead Marketo verrà ora visualizzato nell’elenco delle soluzioni.

   ![](assets/image2015-3-19-8-3a40-3a38.png)

1. Seleziona **Gestione lead Marketo** e fai clic su **Pubblica tutte le personalizzazioni.**

   ![](assets/image2015-3-19-8-3a41-3a21.png)

   Cinque in alto! L&#39;installazione è terminata.

   >[!MORELIKETHIS]
   >
   >[Passaggio 2 di 4: configurare la soluzione Marketo con la connessione di controllo della password del proprietario della risorsa](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md)
