---
unique-page-id: 3571739
description: Installazione e configurazione di Marketing Sales Insight in Microsoft Dynamics 365 - Marketo Docs - Documentazione prodotto
title: Installazione e configurazione di Marketing Sales Insight in Microsoft Dynamics 365
translation-type: tm+mt
source-git-commit: dc20aede0894a09e6c0bcd3d1580859b5fecb5f1
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 0%

---


# Installazione e configurazione di Marketing Sales Insight in Microsoft Dynamics 365 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo Sales Insight è uno strumento fantastico per dare al vostro team di vendita una &quot;finestra&quot; nella ricchezza di dati di cui dispone il team Marketing. Come installare e configurare.

>[!NOTE]
>
>**Prerequisiti**
>
>Completate l&#39;integrazione con [Marketo-Microsoft](http://docs.marketo.com/x/E4A2).
>
>[Scarica la soluzione](http://docs.marketo.com/x/LoJo) corretta per la versione di Microsoft Dynamics CRM in uso.

## Soluzione di importazione {#import-solution}

1. Accedete a [Microsoft Office 365](https://login.microsoftonline.com/).

   ![](assets/image2015-3-16-15-58-55.png)

1. Fare clic sul ![—](assets/image2015-3-16-16-1-13.png) menu e selezionare **CRM**.

   ![](assets/image2015-3-16-16-0-10.png)

1. Fare clic sul ![—](assets/image2015-5-13-10-5-8.png) menu. Nell&#39;elenco a discesa, selezionate **Impostazioni**, quindi selezionate **Soluzioni**.

   ![](assets/image2015-5-13-10-4-1.png)

   >[!NOTE]
   >
   >**Promemoria**
   >
   >
   >Prima di procedere, dovresti aver già [installato e configurato la soluzione](../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365/step-1-of-3-install.md) Marketo.

   Fate clic su Importa.
   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. Nella nuova finestra, fate clic su **Sfoglia**. Scegli la soluzione [Marketing Sales Insight che hai scaricato al passaggio 1](#msi). Fate clic su **Avanti**.

   ![](assets/image2015-5-13-15-3a38-3a49.png)

1. La soluzione verrà caricata. Potete visualizzare il contenuto del pacchetto, se lo desiderate. Fate clic su **Avanti**.

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. Accertatevi di lasciare la casella **selezionata** e di fare clic su **Importa**.

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. Sentitevi liberi di scaricare il file di registro. Fate clic su **Chiudi**.

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

1. Accedi a Marketo e vai alla sezione **Admin** .

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. Nella sezione **Sales Insight** , fate clic su **Edit API Configuration**(Modifica configurazione API).

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Copiate l&#39;host **** Marketo, l&#39;URL **** API e l&#39;ID **utente** API da utilizzare in un secondo momento. Immettete una chiave **Segreto** API di vostra scelta e fate clic su **SALVA**.

   >[!CAUTION]
   >
   >Non utilizzate una e commerciale (&amp;) nella chiave segreta API.

   ![](assets/image2014-12-12-9-3a7-3a9.png)

   >[!NOTE]
   >
   >Per il funzionamento di *Lead e Contact* for Sales Insight, è necessario sincronizzare i campi seguenti con Marketo:
   >
   > * Priorità
   > * Urgenza
   > * Punteggio relativo

   >
   >Se manca uno di questi campi, in Marketo verrà visualizzato un messaggio di errore con il nome dei campi mancanti. Per risolvere il problema, eseguire [questa procedura](../../../../product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. In Microsoft Dynamics, fai clic sull&#39; ![](assets/image2015-5-13-15-3a49-3a19.png) icona accanto a Impostazioni, quindi seleziona Configurazione **API** Marketo nel menu a discesa.

   ![](assets/image2015-5-13-16-3a4-3a1.png)

1. Fate clic su Configurazione **** predefinita.

   ![](assets/image2015-5-13-16-3a5-3a2.png)

1. Inserite le informazioni copiate da Marketo in precedenza.

   ![](assets/image2015-5-13-16-3a7-3a6.png)

1. Fate clic sull’ ![](assets/image2015-5-13-16-3a8-3a51.png) icona nell’angolo in basso a destra per salvare le modifiche.

## Imposta accesso utente {#set-user-access}

Devi concedere agli utenti le autorizzazioni per utilizzare Sales Insight.

1. Fare clic sul ![](assets/image2015-5-13-10-3a5-3a8.png) menu. Nel menu a discesa selezionate **Impostazioni**, quindi selezionate **Protezione**.

   ![](assets/image2015-5-13-16-3a12-3a12.png)

1. Fate clic su **Utenti**.

   ![](assets/image2015-4-29-14-3a57-3a46.png)

1. Selezionare gli utenti a cui si desidera accedere a Informazioni sulle vendite e fare clic su **Gestisci ruoli**.

   ![](assets/image2015-4-29-14-3a59-3a31.png)

1. Selezionate il ruolo **Visione** vendite marketing e fate clic su **OK**.

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   E dovreste essere tutti pronti! Infine, per testare, accedi a Dynamics come utente che ha accesso a Marketing Sales Insight e cerca un lead o un contatto.

   ![](assets/image2015-4-29-15-3a2-3a27.png)

Ora hai sbloccato la potenza di Marketing Sales Insight per il tuo team di vendita.

>[!NOTE]
>
>**Articoli correlati**
>
>[Impostazione di stelle e fiamme per i record lead/contatto](http://docs.marketo.com/x/BICMAg)