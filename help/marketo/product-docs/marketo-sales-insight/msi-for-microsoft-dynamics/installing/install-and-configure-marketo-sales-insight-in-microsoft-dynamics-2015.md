---
unique-page-id: 7513865
description: Installare e configurare Marketo Sales Insight in Microsoft Dynamics 2015 - Documentazione di Marketo - Documentazione del prodotto
title: Installazione e configurazione di Marketo Sales Insight in Microsoft Dynamics 2015
exl-id: 26c1f02c-c910-445d-8560-0b37961eadcb
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '442'
ht-degree: 0%

---

# Installazione e configurazione di Marketo Sales Insight in Microsoft Dynamics 2015 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo Sales Insight è uno strumento fantastico per dare al tuo team di vendita una &quot;finestra&quot; nella ricchezza di dati di cui dispone il team Marketing. Come installarlo e configurarlo in Microsoft Dynamics 201

>[!PREREQUISITES]
>
>Completa l’integrazione Marketo-Microsoft.
>
>[Scarica la soluzione corretta](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) per la tua versione di Microsoft Dynamics CRM.

## Soluzione di importazione {#import-solution}

OK, ora è il momento di importare la soluzione Marketo Sales Insight in Microsoft Dynamics. Ecco come:

1. Fai clic su Microsoft Dynamics CRM **Impostazioni**.

   ![](assets/image2014-12-12-9-3a4-3a56.png)

1. In IMPOSTAZIONI, fai clic su **Personalizzazioni**.

   ![](assets/image2015-4-29-14-3a22-3a1.png)

1. Fai clic su **Soluzioni**.

   ![](assets/image2014-12-12-9-3a5-3a17.png)

   >[!NOTE]
   >
   >Prima di procedere, dovresti aver già installato e configurato la soluzione Marketo.

1. Fai clic su **Importa**.

   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. Nella nuova finestra, fai clic su **Sfoglia**.

   ![](assets/image2014-12-12-9-3a5-3a36.png)

1. Trova e seleziona la soluzione scaricata in precedenza.

   ![](assets/image2014-12-12-9-3a5-3a45.png)

1. Fai clic su **Successivo**.

   ![](assets/image2014-12-12-9-3a5-3a55.png)

1. La soluzione verrà caricata. Puoi visualizzare il contenuto del pacchetto, se lo desideri. Fai clic su **Successivo**.

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. Assicurati di lasciare selezionata la casella e fai clic su **Importa**.

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. Sentitevi liberi di scaricare il file di log, quindi fai clic su **Chiudi**.

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. Fantastico! Dovresti vedere la soluzione ora. Se non è presente, aggiorna lo schermo.

   ![](assets/image2014-12-12-9-3a6-3a40.png)

## Collegare Marketo e Sales Insight {#connect-marketo-and-sales-insight}

Colleghiamo la tua istanza Marketo a Sales Insight in Dynamics. Ecco come:

>[!NOTE]
>
>Sono richiesti i diritti di amministratore.

1. Accedi a Marketo e vai a **Amministratore** sezione .

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. Nella sezione Approfondimenti vendite fare clic su **Modifica configurazione API**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Copia il **Host Marketo**, **URL API** e **ID utente API** da utilizzare in un passaggio successivo. Immetti una chiave segreto API a tua scelta e fai clic su **Salva**.

   >[!CAUTION]
   >
   >Non utilizzare una e commerciale (&amp;) nella chiave segreto API.

   ![](assets/image2014-12-12-9-3a7-3a9.png)

   >[!NOTE]
   >
   >I campi seguenti devono essere sincronizzati con Marketo per *lead e contatti* per il funzionamento di Sales Insight:
   >
   >* Priorità
   >* Urgenza
   >* Punteggio relativo

   >
   >Se manca uno di questi campi, in Marketo verrà visualizzato un messaggio di errore con il nome dei campi mancanti. Per risolvere il problema, esegui [presente procedura](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. Torna a Microsoft Dynamics **Impostazioni**.

   ![](assets/image2014-12-12-9-3a7-3a25.png)

1. Sotto **Impostazioni**, fai clic su **Configurazione API Marketo**.

   ![](assets/image2014-12-12-9-3a7-3a34.png)

1. Fai clic su **Nuovo**.

   ![](assets/image2014-12-12-9-3a8-3a8.png)

1. Immetti le informazioni acquisite in precedenza da Marketo e fai clic su **Salva**.

   ![](assets/image2014-12-12-9-3a8-3a17.png)

## Imposta accesso utente {#set-user-access}

Infine, è necessario consentire a utenti specifici l&#39;accesso per utilizzare Marketo Sales Insight.

1. Vai a **Impostazioni**.

   ![](assets/image2014-12-12-9-3a8-3a34.png)

1. Vai a **Sicurezza**.

   ![](assets/image2015-4-29-14-3a56-3a33.png)

1. Fai clic su **Utenti**.

   ![](assets/image2015-4-29-14-3a57-3a46.png)

1. Selezionare gli utenti a cui si desidera accedere a Informazioni sulle vendite e fare clic su **Gestisci ruoli**.

   ![](assets/image2015-4-29-14-3a59-3a31.png)

1. Selezionare il ruolo Marketo Sales Insight e fare clic su **OK**.

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   E dovreste essere tutti fatti! Infine, per testare, accedi a Dynamics come utente con accesso a Marketo Sales Insight e cerca un lead o un contatto.

   ![](assets/image2015-4-29-15-3a2-3a27.png)

Ora hai sbloccato la potenza di Marketo Sales Insight per il tuo team di vendita.

>[!MORELIKETHIS]
>
>[Impostazione di stelle e fiamme per i record lead/contatti](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
