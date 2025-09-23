---
unique-page-id: 7513865
description: Installare e configurare Marketo Sales Insight in Microsoft Dynamics 2015 - Documentazione Marketo - Documentazione del prodotto
title: Installare e configurare Marketo Sales Insight in Microsoft Dynamics 2015
exl-id: 26c1f02c-c910-445d-8560-0b37961eadcb
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 4%

---

# Installa e configura [!DNL Marketo Sales Insight] in [!DNL Microsoft Dynamics 2015] {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

Marketo Sales Insight è uno strumento fantastico per offrire al vostro team di vendita una &quot;finestra&quot; sulla ricchezza di dati di cui dispone il team marketing. Ecco come installarlo e configurarlo in [!DNL Microsoft Dynamics 2015]

>[!PREREQUISITES]
>
>Completa l&#39;integrazione Marketo-Microsoft.
>
>[Scarica la soluzione corretta](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) per la tua versione di [!DNL Microsoft Dynamics CRM].

## Importa soluzione {#import-solution}

OK, è ora di importare la soluzione [!DNL Marketo Sales Insight] in [!DNL Microsoft Dynamics]. Ecco come:

1. In [!UICONTROL Microsoft Dynamics CRM] fare clic su **[!UICONTROL Settings]**.

   ![](assets/image2014-12-12-9-3a4-3a56.png)

1. In [!UICONTROL SETTINGS], fare clic su **[!UICONTROL Customizations]**.

   ![](assets/image2015-4-29-14-3a22-3a1.png)

1. Fai clic su **[!UICONTROL Solutions]**.

   ![](assets/image2014-12-12-9-3a5-3a17.png)

   >[!NOTE]
   >
   >Prima di procedere, dovreste aver già installato e configurato la soluzione Marketo.

1. Fai clic su **[!UICONTROL Import]**.

   ![](assets/image2014-12-12-9-3a5-3a27.png)

1. Nella nuova finestra, fare clic su **[!UICONTROL Browse]**.

   ![](assets/image2014-12-12-9-3a5-3a36.png)

1. Trova e seleziona la soluzione scaricata in precedenza.

   ![](assets/image2014-12-12-9-3a5-3a45.png)

1. Fai clic su **[!UICONTROL Next]**.

   ![](assets/image2014-12-12-9-3a5-3a55.png)

1. La soluzione verrà caricata. Puoi visualizzare il contenuto del pacchetto, se lo desideri. Fai clic su **[!UICONTROL Next]**.

   ![](assets/image2014-12-12-9-3a6-3a10.png)

1. Assicurarsi di lasciare selezionata la casella e fare clic su **[!UICONTROL Import]**.

   ![](assets/image2014-12-12-9-3a6-3a19.png)

1. Scaricare il file di registro, quindi fare clic su **[!UICONTROL Close]**.

   ![](assets/image2014-12-12-9-3a6-3a29.png)

1. Fantastico! Dovresti vedere la soluzione ora. Se non è presente, aggiorna lo schermo.

   ![](assets/image2014-12-12-9-3a6-3a40.png)

## Connettere Marketo e Sales Insight {#connect-marketo-and-sales-insight}

Colleghiamo l&#39;istanza di Marketo a [!DNL Sales Insight] in [!DNL Dynamics]. Ecco come:

>[!NOTE]
>
>Diritti di amministrazione richiesti.

1. Accedere a Marketo e passare alla sezione **[!UICONTROL Admin]**.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. Nella sezione [!UICONTROL Sales Insight] fare clic su **[!UICONTROL Edit API Configuration]**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Copiare **[!UICONTROL Marketo Host]**, **[!UICONTROL API URL]** e **[!UICONTROL API User Id]** per utilizzarli in un passaggio successivo. Immettere una chiave segreta API e fare clic su **[!UICONTROL Save]**.

   >[!CAUTION]
   >
   >Non utilizzare una e commerciale (&amp;) nella chiave segreta API.

   ![](assets/image2014-12-12-9-3a7-3a9.png)

   >[!NOTE]
   >
   >I campi seguenti devono essere sincronizzati con Marketo affinché *sia lead che contatto* per [!DNL Sales Insight] funzionino:
   >
   >* Priorità
   >* Urgenza
   >* Punteggio relativo
   >
   >Se manca uno di questi campi, in Marketo verrà visualizzato un messaggio di errore con il nome dei campi mancanti. Per risolvere il problema, eseguire [questa procedura](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. Torna tra [!DNL Microsoft Dynamics], passa a **[!UICONTROL Settings]**.

   ![](assets/image2014-12-12-9-3a7-3a25.png)

1. In **[!UICONTROL Settings]**, fare clic su **[!UICONTROL Marketo API Config]**.

   ![](assets/image2014-12-12-9-3a7-3a34.png)

1. Fai clic su **[!UICONTROL New]**.

   ![](assets/image2014-12-12-9-3a8-3a8.png)

1. Immettere le informazioni ottenute da Marketo in precedenza e fare clic su **[!UICONTROL Save]**.

   ![](assets/image2014-12-12-9-3a8-3a17.png)

## Imposta accesso utente {#set-user-access}

Infine, devi fornire a utenti specifici l’accesso per utilizzare Marketo Sales Insight.

1. Vai a **[!UICONTROL Settings]**.

   ![](assets/image2014-12-12-9-3a8-3a34.png)

1. Vai a **[!UICONTROL Security]**.

   ![](assets/image2015-4-29-14-3a56-3a33.png)

1. Fai clic su **[!UICONTROL Users]**.

   ![](assets/image2015-4-29-14-3a57-3a46.png)

1. Selezionare gli utenti a cui si desidera concedere l&#39;accesso a [!DNL Sales Insight] e fare clic su **[!UICONTROL Manage Roles]**.

   ![](assets/image2015-4-29-14-3a59-3a31.png)

1. Selezionare la mansione [!DNL Marketo Sales Insight] e fare clic su **[!UICONTROL OK]**.

   ![](assets/image2014-12-12-9-3a9-3a22.png)

   E dovreste aver finito! Infine, per eseguire il test, accedere a [!DNL Dynamics] come utente che ha accesso a [!DNL Marketo Sales Insight] e controllare un lead o un contatto.

   ![](assets/image2015-4-29-15-3a2-3a27.png)

Hai sbloccato la potenza di [!DNL Marketo Sales Insight] per il tuo team vendite.

>[!MORELIKETHIS]
>
>[Impostazione di stelle e fiamme per record lead/contatti](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
