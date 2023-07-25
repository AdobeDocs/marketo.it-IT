---
unique-page-id: 3571737
description: Installare e configurare Marketo Sales Insight in Microsoft Dynamics 2013 - Documentazione di Marketo - Documentazione del prodotto
title: Installare e configurare Marketo Sales Insight in Microsoft Dynamics 2013
exl-id: 290db451-47a6-4cfa-a36f-bc12ef7d3482
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 0%

---

# Installare e configurare Marketo Sales Insight in Microsoft Dynamics 2013 {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo Sales Insight è uno strumento fantastico per dare al vostro team di vendita una &quot;finestra&quot; sulla ricchezza di dati che il team di marketing ha. Ecco come installarlo e configurarlo.

>[!PREREQUISITES]
>
>Completa l&#39;integrazione Marketo-Microsoft.
>
>[Scaricare la soluzione corretta](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) per la versione di Microsoft Dynamics CRM in uso.

## Importa soluzione {#import-solution}

Ora è il momento di importare la soluzione Marketo Sales Insight in Microsoft Dynamics.

1. Sotto **Microsoft Dynamics CRM** click **Impostazioni**.

   ![](assets/image2014-12-12-9-3a4-3a56.png)

1. Sotto **Impostazioni**, fai clic su **Personalizzazioni**.

   ![](assets/image2014-12-12-9-3a5-3a6.png)

1. Clic **Soluzioni**.

   ![](assets/image2014-12-12-9-3a5-3a17.png)

   >[!NOTE]
   >
   >Prima di procedere, dovresti aver già installato e configurato Marketo

1. Clic **Importa**.

   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. Nella nuova finestra, fai clic su **Sfoglia**.

   ![](assets/image2014-12-12-9-3a5-3a36.png)

1. Trova e seleziona la soluzione scaricata in precedenza.

   ![](assets/image2014-12-12-9-3a5-3a45.png)

1. Clic **Successivo**.

   ![](assets/image2014-12-12-9-3a5-3a55.png)

1. La soluzione verrà caricata. Puoi visualizzare il contenuto del pacchetto, se lo desideri. Clic **Successivo**.

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. Assicurati di lasciare selezionata la casella e fai clic su **Importa**.

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. Scarica il file di registro. Fai clic su **Chiudi**.

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. Fantastico! Dovresti vedere la soluzione ora. Se non è presente, aggiorna lo schermo.

   ![](assets/image2014-12-12-9-3a6-3a40.png)

## Connettere Marketo e Sales Insight {#connect-marketo-and-sales-insight}

Colleghiamo la tua istanza di Marketo a Sales Insight in Dynamics.

>[!NOTE]
>
>Diritti di amministrazione richiesti.

1. Accedi a Marketo e passa a **Amministratore** sezione.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. Sotto **Insight sulle vendite** clic sezione **Modifica configurazione API**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Copia il **Host Marketo**, **URL API**, e **ID utente API** da utilizzare in un passaggio successivo. Immetti un **Chiave segreta API** a tua scelta e fai clic su **Salva**.

   >[!CAUTION]
   >
   >Non utilizzare una e commerciale (&amp;) nella chiave segreta API.

   ![](assets/image2014-12-12-9-3a7-3a9.png)

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

   ![](assets/image2014-12-12-9-3a7-3a25.png)

1. Sotto **Impostazioni**, fai clic su **Configurazione API Marketo**.

   ![](assets/image2014-12-12-9-3a7-3a34.png)

1. Clic **Nuovo**.

   ![](assets/image2014-12-12-9-3a8-3a8.png)

1. Immetti le informazioni ottenute da Marketo in precedenza e fai clic su **Salva**.

   ![](assets/image2014-12-12-9-3a8-3a17.png)

## Imposta accesso utente {#set-user-access}

Infine, puoi fornire a utenti specifici l’accesso a Marketo Sales Insight.

1. Vai a **Impostazioni**.

   ![](assets/image2014-12-12-9-3a8-3a34.png)

1. Clic **Utenti**.

   ![](assets/image2014-12-12-9-3a8-3a42.png)

1. Seleziona gli utenti a cui vuoi concedere l’accesso a Sales Insight e fai clic su **Gestisci ruoli**.

   ![](assets/image2014-12-12-9-3a9-3a13.png)

1. Seleziona la **Insight sulla vendita di Marketo** ruolo e clic **OK**.

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   E dovreste aver finito! Infine, per eseguire il test, accedi a Dynamics come utente che ha accesso a Marketo Sales Insight e controlla un lead o un contatto.

   ![](assets/image2014-12-12-9-3a9-3a31.png)

Ora hai sbloccato la potenza di Marketo Sales Insight per il tuo team di vendita.

>[!MORELIKETHIS]
>
>[Impostazione di stelle e fiamme per record lead/contatti](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
