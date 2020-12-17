---
unique-page-id: 7504736
description: Installazione di Marketo per Dynamics 2015 On-Prem e 2016 365 On-Prem Step 1 di 3 - Marketo Docs - Documentazione prodotto
title: Installazione di Marketo per Dynamics 2015 On-Prem e 2016 365 On-Prem Step 1 di 3
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---


# Passaggio 1 di 3

<!--Install Marketo for Dynamics 2015 On-Prem and 2016 365 On-Prem Step 1 of 3-->

Prima di poter sincronizzare Microsoft Dynamics 2015 On-Premises o 2016 (Dynamics 365) con Marketo, è necessario installare prima la soluzione Marketo in Dynamics.

>[!NOTE]
>
>Dopo aver sincronizzato Marketo con un CRM, non puoi sincronizzare un nuovo CRM con l&#39;istanza Marketo esistente.

>[!PREREQUISITES]
>
>Se si utilizza Microsoft Dynamics On-Premise, è necessario che [Internet Facing Deployment](http://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) (IFD) sia configurato con [Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0+ (ADFS). Nota: Il documento IFD viene scaricato automaticamente quando si fa clic sul collegamento.
>
>[Scarica la ](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) soluzione di gestione dei lead Marketo prima di iniziare.

>[!NOTE]
>
>**Autorizzazioni di amministrazione di Dynamics richieste.**
>
>Per eseguire questa sincronizzazione, sono necessari i privilegi di amministratore CRM.

1. Accedete a **Dynamics.** Fai clic sul menu a discesa  **Microsoft Dynamics** CRM **e seleziona** Impostazioni.

   ![](assets/image2015-3-19-8-33-29.png)

1. In **Impostazioni**, selezionare **Soluzioni**.

   ![](assets/image2015-3-19-8-33-3.png)

1. Fare clic su **Importa**.

   ![](assets/image2015-3-19-8-34-8.png)

1. Fare clic su **Sfoglia** e selezionare la soluzione [scaricata](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Fare clic su **Next**.

   ![](assets/image2015-3-19-9-20-56.png)

1. Visualizzare le informazioni sulla soluzione e fare clic su **Visualizza i dettagli del pacchetto della soluzione**.

   ![](assets/image2015-11-18-11-12-8.png)

1. Dopo aver controllato tutti i dettagli, fare clic su **Chiudi**.

   ![](assets/step6.png)

1. Nella pagina Informazioni sulla soluzione, fate clic su **Avanti**.

   ![](assets/image2015-3-19-9-21-50.png)

1. Accertati che la casella di controllo dell’opzione SDK sia selezionata. Fare clic su **Importa**.

   ![](assets/image2015-3-19-9-19-12.png)

1. Attendere il termine dell&#39;importazione.

   >[!TIP]
   >
   >Sarà necessario abilitare i pop-up nel browser per completare il processo di installazione.

   ![](assets/image2015-3-11-11-34-9.png)

1. Scaricate un file di registro (se lo desiderate) e fate clic su **Chiudi**.

   >[!NOTE]
   >
   >È possibile che venga visualizzato un messaggio con la dicitura &quot;Gestione lead Marketo completata con un avviso&quot;. Ciò è pienamente atteso.

   ![](assets/image2015-3-13-9-54-39.png)

1. La gestione dei lead Marketo verrà ora visualizzata nella pagina **Tutte le soluzioni**.

   ![](assets/image2015-3-19-8-40-38.png)

1. Selezionate la soluzione Marketo e fate clic su **Pubblica tutte le personalizzazioni**.

   ![](assets/image2015-3-19-8-41-21.png)

   Cinque in alto! Installazione completata.

   >[!CAUTION]
   >
   >La disattivazione di uno qualsiasi dei processi di messaggistica SDK di Marketo comporterà l&#39;interruzione dell&#39;installazione.

   >[!NOTE]
   >
   >**Articoli correlati**
   >
   >
   >[Installazione di Marketo per Dynamics 2015 On-Prem e 2016 365 On-Prem Step 2 di 3](step-2-of-3-set-up.md)
