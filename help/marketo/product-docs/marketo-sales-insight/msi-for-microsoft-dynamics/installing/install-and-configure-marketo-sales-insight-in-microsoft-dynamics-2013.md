---
unique-page-id: 3571737
description: Installare e configurare Marketo Sales Insight in Microsoft Dynamics 2013 - Documentazione di Marketo - Documentazione del prodotto
title: Installazione e configurazione di Marketo Sales Insight in Microsoft Dynamics 2013
exl-id: 290db451-47a6-4cfa-a36f-bc12ef7d3482
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---

# Installazione e configurazione di Marketo Sales Insight in Microsoft Dynamics 2013 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo Sales Insight è uno strumento fantastico per dare al tuo team di vendita una &quot;finestra&quot; nella ricchezza di dati di cui dispone il team di marketing. Ecco come installarlo e configurarlo.

>[!PREREQUISITES]
>
>Completa l’integrazione Marketo-Microsoft.
>
>[Scarica la soluzione corretta](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) per la tua versione di Microsoft Dynamics CRM.

## Soluzione di importazione {#import-solution}

OK, ora è il momento di importare la soluzione Marketo Sales Insight in Microsoft Dynamics.

1. Sotto **Microsoft Dynamics CRM** click **Impostazioni**.

   ![](assets/image2014-12-12-9-3a4-3a56.png)

1. Sotto **Impostazioni**, fai clic su **Personalizzazioni**.

   ![](assets/image2014-12-12-9-3a5-3a6.png)

1. Fai clic su **Soluzioni**.

   ![](assets/image2014-12-12-9-3a5-3a17.png)

   >[!NOTE]
   >
   >Prima di procedere, avrebbe già dovuto installare e configurare Marketo

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

1. Scaricate il file di registro. Fai clic su **Chiudi**.

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. Fantastico! Dovresti vedere la soluzione ora. Se non è presente, aggiorna lo schermo.

   ![](assets/image2014-12-12-9-3a6-3a40.png)

## Collegare Marketo e Sales Insight {#connect-marketo-and-sales-insight}

Colleghiamo la tua istanza Marketo a Sales Insight in Dynamics.

>[!NOTE]
>
>Sono richiesti i diritti di amministratore.

1. Accedi a Marketo e vai al **Amministratore** sezione .

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. Sotto la **Approfondimenti vendite** clic sulla sezione **Modifica configurazione API**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Copia il **Host Marketo**, **URL API** e **ID utente API** da utilizzare in un passaggio successivo. Inserisci un **Chiave segreta API** di tua scelta e fai clic su **Salva**.

   >[!CAUTION]
   >
   >Non utilizzare una e commerciale (&amp;) nella chiave segreto API.

   ![](assets/image2014-12-12-9-3a7-3a9.png)

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

   ![](assets/image2014-12-12-9-3a7-3a25.png)

1. Sotto **Impostazioni**, fai clic su **Configurazione API Marketo**.

   ![](assets/image2014-12-12-9-3a7-3a34.png)

1. Fai clic su **Nuovo**.

   ![](assets/image2014-12-12-9-3a8-3a8.png)

1. Immetti le informazioni acquisite in precedenza da Marketo e fai clic su **Salva**.

   ![](assets/image2014-12-12-9-3a8-3a17.png)

## Imposta accesso utente {#set-user-access}

Infine, puoi dare a utenti specifici l&#39;accesso a Marketo Sales Insight.

1. Vai a **Impostazioni**.

   ![](assets/image2014-12-12-9-3a8-3a34.png)

1. Fai clic su **Utenti**.

   ![](assets/image2014-12-12-9-3a8-3a42.png)

1. Selezionare gli utenti a cui si desidera accedere a Informazioni sulle vendite e fare clic su **Gestisci ruoli**.

   ![](assets/image2014-12-12-9-3a9-3a13.png)

1. Seleziona la **Informazioni sulle vendite Marketo** ruolo e clic **OK**.

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   E dovreste essere tutti fatti! Infine, per eseguire il test, accedi a Dynamics come utente con accesso a Marketo Sales Insight e cerca un lead o un contatto.

   ![](assets/image2014-12-12-9-3a9-3a31.png)

Ora hai sbloccato la potenza di Marketo Sales Insight per il tuo team di vendita.

>[!MORELIKETHIS]
>
>[Impostazione di stelle e fiamme per i record lead/contatti](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
