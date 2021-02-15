---
unique-page-id: 3571737
description: Installazione e configurazione di Marketing Sales Insight in Microsoft Dynamics 2013 - Marketo Docs - Documentazione prodotto
title: Installazione e configurazione di Marketing Sales Insight in Microsoft Dynamics 2013
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---


# Installazione e configurazione di Marketing Sales Insight in Microsoft Dynamics 2013 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo Sales Insight è uno strumento fantastico per dare al vostro team di vendita una &quot;finestra&quot; nella ricchezza di dati di cui dispone il team di marketing. Ecco come installarlo e configurarlo.

>[!PREREQUISITES]
>
>Completate l&#39;integrazione tra Marketo e Microsoft.
>
>[Scarica la ](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) soluzione corretta per la versione di Microsoft Dynamics CRM in uso.

## Soluzione di importazione {#import-solution}

OK, ora è ora di importare la soluzione Marketing to Sales Insight in Microsoft Dynamics.

1. In **Microsoft Dynamics CRM** fare clic su **Impostazioni**.

   ![](assets/image2014-12-12-9-3a4-3a56.png)

1. In **Impostazioni**, fare clic su **Personalizzazioni**.

   ![](assets/image2014-12-12-9-3a5-3a6.png)

1. Fare clic su **Soluzioni**.

   ![](assets/image2014-12-12-9-3a5-3a17.png)

   >[!NOTE]
   >
   >Prima di procedere, dovresti già avere installato e configurato Marketo

1. Fare clic su **Importa**.

   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. Nella nuova finestra, fare clic su **Sfoglia**.

   ![](assets/image2014-12-12-9-3a5-3a36.png)

1. Trova e seleziona la soluzione che hai scaricato sopra.

   ![](assets/image2014-12-12-9-3a5-3a45.png)

1. Fare clic su **Next**.

   ![](assets/image2014-12-12-9-3a5-3a55.png)

1. La soluzione verrà caricata. Potete visualizzare il contenuto del pacchetto, se lo desiderate. Fare clic su **Next**.

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. Assicurarsi di lasciare la casella selezionata e fare clic su **Importa**.

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. Sentitevi liberi di scaricare il file di registro. Fare clic su **Chiudi**.

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. Fantastico! Dovresti vedere la soluzione ora. Se non è presente, aggiorna lo schermo.

   ![](assets/image2014-12-12-9-3a6-3a40.png)

## Connect Marketing e Sales Insight {#connect-marketo-and-sales-insight}

Colleghiamo la tua istanza di Marketo a Sales Insight in Dynamics.

>[!NOTE]
>
>Diritti di amministratore richiesti.

1. Accedete a Marketo e andate alla sezione **Admin**.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. Nella sezione **Sales Insight** fare clic su **Edit API Configuration** (Modifica configurazione API).

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Copiate l&#39;**Marketo Host**, **URL API** e l&#39;**ID utente API** da utilizzare in un secondo momento. Immettete una **Chiave segreta API** di vostra scelta e fate clic su **Salva**.

   >[!CAUTION]
   >
   >Non utilizzate una e commerciale (&amp;) nella chiave segreta API.

   ![](assets/image2014-12-12-9-3a7-3a9.png)

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

   ![](assets/image2014-12-12-9-3a7-3a25.png)

1. In **Impostazioni**, fare clic su **Configurazione API Marketo**.

   ![](assets/image2014-12-12-9-3a7-3a34.png)

1. Fare clic su **Nuovo**.

   ![](assets/image2014-12-12-9-3a8-3a8.png)

1. Inserite le informazioni da Marketo in precedenza e fate clic su **Salva**.

   ![](assets/image2014-12-12-9-3a8-3a17.png)

## Imposta accesso utente {#set-user-access}

Infine, puoi consentire a utenti specifici di accedere a Marketing Cloud Sales Insight.

1. Vai a **Settings**.

   ![](assets/image2014-12-12-9-3a8-3a34.png)

1. Fare clic su **Utenti**.

   ![](assets/image2014-12-12-9-3a8-3a42.png)

1. Selezionare gli utenti a cui si desidera concedere l&#39;accesso a Sales Insight e fare clic su **Gestisci ruoli**.

   ![](assets/image2014-12-12-9-3a9-3a13.png)

1. Selezionare il ruolo **Marketing Sales Insight** e fare clic su **OK**.

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   E dovreste essere tutti pronti! Infine, per eseguire il test, accedi a Dynamics come utente che ha accesso a Marketing Sales Insight e cerca un lead o un contatto.

   ![](assets/image2014-12-12-9-3a9-3a31.png)

Ora hai sbloccato la potenza di Marketing Sales Insight per il tuo team di vendita.

>[!MORELIKETHIS]
>
>[Impostazione di stelle e fiamme per i record lead/contatto](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
