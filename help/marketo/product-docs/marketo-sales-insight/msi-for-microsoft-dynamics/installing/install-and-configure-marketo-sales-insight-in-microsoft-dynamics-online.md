---
unique-page-id: 37355602
description: Installare e configurare Marketo Sales Insight in Microsoft Dynamics Online - Documentazione di Marketo - Documentazione del prodotto
title: Installare e configurare Marketo Sales Insight in Microsoft Dynamics Online
exl-id: 3b58b109-96f9-427e-be5c-a8db270ffe69
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 0%

---

# Installare e configurare Marketo Sales Insight in Microsoft Dynamics Online {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics-online}

Marketo Sales Insight è uno strumento fantastico per dare al vostro team di vendita una &quot;finestra&quot; sulla ricchezza di dati che il team di marketing ha. Di seguito viene illustrato come installarlo e configurarlo in Microsoft Dynamics Online.

>[!PREREQUISITES]
>
>Completa l&#39;integrazione Marketo-Microsoft.
>
>[Scaricare la soluzione corretta](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) per la versione di Microsoft Dynamics CRM in uso.

## Importa soluzione {#import-solution}

>[!NOTE]
>
>Se utilizzi l’interfaccia unificata, prima del passaggio 1 di seguito, fai clic sull’icona Impostazioni in alto a destra e seleziona **Impostazioni avanzate**.

1. In Microsoft Dynamics CRM, fai clic su **Impostazioni**.

   ![](assets/image2014-12-12-9-3a4-3a56-1.png)

1. In Impostazioni, fai clic su **Personalizzazioni**.

   ![](assets/image2015-4-29-14-3a22-3a1-1.png)

1. Clic **Soluzioni**.

   ![](assets/image2014-12-12-9-3a5-3a17-1.png)

   >[!NOTE]
   >
   >Prima di procedere, dovreste aver già installato e configurato la soluzione Marketo.

1. Clic **Importa**.

   ![](assets/image2014-12-12-9-3a5-3a27-1.png)

1. Nella nuova finestra, fai clic su **Sfoglia**.

   ![](assets/image2014-12-12-9-3a5-3a36-1.png)

1. Nel computer, individuare e installare la soluzione appena scaricata.

1. Clic **Successivo**.

   ![](assets/seven.png)

1. La soluzione verrà caricata. Puoi visualizzare il contenuto del pacchetto, se lo desideri. Clic **Successivo**.

   ![](assets/image2014-12-12-9-3a6-3a10-1.png)

1. Assicurati di lasciare selezionata la casella e fai clic su **Importa**.

   ![](assets/image2014-12-12-9-3a6-3a19-1.png)

1. Puoi scaricare il file di registro, quindi fai clic su **Chiudi**.

   ![](assets/image2014-12-12-9-3a6-3a29-1.png)

1. Fantastico! Dovresti vedere la soluzione ora. Se non è presente, aggiorna lo schermo.

   ![](assets/eleven.png)

1. Clic **Personalizzazione pubblicazione**.

   >[!NOTE]
   >
   >Assicurati di abilitare la sincronizzazione globale di MS Dynamics.

## Connettere Marketo e Sales Insight {#connect-marketo-and-sales-insight}

Colleghiamo la tua istanza di Marketo a Sales Insight in Dynamics. Ecco come:

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

1. Accedi a Marketo e passa a **Amministratore** sezione.

   ![](assets/image2014-12-12-9-3a6-3a50-1.png)

1. Nella sezione Sales Insight (Approfondimenti sulla vendita), fai clic su **Modifica configurazione API**.

   ![](assets/image2014-12-12-9-3a7-3a0-1.png)

1. Copia il **Host Marketo**, **URL API**, e **ID utente API** da utilizzare in un passaggio successivo. Immetti una chiave segreta API a tua scelta e fai clic su **Salva**.

   >[!CAUTION]
   >
   >Non utilizzare una e commerciale (&amp;) nella chiave segreta API.

   ![](assets/image2014-12-12-9-3a7-3a9-1.png)

   >[!NOTE]
   >
   >I seguenti campi devono essere sincronizzati con Marketo per _lead e contatto_ per il corretto funzionamento di Sales Insight:
   >
   >* Priorità
   >* Urgenza
   >* Punteggio relativo
   >
   >Se manca uno di questi campi, in Marketo verrà visualizzato un messaggio di errore con il nome dei campi mancanti. Per risolvere questo problema, esegui [questa procedura](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. Torna a Microsoft Dynamics, vai a **Impostazioni**.

   ![](assets/image2014-12-12-9-3a7-3a25-1.png)

1. Sotto **Impostazioni**, fai clic su **Configurazione API Marketo**.

   ![](assets/image2014-12-12-9-3a7-3a34-1.png)

1. Clic **Nuovo**.

   ![](assets/image2014-12-12-9-3a8-3a8-1.png)

1. Immetti le informazioni ottenute da Marketo in precedenza e fai clic su **Salva**.

   ![](assets/image2014-12-12-9-3a8-3a17-1.png)

## Abilita sincronizzazione {#enable-sync}

1. In Marketo, fai clic su **Amministratore**.

   ![](assets/enable-one.png)

1. In Integrazione, seleziona **Microsoft Dynamics**.

   ![](assets/enable-two.png)

1. Clic **Abilita sincronizzazione**.

   ![](assets/enable-three.png)

1. Clic **Modifica** accanto a Dettagli sincronizzazione campi.

   ![](assets/enable-four.png)

1. Questo _automaticamente_ selezionare i campi MSI precedentemente disabilitati (Urgenza, Punteggio relativo e Priorità). Fai clic su **Salva** per avviare la sincronizzazione dei dati.

   ![](assets/enable-five.png)

## Imposta accesso utente {#set-user-access}

Infine, devi fornire a utenti specifici l’accesso per utilizzare Marketo Sales Insight.

1. Vai a **Impostazioni**.

   ![](assets/image2014-12-12-9-3a8-3a34-1.png)

1. Vai a **Sicurezza**.

   ![](assets/image2015-4-29-14-3a56-3a33-1.png)

1. Clic **Utenti**.

   ![](assets/image2015-4-29-14-3a57-3a46-1.png)

1. Seleziona gli utenti a cui vuoi dare accesso a Sales Insight e fai clic su **Gestisci ruoli**.

   ![](assets/image2015-4-29-14-3a59-3a31-1.png)

1. Seleziona il ruolo Marketo Sales Insight e fai clic su **OK**.

   ![](assets/image2014-12-12-9-3a9-3a22-1.png)

   E dovreste aver finito! Infine, per eseguire il test, accedi a Dynamics come utente che ha accesso a Marketo Sales Insight e controlla un lead o un contatto.

   ![](assets/image2015-4-29-15-3a2-3a27-1.png)

>[!MORELIKETHIS]
>
>[Impostazione di stelle e fiamme per record lead/contatti](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
