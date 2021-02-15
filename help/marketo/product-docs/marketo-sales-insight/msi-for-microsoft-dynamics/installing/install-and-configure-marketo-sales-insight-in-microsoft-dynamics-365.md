---
unique-page-id: 3571739
description: Installazione e configurazione di Marketing Sales Insight in Microsoft Dynamics 365 - Marketo Docs - Documentazione prodotto
title: Installazione e configurazione di Marketing Sales Insight in Microsoft Dynamics 365
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 0%

---


# Installazione e configurazione di Marketing Sales Insight in Microsoft Dynamics 365 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo Sales Insight è uno strumento fantastico per dare al vostro team di vendita una &quot;finestra&quot; nella ricchezza di dati di cui dispone il team Marketing. Come installare e configurare.

>[!PREREQUISITES]
>
>Completate l&#39;integrazione tra Marketo e Microsoft.
>
>[Scarica la ](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) soluzione corretta per la versione di Microsoft Dynamics CRM in uso.

## Soluzione di importazione {#import-solution}

1. Accedete a [Microsoft Office 365](https://login.microsoftonline.com/).

   ![](assets/image2015-3-16-15-58-55.png)

1. Fare clic sul menu ![—](assets/image2015-3-16-16-1-13.png) e selezionare **CRM**.

   ![](assets/image2015-3-16-16-0-10.png)

1. Fare clic sul menu ![—](assets/image2015-5-13-10-5-8.png). Nell&#39;elenco a discesa, selezionare **Impostazioni**, quindi selezionare **Soluzioni**.

   ![](assets/image2015-5-13-10-4-1.png)

   >[!NOTE]
   >
   >Prima di procedere, è necessario che [sia già installato e configurato la soluzione Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-1-of-3-install.md).

1. Fare clic su **Importa**.

   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. Nella nuova finestra, fare clic su **Sfoglia**. Scegliere la [Marketing Sales Insight soluzione scaricata nel passaggio 1](#msi). Fare clic su **Next**.

   ![](assets/image2015-5-13-15-3a38-3a49.png)

1. La soluzione verrà caricata. Potete visualizzare il contenuto del pacchetto, se lo desiderate. Fare clic su **Next**.

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. Assicurarsi di lasciare la casella **selezionata** e fare clic su **Importa**.

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. Sentitevi liberi di scaricare il file di registro. Fare clic su **Chiudi**.

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. Fantastico! Dovresti vedere la soluzione ora. Se non è presente, aggiorna lo schermo.

   ![](assets/image2015-5-13-15-3a42-3a29.png)

1. Fate clic su **Pubblica tutte le personalizzazioni**.

   ![](assets/image2015-11-10-11-3a15-3a40.png)

## Connect Marketing e Sales Insight {#connect-marketo-and-sales-insight}

Colleghiamo la tua istanza di Marketo a Sales Insight in Dynamics. Di seguito è riportata la procedura seguente:

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

1. Accedete a Marketo e andate alla sezione **Admin**.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. Nella sezione **Informazioni sulle vendite**, fare clic su **Modifica configurazione API**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Copiate l&#39;**Marketo Host**, **URL API** e l&#39;**ID utente API** per utilizzarlo in un secondo momento. Immettete una **Chiave segreta API** di vostra scelta e fate clic su **Salva**.

   >[!CAUTION]
   >
   >Non utilizzate una e commerciale (&amp;) nella chiave segreta API.

   ![](assets/image2014-12-12-9-3a7-3a9.png)

   >[!NOTE]
   >
   >Per il funzionamento di _Lead e Contact_, è necessario sincronizzare i campi seguenti con Marketo:
   >
   > * Priorità
   > * Urgenza
   > * Punteggio relativo

   >
   >Se manca uno di questi campi, in Marketo verrà visualizzato un messaggio di errore con il nome dei campi mancanti. Per risolvere il problema, eseguire [questa procedura](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. In Microsoft Dynamics, fai clic sull&#39;icona ![](assets/image2015-5-13-15-3a49-3a19.png) accanto a Impostazioni, quindi seleziona **Configurazione API Marketo** nel menu a discesa.

   ![](assets/image2015-5-13-16-3a4-3a1.png)

1. Fare clic su **Configurazione predefinita**.

   ![](assets/image2015-5-13-16-3a5-3a2.png)

1. Inserite le informazioni copiate da Marketo in precedenza.

   ![](assets/image2015-5-13-16-3a7-3a6.png)

1. Fate clic sull&#39;icona ![](assets/image2015-5-13-16-3a8-3a51.png) nell&#39;angolo inferiore destro per salvare le modifiche.

## Imposta accesso utente {#set-user-access}

Devi concedere agli utenti le autorizzazioni per utilizzare Sales Insight.

1. Fare clic sul menu ![](assets/image2015-5-13-10-3a5-3a8.png). Nel menu a discesa selezionare **Impostazioni**, quindi selezionare **Protezione**.

   ![](assets/image2015-5-13-16-3a12-3a12.png)

1. Fare clic su **Utenti**.

   ![](assets/image2015-4-29-14-3a57-3a46.png)

1. Selezionare gli utenti a cui si desidera concedere l&#39;accesso a Sales Insight e fare clic su **Gestisci ruoli**.

   ![](assets/image2015-4-29-14-3a59-3a31.png)

1. Selezionare il ruolo **Marketing Sales Insight** e fare clic su **OK**.

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   E dovreste essere tutti pronti! Infine, per testare, accedi a Dynamics come utente che ha accesso a Marketing Sales Insight e cerca un lead o un contatto.

   ![](assets/image2015-4-29-15-3a2-3a27.png)

Ora hai sbloccato la potenza di Marketing Sales Insight per il tuo team di vendita.

>[!MORELIKETHIS]
>
>[Impostazione di stelle e fiamme per i record lead/contatto](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
