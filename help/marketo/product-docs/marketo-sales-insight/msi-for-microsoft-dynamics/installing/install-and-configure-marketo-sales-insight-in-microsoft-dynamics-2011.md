---
unique-page-id: 3571735
description: Installare e configurare Marketo Sales Insight in Microsoft Dynamics 2011 - Documentazione di Marketo - Documentazione del prodotto
title: Installare e configurare Marketo Sales Insight in Microsoft Dynamics 2011
exl-id: 40622dcc-7129-4392-95dc-ca829c15c3a6
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 1%

---

# Installare e configurare Marketo Sales Insight in Microsoft Dynamics 2011 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo Sales Insight è uno strumento fantastico per il vostro team di vendita. Di seguito sono riportate istruzioni dettagliate su come installarlo e configurarlo in Microsoft Dynamics 2011 On-Premises.

>[!PREREQUISITES]
>
>Completa l&#39;integrazione Marketo-Microsoft.
>
>[Scarica la soluzione corretta](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) per la versione di Microsoft Dynamics CRM in uso.

## Importa soluzione {#import-solution}

1. Accedere a Microsoft Dynamics CRM. Fai clic su **Impostazioni** nel menu in basso a sinistra.

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. Seleziona **Soluzioni** nella struttura.

   ![](assets/image2015-5-4-10-3a41-3a56.png)

1. Fai clic su **Importa** ( ![](assets/image2015-5-4-10-3a45-3a44.png)).

   ![](assets/image2015-5-4-10-3a42-3a38.png)

   >[!NOTE]
   >
   >Prima di procedere, dovresti avere già [installato e configurato](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-2011.md) la soluzione Marketo.

1. Fare clic su **Sfoglia**. Selezionare la soluzione Marketo Sales Insight [scaricata](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md). Fai clic su **Avanti**.

   ![](assets/image2015-5-4-10-3a55-3a15.png)

1. Verificare i dettagli della soluzione e fare clic su **Avanti**.

   ![](assets/image2015-5-4-10-3a57-3a31.png)

1. Assicurati che l’opzione Messaggio SDK sia selezionata. Fai clic su **Avanti**.

   ![](assets/image2015-5-4-11-3a43-3a37.png)

1. Ora attendi il completamento dell’importazione.

   ![](assets/image2015-5-4-11-3a0-3a58.png)

1. Fai clic su **Chiudi**.

   ![](assets/crmhand.png)

1. Marketo Sales Insight verrà ora visualizzato nell&#39;elenco delle soluzioni. Yay!

   ![](assets/image2015-5-4-11-3a2-3a37.png)

1. Seleziona Marketo Sales Insight e fai clic su **Publish Tutte le personalizzazioni** ( ![](assets/image2015-5-4-11-3a7-3a8.png)).

   ![](assets/image2015-5-4-11-3a8-3a27.png)

## Connettere Marketo e Sales Insight  {#connect-marketo-and-sales-insight}

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

1. Accedi a Marketo e fai clic su **Amministratore**.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. Nella sezione **Informazioni sulle vendite** fai clic su **Modifica configurazione API**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Copiare l&#39;**host Marketo**, l&#39;**URL API** e l&#39;**ID utente API** da utilizzare in un passaggio successivo. Immetti una **chiave segreta API** a tua scelta e fai clic su **Salva**.

   >[!CAUTION]
   >
   >Non utilizzare una e commerciale (&amp;) nella chiave segreta API.

   ![](assets/image2015-5-4-11-3a16-3a3.png)

   >[!NOTE]
   >
   >I campi seguenti devono essere sincronizzati con Marketo affinché _lead e contatto_ possano funzionare:
   >
   >* Priorità
   >* Urgenza
   >* Punteggio relativo
   >
   >Se manca uno di questi campi, in Marketo verrà visualizzato un messaggio di errore con il nome dei campi mancanti. Per risolvere il problema, eseguire [questa procedura](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. Torna a Dynamics, seleziona **Impostazioni**.

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. Selezionare **Configurazione API Marketo** nella struttura.

   ![](assets/image2015-5-4-11-3a22-3a41.png)

1. Fare clic su **Configurazione predefinita**.

   ![](assets/image2015-5-4-11-3a26-3a10.png)

1. Immetti le informazioni ottenute da Marketo in precedenza.

   ![](assets/image2015-5-4-11-3a27-3a16.png)

1. Fai clic su **Salva**.

   ![](assets/image2015-5-4-11-3a28-3a13.png)

## Imposta accesso utente {#set-user-access}

Imposta i ruoli utente per consentire a utenti specifici di accedere a Sales Insight.

1. Seleziona **Impostazioni**.

   ![](assets/image2015-5-4-11-3a30-3a54.png)

1. Selezionare **Amministrazione** nella struttura.

   ![](assets/image2015-5-4-11-3a31-3a39.png)

1. Fare clic su **Utenti**.

   ![](assets/image2015-5-4-11-3a32-3a25.png)

1. Seleziona gli utenti a cui vuoi concedere l&#39;accesso e fai clic su **Gestisci ruoli**.

   ![](assets/image2015-5-4-11-3a35-3a8.png)

1. Seleziona il ruolo **Marketo Sales Insight** e fai clic su **OK**.

   ![](assets/image2015-5-4-11-3a36-3a59.png)

   Ed è tutto! Tutti gli utenti con accesso potranno ora visualizzare la sezione approfondimenti vendite nella visualizzazione dettagli lead/contatto.

   ![](assets/image2015-5-4-11-3a39-3a23.png)

   Congratulazioni. Ora hai liberato la potenza di Marketo Sales Insight.

>[!MORELIKETHIS]
>
>[Impostazione di stelle e fiamme per record lead/contatti](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
