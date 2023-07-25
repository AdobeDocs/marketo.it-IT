---
unique-page-id: 3571813
description: 'Passaggio 1 di 3: installare la soluzione Marketo in Dynamics (on-premises 2013) - Documentazione di Marketo - Documentazione del prodotto'
title: 'Passaggio 1 di 3: installare la soluzione Marketo in Dynamics (on-premises 2013)'
exl-id: 89f90bca-b459-447f-bbdd-363f232a1059
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---

# Passaggio 1 di 3: installare la soluzione Marketo in Dynamics (on-premises 2013) {#step-of-install-the-marketo-solution-in-dynamics-on-premises}

Prima di poter sincronizzare Microsoft Dynamics On-Premises e Marketo, è necessario installare la soluzione Marketo in Dynamics.

>[!NOTE]
>
>Dopo aver sincronizzato Marketo con un CRM, non è possibile eseguire una nuova sincronizzazione senza sostituire l&#39;istanza.

>[!PREREQUISITES]
>
>Devi avere [Distribuzione con connessione Internet](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) (IFD) [Servizi federativi Active Directory](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0, 2.1 o 3.0 (ADFS) configurati. Nota: il documento IFD viene scaricato automaticamente quando si fa clic sul collegamento.
>
>[Scarica la soluzione Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) prima di iniziare.

>[!NOTE]
>
>**Autorizzazioni di amministrazione di Dynamics richieste.**
>
>Per eseguire questa sincronizzazione sono necessari privilegi di amministratore CRM.

1. Accedi a **Dynamics**. Fai clic su **Microsoft Dynamics CRM** menu a discesa e selezionare **Impostazioni**.

   ![](assets/image2014-12-11-10-3a39-3a41.png)

1. Sotto **Impostazioni**, seleziona **Soluzioni**.

   ![](assets/image2014-12-11-10-3a39-3a51.png)

1. Clic **Importa**.

   ![](assets/image2015-3-26-9-3a52-3a10.png)

1. Clic **Sfoglia** e seleziona la [soluzione scaricata](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Clic **Successivo**.

   ![](assets/image2015-3-26-9-3a54-3a1.png)

1. Visualizzare le informazioni sulla soluzione e fare clic su **Visualizza dettagli pacchetto soluzione**.

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. Dopo aver verificato tutti i dettagli, fai clic su **Chiudi**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. Torna alla pagina Informazioni soluzione, fai clic su **Successivo**.

   ![](assets/image2015-3-26-9-3a55-3a17.png)

1. Assicurati che l’opzione SDK sia selezionata. Clic **Importa**.

   ![](assets/image2015-3-26-10-3a3-3a11.png)

1. Attendere il completamento dell&#39;importazione.

   >[!TIP]
   >
   >Per completare il processo di installazione, è necessario abilitare i popup nel browser.

   ![](assets/image2014-12-11-10-3a41-3a5.png)

1. Scarica un file di registro (se lo desideri) e fai clic su **Chiudi**.

   >[!NOTE]
   >
   >È possibile che venga visualizzato un messaggio di avviso che indica &quot;Gestione lead Marketo completata con avviso&quot;. Questo è del tutto previsto.

   ![](assets/image2014-12-11-10-3a41-3a14.png)

1. Marketo Lead Management verrà ora visualizzato nel **Tutte le soluzioni** pagina.

   ![](assets/image2015-3-26-10-3a1-3a21.png)

1. Seleziona la soluzione Marketo e fai clic su **Pubblica tutte le personalizzazioni**.

   ![](assets/image2014-12-11-10-3a41-3a32.png)

Non è stato male, vero? Avanti, continuerò a accompagnarti nel resto.

>[!CAUTION]
>
>Se si disabilita uno dei processi di messaggistica SDK di Marketo, l’installazione non funzionerà più.

>[!MORELIKETHIS]
>
>[Passaggio 2 di 3: configurare l&#39;utente Sync per Marketo (on-premises 2013)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/connecting-to-legacy-versions/step-2-of-3-configure-2013.md)
