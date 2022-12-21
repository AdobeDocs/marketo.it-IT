---
unique-page-id: 37355602
description: Installare e configurare Marketo Sales Insight in Microsoft Dynamics Online - Documentazione di Marketo - Documentazione del prodotto
title: Installazione e configurazione di Marketo Sales Insight in Microsoft Dynamics Online
exl-id: 3b58b109-96f9-427e-be5c-a8db270ffe69
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 0%

---

# Installazione e configurazione di Marketo Sales Insight in Microsoft Dynamics Online {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics-online}

Marketo Sales Insight è uno strumento fantastico per dare al tuo team di vendita una &quot;finestra&quot; nella ricchezza di dati di cui dispone il team Marketing. Come installarlo e configurarlo in Microsoft Dynamics Online.

>[!PREREQUISITES]
>
>Completa l’integrazione Marketo-Microsoft.
>
>[Scarica la soluzione corretta](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) per la tua versione di Microsoft Dynamics CRM.

## Soluzione di importazione {#import-solution}

>[!NOTE]
>
>Se utilizzi l’interfaccia unificata, prima del passaggio 1, fai clic sull’icona Impostazioni nell’angolo in alto a destra e seleziona **Impostazioni avanzate**.

1. Fai clic su Microsoft Dynamics CRM **Impostazioni**.

   ![](assets/image2014-12-12-9-3a4-3a56-1.png)

1. In Impostazioni, fai clic su **Personalizzazioni**.

   ![](assets/image2015-4-29-14-3a22-3a1-1.png)

1. Fai clic su **Soluzioni**.

   ![](assets/image2014-12-12-9-3a5-3a17-1.png)

   >[!NOTE]
   >
   >Prima di procedere, dovresti aver già installato e configurato la soluzione Marketo.

1. Fai clic su **Importa**.

   ![](assets/image2014-12-12-9-3a5-3a27-1.png)

1. Nella nuova finestra, fai clic su **Sfoglia**.

   ![](assets/image2014-12-12-9-3a5-3a36-1.png)

1. Sul computer, trovare e installare la soluzione appena scaricata.

1. Fai clic su **Successivo**.

   ![](assets/seven.png)

1. La soluzione verrà caricata. Puoi visualizzare il contenuto del pacchetto, se lo desideri. Fai clic su **Successivo**.

   ![](assets/image2014-12-12-9-3a6-3a10-1.png)

1. Assicurati di lasciare selezionata la casella e fai clic su **Importa**.

   ![](assets/image2014-12-12-9-3a6-3a19-1.png)

1. Sentitevi liberi di scaricare il file di log, quindi fai clic su **Chiudi**.

   ![](assets/image2014-12-12-9-3a6-3a29-1.png)

1. Fantastico! Dovresti vedere la soluzione ora. Se non è presente, aggiorna lo schermo.

   ![](assets/eleven.png)

1. Fai clic su **Personalizzazione della pubblicazione**.

   >[!NOTE]
   >
   >Assicurati di abilitare la sincronizzazione di Global MS Dynamics.

## Collegare Marketo e Sales Insight {#connect-marketo-and-sales-insight}

Colleghiamo la tua istanza Marketo a Sales Insight in Dynamics. Ecco come:

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

1. Accedi a Marketo e vai a **Amministratore** sezione .

   ![](assets/image2014-12-12-9-3a6-3a50-1.png)

1. Nella sezione Approfondimenti vendite fare clic su **Modifica configurazione API**.

   ![](assets/image2014-12-12-9-3a7-3a0-1.png)

1. Copia il **Host Marketo**, **URL API** e **ID utente API** da utilizzare in un passaggio successivo. Immetti una chiave segreto API a tua scelta e fai clic su **Salva**.

   >[!CAUTION]
   >
   >Non utilizzare una e commerciale (&amp;) nella chiave segreto API.

   ![](assets/image2014-12-12-9-3a7-3a9-1.png)

   >[!NOTE]
   >
   >I campi seguenti devono essere sincronizzati con Marketo per _lead e contatti_ per il funzionamento di Sales Insight:
   >
   >* Priorità
   >* Urgenza
   >* Punteggio relativo

   >
   >Se manca uno di questi campi, in Marketo verrà visualizzato un messaggio di errore con il nome dei campi mancanti. Per risolvere il problema, esegui [presente procedura](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. Torna a Microsoft Dynamics **Impostazioni**.

   ![](assets/image2014-12-12-9-3a7-3a25-1.png)

1. Sotto **Impostazioni**, fai clic su **Configurazione API Marketo**.

   ![](assets/image2014-12-12-9-3a7-3a34-1.png)

1. Fai clic su **Nuovo**.

   ![](assets/image2014-12-12-9-3a8-3a8-1.png)

1. Immetti le informazioni acquisite in precedenza da Marketo e fai clic su **Salva**.

   ![](assets/image2014-12-12-9-3a8-3a17-1.png)

## Abilita sincronizzazione {#enable-sync}

1. In Marketo, fai clic su **Amministratore**.

   ![](assets/enable-one.png)

1. In Integrazione, seleziona **Microsoft Dynamics**.

   ![](assets/enable-two.png)

1. Fai clic su **Abilita sincronizzazione**.

   ![](assets/enable-three.png)

1. Fai clic su **Modifica** accanto a Dettagli sincronizzazione campi.

   ![](assets/enable-four.png)

1. Questo _automaticamente_ selezionare i campi MSI precedentemente disabilitati (Urgenza, Punteggio relativo e Priorità). Fai clic su **Salva** per avviare la sincronizzazione dei dati.

   ![](assets/enable-five.png)

## Imposta accesso utente {#set-user-access}

Infine, è necessario consentire a utenti specifici l&#39;accesso per utilizzare Marketo Sales Insight.

1. Vai a **Impostazioni**.

   ![](assets/image2014-12-12-9-3a8-3a34-1.png)

1. Vai a **Sicurezza**.

   ![](assets/image2015-4-29-14-3a56-3a33-1.png)

1. Fai clic su **Utenti**.

   ![](assets/image2015-4-29-14-3a57-3a46-1.png)

1. Selezionare gli utenti a cui si desidera accedere a Informazioni sulle vendite e fare clic su **Gestisci ruoli**.

   ![](assets/image2015-4-29-14-3a59-3a31-1.png)

1. Selezionare il ruolo Marketo Sales Insight e fare clic su **OK**.

   ![](assets/image2014-12-12-9-3a9-3a22-1.png)

   E dovreste essere tutti fatti! Infine, per testare, accedi a Dynamics come utente con accesso a Marketo Sales Insight e cerca un lead o un contatto.

   ![](assets/image2015-4-29-15-3a2-3a27-1.png)

>[!MORELIKETHIS]
>
>[Impostazione di stelle e fiamme per i record lead/contatti](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
