---
unique-page-id: 3571805
description: Passaggio 1 di 3 - Installare la soluzione Marketo (On-Premises 2011) - Marketo Docs - Documentazione del prodotto
title: Passaggio 1 di 3 - Installare la soluzione Marketo (2011 On-Premises)
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---


# Passaggio 1 di 3: Installare la soluzione Marketo (On-Premises 2011) {#step-of-install-the-marketo-solution-on-premises}

Prima di poter sincronizzare Microsoft Dynamics On-Premises e Marketo, è necessario installare la soluzione Marketo in Dynamics.

>[!NOTE]
>
>Dopo aver sincronizzato Marketo con un CRM, non puoi eseguire una nuova sincronizzazione senza sostituire l&#39;istanza.

>[!PREREQUISITES]
>
>È necessario che [Distribuzione su Internet](http://www.microsoft.com/en-us/download/confirmation.aspx?id=41701) (IFD) sia configurato [Active Directory Federation Services](https://msdn.microsoft.com/en-us/library/bb897402.aspx) 2.0, 2.1 o 3.0 (ADFS). **Nota**: Il documento IFD viene scaricato automaticamente quando si fa clic sul collegamento.
>
>[Scarica la ](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md) soluzione di gestione dei lead Marketo prima di iniziare.

>[!NOTE]
>
>**Autorizzazioni di amministrazione di Dynamics richieste.**
>
>Per eseguire questa sincronizzazione, sono necessari i privilegi di amministratore CRM.

1. Accedete a **Dynamics**, selezionate **Settings** nel menu in basso a sinistra.

   ![](assets/image2015-4-2-11-3a32-3a53.png)

1. Selezionare **Soluzioni** nella struttura.

   ![](assets/image2015-4-2-11-3a35-3a28.png)

1. Fare clic su **Importa**.

   ![](assets/image2015-4-2-11-3a37-3a33.png)

1. Fare clic su **Sfoglia**. Selezionate la soluzione Marketing To Lead Management che avete [scaricato](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/download-the-marketo-lead-management-solution.md). Fare clic su **Next**.

   ![](assets/image2015-4-2-11-3a40-3a33.png)

1. Visualizzare le informazioni sulla soluzione e fare clic su **Visualizza i dettagli del pacchetto della soluzione**.

   ![](assets/image2015-11-18-11-3a12-3a8.png)

1. Dopo aver controllato tutti i dettagli, fare clic su **Chiudi**.

   ![](assets/image2015-10-9-14-3a57-3a3.png)

1. Nella pagina Informazioni sulla soluzione, fate clic su **Avanti**.

   ![](assets/image2015-4-2-11-3a41-3a48.png)

1. Accertati che la casella di controllo relativa all’opzione Messaggio SDK sia selezionata. Fare clic su **Next**.

   ![](assets/image2015-4-2-11-3a42-3a37.png)

   >[!TIP]
   >
   >Sarà necessario abilitare i pop-up nel browser per completare il processo di installazione.

1. Attendere il termine dell&#39;importazione. Alzati e fai qualche stirata.

   ![](assets/image2015-4-2-11-3a43-3a51.png)

1. Fare clic su **Chiudi**.

   >[!NOTE]
   >
   >È possibile che venga visualizzato un messaggio con la dicitura &quot;Gestione lead Marketo completata con un avviso&quot;. Ciò è pienamente atteso.

   ![](assets/image2015-4-2-11-3a44-3a44.png)

1. La gestione dei lead Marketo verrà ora visualizzata nella pagina **Tutte le soluzioni**.

   ![](assets/image2015-4-2-11-3a46-3a55.png)

1. Selezionare Gestione lead Marketo e fare clic su **Pubblica tutte le personalizzazioni.**

   ![](assets/image2015-4-2-11-3a48-3a21.png)

Non era troppo male, giusto? Avanti, continuerò a passarvi attraverso il resto.

>[!CAUTION]
>
>La disattivazione di uno qualsiasi dei processi di messaggistica SDK di Marketo comporterà l&#39;interruzione dell&#39;installazione.

>[!NOTE]
>
>**Articoli correlati**
>
>[Passaggio 2 di 3: Impostazione della sincronizzazione degli utenti di Marketing in Dynamics (On-Premises 2011)](step-2-of-3-set-up.md)
