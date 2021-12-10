---
unique-page-id: 3571735
description: Installare e configurare Marketo Sales Insight in Microsoft Dynamics 2011 - Documentazione di Marketo - Documentazione del prodotto
title: Installazione e configurazione di Marketo Sales Insight in Microsoft Dynamics 2011
exl-id: 40622dcc-7129-4392-95dc-ca829c15c3a6
source-git-commit: fda1bf51d4016a61c41be9acba4771db1797a552
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 0%

---

# Installazione e configurazione di Marketo Sales Insight in Microsoft Dynamics 2011 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo Sales Insight è uno strumento fantastico per il tuo team di vendita. Di seguito sono riportate le istruzioni dettagliate su come installarlo e configurarlo in Microsoft Dynamics 2011 On-Premises.

>[!PREREQUISITES]
>
>Completa l’integrazione Marketo-Microsoft.
>
>[Scarica la soluzione corretta](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) per la tua versione di Microsoft Dynamics CRM.

## Soluzione di importazione {#import-solution}

1. Accesso a Microsoft Dynamics CRM. Fai clic su **Impostazioni** nel menu in basso a sinistra.

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. Seleziona **Soluzioni** nell&#39;albero.

   ![](assets/image2015-5-4-10-3a41-3a56.png)

1. Fai clic su **Importa** ( ![](assets/image2015-5-4-10-3a45-3a44.png)).

   ![](assets/image2015-5-4-10-3a42-3a38.png)

   >[!NOTE]
   >
   >Dovresti già avere [installati e configurati](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-2011.md) la soluzione Marketo prima di procedere.

1. Fai clic su **Sfoglia**. Selezionare la soluzione Marketo Sales Insight [scaricato](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md). Fai clic su **Successivo**.

   ![](assets/image2015-5-4-10-3a55-3a15.png)

1. Verifica i dettagli della soluzione e fai clic su **Successivo**.

   ![](assets/image2015-5-4-10-3a57-3a31.png)

1. Assicurati che l&#39;opzione Messaggio SDK sia selezionata. Fai clic su **Successivo**.

   ![](assets/image2015-5-4-11-3a43-3a37.png)

1. Ora attendi il completamento dell’importazione.

   ![](assets/image2015-5-4-11-3a0-3a58.png)

1. Fai clic su **Chiudi**.

   ![](assets/crmhand.png)

1. Marketo Sales Insight verrà visualizzato nell’elenco delle soluzioni. Yay!

   ![](assets/image2015-5-4-11-3a2-3a37.png)

1. Selezionare Marketo Sales Insight e fare clic su **Pubblica tutte le personalizzazioni** ( ![](assets/image2015-5-4-11-3a7-3a8.png)).

   ![](assets/image2015-5-4-11-3a8-3a27.png)

## Collegare Marketo e Sales Insight  {#connect-marketo-and-sales-insight}

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

1. Accedi a Marketo e fai clic su **Amministratore**.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. Sotto la **Approfondimenti vendite** clic sulla sezione **Modifica configurazione API**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Copia il **Host Marketo**, **URL API** e **ID utente API** da utilizzare in un passaggio successivo. Inserisci un **Chiave segreta API** di tua scelta e fai clic su **Salva**.

   >[!CAUTION]
   >
   >Non utilizzare una e commerciale (&amp;) nella chiave segreto API.

   ![](assets/image2015-5-4-11-3a16-3a3.png)

   >[!NOTE]
   >
   >I campi seguenti devono essere sincronizzati con Marketo per _lead e contatti_ per il funzionamento di Sales Insight:
   >
   >* Priorità
   >* Urgenza
   >* Punteggio relativo

   >
   >Se manca uno di questi campi, in Marketo verrà visualizzato un messaggio di errore con il nome dei campi mancanti. Per risolvere il problema, esegui [presente procedura](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. Torna a Dynamics, seleziona **Impostazioni**.

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. Seleziona **Configurazione API Marketo** nell&#39;albero.

   ![](assets/image2015-5-4-11-3a22-3a41.png)

1. Fai clic su **Configurazione predefinita**.

   ![](assets/image2015-5-4-11-3a26-3a10.png)

1. Immetti le informazioni che hai preso in precedenza da Marketo.

   ![](assets/image2015-5-4-11-3a27-3a16.png)

1. Fai clic su **Salva**.

   ![](assets/image2015-5-4-11-3a28-3a13.png)

## Imposta accesso utente {#set-user-access}

Imposta i ruoli utente per consentire agli utenti specifici di accedere a Sales Insight.

1. Seleziona **Impostazioni**.

   ![](assets/image2015-5-4-11-3a30-3a54.png)

1. Seleziona **Amministrazione** nell&#39;albero.

   ![](assets/image2015-5-4-11-3a31-3a39.png)

1. Fai clic su **Utenti**.

   ![](assets/image2015-5-4-11-3a32-3a25.png)

1. Seleziona gli utenti a cui desideri concedere l’accesso e fai clic su **Gestisci ruoli**.

   ![](assets/image2015-5-4-11-3a35-3a8.png)

1. Seleziona la **Informazioni sulle vendite Marketo** ruolo e clic **OK**.

   ![](assets/image2015-5-4-11-3a36-3a59.png)

   Ed è tutto! Ora tutti gli utenti con accesso potranno visualizzare la sezione approfondimenti sulle vendite nella vista dettagli lead/contatti.

   ![](assets/image2015-5-4-11-3a39-3a23.png)

   Congratulazioni. Ora hai liberato la potenza di Marketo Sales Insight.

>[!MORELIKETHIS]
>
>[Impostazione di stelle e fiamme per i record lead/contatti](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
