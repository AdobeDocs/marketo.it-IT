---
unique-page-id: 3571739
description: Installare e configurare Marketo Sales Insight in Microsoft Dynamics 365 - Documenti Marketo - Documentazione del prodotto
title: Installare e configurare Marketo Sales Insight in Microsoft Dynamics 365
exl-id: c1f06b8c-48fd-4015-9502-7c9693632589
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '462'
ht-degree: 0%

---

# Installare e configurare Marketo Sales Insight in Microsoft Dynamics 365 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo Sales Insight è uno strumento fantastico per dare al vostro team di vendita una &quot;finestra&quot; sulla ricchezza di dati che il team di marketing ha. Ecco come installare e configurare.

>[!PREREQUISITES]
>
>Completa l&#39;integrazione Marketo-Microsoft.
>
>[Scarica la soluzione corretta](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) per la versione di Microsoft Dynamics CRM in uso.

## Importa soluzione {#import-solution}

1. Accedere a [Microsoft Office 365](https://login.microsoftonline.com/).

   ![](assets/image2015-3-16-15-58-55.png)

1. Fare clic sul menu ![—](assets/image2015-3-16-16-1-13.png) e selezionare **CRM**.

   ![](assets/image2015-3-16-16-0-10.png)

1. Fare clic sul menu ![—](assets/image2015-5-13-10-5-8.png). Nel menu a discesa, seleziona **Impostazioni**, quindi seleziona **Soluzioni**.

   ![](assets/image2015-5-13-10-4-1.png)

   >[!NOTE]
   >
   >Prima di procedere, dovresti avere già installato [e configurato la soluzione Marketo](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/microsoft-dynamics-365-with-ropc-connection/step-1-of-4-install.md).

1. Fai clic su **Importa**.

   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. Nella nuova finestra, fai clic su **Sfoglia**. Scegliere la [soluzione Marketo Sales Insight scaricata al passaggio 1](#msi). Fai clic su **Avanti**.

   ![](assets/image2015-5-13-15-3a38-3a49.png)

1. La soluzione verrà caricata. Puoi visualizzare il contenuto del pacchetto, se lo desideri. Fai clic su **Avanti**.

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. Assicurati di lasciare la casella **selezionata** e fai clic su **Importa**.

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. Scarica il file di registro. Fai clic su **Chiudi**.

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. Fantastico! Dovresti vedere la soluzione ora. Se non è presente, aggiorna lo schermo.

   ![](assets/image2015-5-13-15-3a42-3a29.png)

1. Fare clic su **Publish tutte le personalizzazioni**.

   ![](assets/image2015-11-10-11-3a15-3a40.png)

## Connettere Marketo e Sales Insight {#connect-marketo-and-sales-insight}

Colleghiamo la tua istanza di Marketo a Sales Insight in Dynamics. Ecco come:

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

1. Accedi a Marketo e passa alla sezione **Admin**.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. Nella sezione **Informazioni sulle vendite**, fai clic su **Modifica configurazione API**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Copiare l&#39;**host Marketo**, l&#39;**URL API** e l&#39;**ID utente API** da utilizzare in un passaggio successivo. Immetti una **chiave segreta API** a tua scelta e fai clic su **Salva**.

   >[!CAUTION]
   >
   >Non utilizzare una e commerciale (&amp;) nella chiave segreta API.

   ![](assets/image2014-12-12-9-3a7-3a9.png)

   >[!NOTE]
   >
   >I campi seguenti devono essere sincronizzati con Marketo affinché _lead e contatto_ possano funzionare:
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

1. Immetti le informazioni copiate in precedenza da Marketo.

   ![](assets/image2015-5-13-16-3a7-3a6.png)

1. Fai clic sull&#39;icona ![](assets/image2015-5-13-16-3a8-3a51.png) nell&#39;angolo in basso a destra per salvare le modifiche.

## Imposta accesso utente {#set-user-access}

È necessario concedere agli utenti le autorizzazioni per utilizzare Sales Insight.

1. Fare clic sul menu ![](assets/image2015-5-13-10-3a5-3a8.png). Nel menu a discesa, seleziona **Impostazioni**, quindi seleziona **Sicurezza**.

   ![](assets/image2015-5-13-16-3a12-3a12.png)

1. Fare clic su **Utenti**.

   ![](assets/image2015-4-29-14-3a57-3a46.png)

1. Seleziona gli utenti a cui vuoi concedere l&#39;accesso a Sales Insight e fai clic su **Gestisci ruoli**.

   ![](assets/image2015-4-29-14-3a59-3a31.png)

1. Seleziona il ruolo **Marketo Sales Insight** e fai clic su **OK**.

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   E dovreste aver finito! Infine, per eseguire il test, accedi a Dynamics come utente che ha accesso a Marketo Sales Insight e controlla un lead o un contatto.

   ![](assets/image2015-4-29-15-3a2-3a27.png)

Ora hai sbloccato la potenza di Marketo Sales Insight per il tuo team di vendita.

>[!MORELIKETHIS]
>
>[Impostazione di stelle e fiamme per record lead/contatti](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
