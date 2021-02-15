---
unique-page-id: 37355602
description: Installazione e configurazione di Marketing Sales Insight in Microsoft Dynamics Online - Marketo Docs - Documentazione prodotto
title: Installazione e configurazione di Marketing Sales Insight in Microsoft Dynamics Online
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 0%

---


# Installazione e configurazione di Marketing Sales Insight in Microsoft Dynamics Online {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics-online}

Marketo Sales Insight è uno strumento fantastico per dare al vostro team di vendita una &quot;finestra&quot; nella ricchezza di dati di cui dispone il team Marketing. Come installare e configurare in Microsoft Dynamics Online.

>[!PREREQUISITES]
>
>Completate l&#39;integrazione tra Marketo e Microsoft.
>
>[Scarica la ](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) soluzione corretta per la versione di Microsoft Dynamics CRM in uso.

## Soluzione di importazione {#import-solution}

>[!NOTE]
>
>Se si utilizza l&#39;interfaccia unificata, prima del passaggio 1, fare clic sull&#39;icona Impostazioni nell&#39;angolo superiore destro e selezionare **Impostazioni avanzate**.

1. In Microsoft Dynamics CRM fare clic su **Impostazioni**.

   ![](assets/image2014-12-12-9-3a4-3a56-1.png)

1. In Impostazioni, fate clic su **Personalizzazioni**.

   ![](assets/image2015-4-29-14-3a22-3a1-1.png)

1. Fare clic su **Soluzioni**.

   ![](assets/image2014-12-12-9-3a5-3a17-1.png)

   >[!NOTE]
   >
   >Prima di procedere, avresti già installato e configurato la soluzione Marketo.

1. Fare clic su **Importa**.

   ![](assets/image2014-12-12-9-3a5-3a27-1.png)

1. Nella nuova finestra, fare clic su **Sfoglia**.

   ![](assets/image2014-12-12-9-3a5-3a36-1.png)

1. Sul computer, trovate e installate la soluzione che avete appena scaricato.

1. Fare clic su **Next**.

   ![](assets/seven.png)

1. La soluzione verrà caricata. Potete visualizzare il contenuto del pacchetto, se lo desiderate. Fare clic su **Next**.

   ![](assets/image2014-12-12-9-3a6-3a10-1.png)

1. Assicurarsi di lasciare la casella selezionata e fare clic su **Importa**.

   ![](assets/image2014-12-12-9-3a6-3a19-1.png)

1. Sentitevi liberi di scaricare il file di registro, quindi fate clic su **Chiudi**.

   ![](assets/image2014-12-12-9-3a6-3a29-1.png)

1. Fantastico! Dovresti vedere la soluzione ora. Se non è presente, aggiorna lo schermo.

   ![](assets/eleven.png)

1. Fate clic su **Pubblica personalizzazione**.

   >[!NOTE]
   >
   >Assicuratevi di abilitare la sincronizzazione di Global MS Dynamics.

## Connect Marketing e Sales Insight {#connect-marketo-and-sales-insight}

Colleghiamo la tua istanza di Marketo a Sales Insight in Dynamics. Di seguito viene illustrato come:

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

1. Accedete a Marketo e andate alla sezione **Admin**.

   ![](assets/image2014-12-12-9-3a6-3a50-1.png)

1. Nella sezione Sales Insight, fare clic su **Edit API Configuration**.

   ![](assets/image2014-12-12-9-3a7-3a0-1.png)

1. Copiate l&#39;**Marketo Host**, **URL API** e l&#39;**ID utente API** da utilizzare in un secondo momento. Immettete una chiave segreta API a vostra scelta e fate clic su **Salva**.

   >[!CAUTION]
   >
   >Non utilizzate una e commerciale (&amp;) nella chiave segreta API.

   ![](assets/image2014-12-12-9-3a7-3a9-1.png)

   >[!NOTE]
   >
   >Per il funzionamento di _Lead e Contact_, è necessario sincronizzare i campi seguenti con Marketo:
   >
   >* Priorità
   >* Urgenza
   >* Punteggio relativo

   >
   >Se manca uno di questi campi, in Marketo verrà visualizzato un messaggio di errore con il nome dei campi mancanti. Per risolvere il problema, eseguire [questa procedura](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. In Microsoft Dynamics, passare a **Impostazioni**.

   ![](assets/image2014-12-12-9-3a7-3a25-1.png)

1. In **Impostazioni**, fare clic su **Configurazione API Marketo**.

   ![](assets/image2014-12-12-9-3a7-3a34-1.png)

1. Fare clic su **Nuovo**.

   ![](assets/image2014-12-12-9-3a8-3a8-1.png)

1. Inserite le informazioni da Marketo in precedenza e fate clic su **Salva**.

   ![](assets/image2014-12-12-9-3a8-3a17-1.png)

## Abilita sincronizzazione {#enable-sync}

1. In Marketo, fare clic su **Admin**.

   ![](assets/enable-one.png)

1. In Integrazione, selezionare **Microsoft Dynamics**.

   ![](assets/enable-two.png)

1. Fare clic su **Abilita sincronizzazione**.

   ![](assets/enable-three.png)

1. Fare clic su **Modifica** accanto a Dettagli sincronizzazione campo.

   ![](assets/enable-four.png)

1. In questo modo _automaticamente_ verranno selezionati i campi MSI precedentemente disabilitati (Urgenza, Punteggio relativo e Priorità). È sufficiente fare clic su **Salva** per avviare la sincronizzazione dei dati.

   ![](assets/enable-five.png)

## Imposta accesso utente {#set-user-access}

Infine, è necessario consentire a utenti specifici l&#39;accesso per utilizzare Marketing Cloud Sales Insight.

1. Vai a **Settings**.

   ![](assets/image2014-12-12-9-3a8-3a34-1.png)

1. Vai a **Security**.

   ![](assets/image2015-4-29-14-3a56-3a33-1.png)

1. Fare clic su **Utenti**.

   ![](assets/image2015-4-29-14-3a57-3a46-1.png)

1. Selezionare gli utenti a cui si desidera concedere l&#39;accesso a Sales Insight e fare clic su **Gestisci ruoli**.

   ![](assets/image2015-4-29-14-3a59-3a31-1.png)

1. Selezionare il ruolo Marketing Sales Insight e fare clic su **OK**.

   ![](assets/image2014-12-12-9-3a9-3a22-1.png)

   E dovreste essere tutti pronti! Infine, per testare, accedi a Dynamics come utente che ha accesso a Marketing Sales Insight e cerca un lead o un contatto.

   ![](assets/image2015-4-29-15-3a2-3a27-1.png)

>[!MORELIKETHIS]
>
>[Impostazione di stelle e fiamme per i record lead/contatto](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
