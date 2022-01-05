---
description: Passaggio 1 di 3 - Installare la soluzione Marketo con la connessione per il controllo della password del proprietario della risorsa - Documenti Marketo - Documentazione del prodotto
title: Passaggio 1 di 3 - Installare la soluzione Marketo con la connessione per il controllo della password del proprietario della risorsa
source-git-commit: e46673423bdb2757e8a9f97dc702d32d02200e6e
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 0%

---

# Passaggio 1 di 3: Installare la soluzione Marketo con la connessione Controllo password proprietario risorsa {#step-1-of-3-install-the-marketo-solution-ropc}

Prima di poter sincronizzare Microsoft Dynamics 365 e Marketo, è necessario installare la soluzione Marketo in Dynamics. **Le autorizzazioni di Dynamics Admin sono necessarie.**

>[!CAUTION]
>
>* Non abilitare la sincronizzazione di entità personalizzata prima del completamento della sincronizzazione iniziale. Una volta completata la sincronizzazione iniziale, riceverai una notifica via e-mail.
>* Se per la sincronizzazione di Dynamics è abilitata l’autenticazione a più fattori (MFA), devi disattivarla affinché Dynamics si sincronizzi correttamente con Marketo. Per ulteriori informazioni, contattare [Supporto Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).


>[!NOTE]
>
>Dopo aver sincronizzato Marketo con un CRM, non puoi eseguire una nuova sincronizzazione senza sostituire l&#39;istanza.

>[!PREREQUISITES]
>
>[Scarica la soluzione Marketo per la gestione dei lead](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md)

1. Accedi a **[Microsoft Office 365](https://login.microsoftonline.com/)**.

   ![](assets/image2015-3-16-15-3a58-3a55.png)

1. Fai clic su ![](assets/image2015-3-16-16-3a1-3a13.png) menu e seleziona **CRM**.

   ![](assets/image2015-3-16-16-3a0-3a10.png)

1. Fai clic su ![](assets/image2015-5-13-10-3a5-3a8.png) menu. Nel menu a discesa seleziona **Impostazioni** quindi seleziona **Soluzioni**.

   ![](assets/image2015-5-13-10-3a4-3a1.png)

1. Fai clic su **Importa.**

   ![](assets/image2015-3-19-8-3a34-3a8.png)

1. Fai clic su **Scegliere File.** Seleziona la soluzione Marketo Lead Management [scaricato](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Fai clic su **Successivo**.

   ![](assets/image2015-10-9-14-3a44-3a14.png)

1. Visualizza le informazioni sulla soluzione e fai clic su **Visualizza i dettagli del pacchetto della soluzione**.

   ![](assets/image2015-10-9-15-3a4-3a16.png)

1. Dopo aver controllato tutti i dettagli, fai clic su **Chiudi**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. Ora, nella pagina Informazioni sulla soluzione, fai clic su **Successivo**.

   ![](assets/image2015-10-9-14-3a59-3a24.png)

1. Assicurati che la casella di controllo dell&#39;opzione SDK sia selezionata. Fai clic su **Importa**.

   ![](assets/image2015-10-9-15-3a7-3a12.png)

   >[!TIP]
   >
   >Sarà necessario abilitare i pop-up sul browser per completare il processo di installazione.

1. Ora attendi il completamento dell’importazione. Alzati e fai delle distese.

   ![](assets/image2015-3-11-11-3a34-3a9.png)

1. Fai clic su **Chiudi.**

   >[!NOTE]
   >
   >È possibile che venga visualizzato un messaggio che indica &quot;Gestione lead Marketo completata con un avviso&quot;. Ciò è pienamente atteso.

   ![](assets/image2015-3-13-9-3a54-3a39.png)

1. Gestione lead Marketo verrà ora incluso nell’elenco delle soluzioni.

   ![](assets/image2015-3-19-8-3a40-3a38.png)

1. Seleziona **Gestione dei lead Marketo** e fai clic su **Pubblica Tutte Le Personalizzazioni.**

   ![](assets/image2015-3-19-8-3a41-3a21.png)

   Cinque in alto! Installazione completata.

   >[!MORELIKETHIS]
   >
   >[Passaggio 2 di 4: Configurare la soluzione Marketo con la connessione Controllo password proprietario risorsa](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-2-of-4-set-up.md)
