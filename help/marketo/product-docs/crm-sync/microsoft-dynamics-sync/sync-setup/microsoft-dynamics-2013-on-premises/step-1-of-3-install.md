---
unique-page-id: 3571813
description: Passaggio 1 di 3 - Installare la soluzione Marketo in Dynamics (2013 On-Premises) - Marketo Docs - Documentazione prodotto
title: Passaggio 1 di 3 - Installare la soluzione Marketo in Dynamics (2013 On-Premises)
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---


# Passaggio 1 di 3: Installare la soluzione Marketo in Dynamics (2013 On-Premises) {#step-of-install-the-marketo-solution-in-dynamics-on-premises}

Prima di poter sincronizzare Microsoft Dynamics On-Premises e Marketo, è necessario installare la soluzione Marketo in Dynamics.

>[!NOTE]
>
>Dopo aver sincronizzato Marketo con un CRM, non puoi eseguire una nuova sincronizzazione senza sostituire l&#39;istanza.

>[!PREREQUISITES]
>
>È necessario che [Distribuzione su Internet](https://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) (IFD) sia configurato [Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0, 2.1 o 3.0 (ADFS). Nota: Il documento IFD viene scaricato automaticamente quando si fa clic sul collegamento.
>
>[Scarica la ](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) soluzione Marketo prima di iniziare.

>[!NOTE]
>
>**Autorizzazioni di amministrazione di Dynamics richieste.**
>
>Per eseguire questa sincronizzazione, sono necessari i privilegi di amministratore CRM.

1. Accedere a **Dynamics**. Fare clic sul menu a discesa **Microsoft Dynamics CRM** e selezionare **Impostazioni**.

   ![](assets/image2014-12-11-10-3a39-3a41.png)

1. In **Impostazioni**, selezionare **Soluzioni**.

   ![](assets/image2014-12-11-10-3a39-3a51.png)

1. Fare clic su **Importa**.

   ![](assets/image2015-3-26-9-3a52-3a10.png)

1. Fare clic su **Sfoglia** e selezionare la [soluzione scaricata](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Fare clic su **Next**.

   ![](assets/image2015-3-26-9-3a54-3a1.png)

1. Visualizzare le informazioni sulla soluzione e fare clic su **Visualizza i dettagli del pacchetto della soluzione**.

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. Dopo aver controllato tutti i dettagli, fare clic su **Chiudi**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. Nella pagina Informazioni sulla soluzione, fate clic su **Avanti**.

   ![](assets/image2015-3-26-9-3a55-3a17.png)

1. Accertati che l’opzione SDK sia selezionata. Fare clic su **Importa**.

   ![](assets/image2015-3-26-10-3a3-3a11.png)

1. Attendere il termine dell&#39;importazione.

   >[!TIP]
   >
   >Sarà necessario abilitare i pop-up nel browser per completare il processo di installazione.

   ![](assets/image2014-12-11-10-3a41-3a5.png)

1. Scaricate un file di registro (se lo desiderate) e fate clic su **Chiudi**.

   >[!NOTE]
   >
   >È possibile che venga visualizzato un messaggio con la dicitura &quot;Gestione lead Marketo completata con un avviso&quot;. Ciò è pienamente atteso.

   ![](assets/image2014-12-11-10-3a41-3a14.png)

1. La gestione dei lead Marketo verrà ora visualizzata nella pagina **Tutte le soluzioni**.

   ![](assets/image2015-3-26-10-3a1-3a21.png)

1. Selezionate la soluzione Marketo e fate clic su **Pubblica tutte le personalizzazioni**.

   ![](assets/image2014-12-11-10-3a41-3a32.png)

Non era troppo male, giusto? Avanti, continuerò a passarvi attraverso il resto.

>[!CAUTION]
>
>La disattivazione di uno qualsiasi dei processi di messaggistica SDK di Marketo comporterà l&#39;interruzione dell&#39;installazione.

>[!MORELIKETHIS]
>
>[Passaggio 2 di 3: Configurare l&#39;utente di sincronizzazione per Marketo (On-Premises 2013)](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-2013-on-premises/step-2-of-3-configure.md)
