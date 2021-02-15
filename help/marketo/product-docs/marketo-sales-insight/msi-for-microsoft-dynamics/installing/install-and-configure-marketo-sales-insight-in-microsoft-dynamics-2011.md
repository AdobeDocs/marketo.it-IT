---
unique-page-id: 3571735
description: Installazione e configurazione di Marketing Sales Insight in Microsoft Dynamics 2011 - Marketo Docs - Documentazione prodotto
title: Installazione e configurazione di Marketing Sales Insight in Microsoft Dynamics 2011
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 0%

---


# Installazione e configurazione di Marketing Sales Insight in Microsoft Dynamics 2011 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketing Sales Insight è uno strumento fantastico per il vostro team di vendita. Di seguito sono riportate le istruzioni dettagliate su come installarlo e configurarlo nei locali di Microsoft Dynamics 2011.

>[!PREREQUISITES]
>
>Completate l&#39;integrazione tra Marketo e Microsoft.
>
>[Scarica la ](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) soluzione corretta per la versione di Microsoft Dynamics CRM in uso.

## Soluzione di importazione {#import-solution}

1. Accedi a Microsoft Dynamics CRM. Fare clic su **Impostazioni** nel menu in basso a sinistra.

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. Selezionare **Soluzioni** nella struttura.

   ![](assets/image2015-5-4-10-3a41-3a56.png)

1. Fare clic su **Importa** ( ![](assets/image2015-5-4-10-3a45-3a44.png)).

   ![](assets/image2015-5-4-10-3a42-3a38.png)

   >[!NOTE]
   >
   >Prima di procedere, è già necessario che [sia installata e configurata](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-2011.md) la soluzione Marketo.

1. Fare clic su **Sfoglia**. Selezionate la soluzione Marketing Sales Insight [scaricata](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md). Fare clic su **Next**.

   ![](assets/image2015-5-4-10-3a55-3a15.png)

1. Verificate i dettagli della soluzione e fate clic su **Next**.

   ![](assets/image2015-5-4-10-3a57-3a31.png)

1. Accertati che l’opzione Messaggio SDK sia selezionata. Fare clic su **Next**.

   ![](assets/image2015-5-4-11-3a43-3a37.png)

1. Attendere il termine dell&#39;importazione.

   ![](assets/image2015-5-4-11-3a0-3a58.png)

1. Fare clic su **Chiudi**.

   ![](assets/crmhand.png)

1. Marketing Sales Insight verrà visualizzato nell&#39;elenco delle soluzioni. Sì!

   ![](assets/image2015-5-4-11-3a2-3a37.png)

1. Selezionare Marketing Sales Insight e fare clic su **Pubblica tutte le personalizzazioni** ( ![](assets/image2015-5-4-11-3a7-3a8.png)).

   ![](assets/image2015-5-4-11-3a8-3a27.png)

## Connect Marketing e Sales Insight {#connect-marketo-and-sales-insight}

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

1. Accedete a Marketo e fate clic su **Admin**.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. Nella sezione **Sales Insight** fare clic su **Edit API Configuration** (Modifica configurazione API).

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Copiate l&#39;**Marketo Host**, **URL API** e l&#39;**ID utente API** da utilizzare in un secondo momento. Immettete una **Chiave segreta API** di vostra scelta e fate clic su **Salva**.

   >[!CAUTION]
   >
   >Non utilizzate una e commerciale (&amp;) nella chiave segreta API.

   ![](assets/image2015-5-4-11-3a16-3a3.png)

   >[!NOTE]
   >
   >Per il funzionamento di _Lead e Contact_, è necessario sincronizzare i campi seguenti con Marketo:
   >
   >* Priorità
   >* Urgenza
   >* Punteggio relativo

   >
   >Se manca uno di questi campi, in Marketo verrà visualizzato un messaggio di errore con il nome dei campi mancanti. Per risolvere il problema, eseguire [questa procedura](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. Torna a Dynamics, seleziona **Settings**.

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. Selezionare **Configurazione API Marketo** nella struttura.

   ![](assets/image2015-5-4-11-3a22-3a41.png)

1. Fare clic su **Configurazione predefinita**.

   ![](assets/image2015-5-4-11-3a26-3a10.png)

1. Inserite le informazioni da Marketo a precedente.

   ![](assets/image2015-5-4-11-3a27-3a16.png)

1. Fare clic su **Salva**.

   ![](assets/image2015-5-4-11-3a28-3a13.png)

## Imposta accesso utente {#set-user-access}

Configurate i ruoli utente per consentire a utenti specifici di accedere a Sales Insight.

1. Selezionare **Settings**.

   ![](assets/image2015-5-4-11-3a30-3a54.png)

1. Selezionare **Amministrazione** nella struttura.

   ![](assets/image2015-5-4-11-3a31-3a39.png)

1. Fare clic su **Utenti**.

   ![](assets/image2015-5-4-11-3a32-3a25.png)

1. Selezionare gli utenti a cui si desidera concedere l&#39;accesso e fare clic su **Gestisci ruoli**.

   ![](assets/image2015-5-4-11-3a35-3a8.png)

1. Selezionare il ruolo **Marketing Sales Insight** e fare clic su **OK**.

   ![](assets/image2015-5-4-11-3a36-3a59.png)

   Ed è tutto! Tutti gli utenti dispongono dell&#39;accesso per visualizzare la sezione Informazioni sulle vendite nella visualizzazione Dettagli lead/contatto.

   ![](assets/image2015-5-4-11-3a39-3a23.png)

   Congratulazioni. Ora hai scatenato la potenza di Marketing Sales Insight.

>[!MORELIKETHIS]
>
>[Impostazione di stelle e fiamme per i record lead/contatto](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
