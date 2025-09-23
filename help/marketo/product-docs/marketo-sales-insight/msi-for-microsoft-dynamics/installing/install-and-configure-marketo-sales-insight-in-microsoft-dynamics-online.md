---
unique-page-id: 37355602
description: Installare e configurare Marketo Sales Insight in Microsoft Dynamics Online - Documentazione Marketo - Documentazione del prodotto
title: Installare e configurare Marketo Sales Insight in Microsoft Dynamics Online
exl-id: 3b58b109-96f9-427e-be5c-a8db270ffe69
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 4%

---

# Installa e configura [!DNL Marketo Sales Insight] in [!DNL Microsoft Dynamics Online] {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics-online}

[!DNL Marketo Sales Insight] è uno strumento fantastico per offrire al tuo team di vendita una &quot;finestra&quot; sulla ricchezza di dati di cui dispone il team Marketing. Ecco come installarlo e configurarlo in [!DNL Microsoft Dynamics Online].

>[!PREREQUISITES]
>
>Completa l&#39;integrazione Marketo-Microsoft.
>
>[Scarica la soluzione corretta](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) per la tua versione di [!DNL Microsoft Dynamics CRM].

## Importa soluzione {#import-solution}

>[!NOTE]
>
>Se utilizzi l&#39;interfaccia unificata, prima del passaggio 1 di seguito, fai clic sull&#39;icona Impostazioni in alto a destra e seleziona **[!UICONTROL Advanced Settings]**.

1. In Microsoft Dynamics CRM fare clic su **[!UICONTROL Settings]**.

   ![](assets/image2014-12-12-9-3a4-3a56-1.png)

1. In Impostazioni fare clic su **[!UICONTROL Customizations]**.

   ![](assets/image2015-4-29-14-3a22-3a1-1.png)

1. Fai clic su **[!UICONTROL Solutions]**.

   ![](assets/image2014-12-12-9-3a5-3a17-1.png)

   >[!NOTE]
   >
   >Prima di procedere, dovreste aver già installato e configurato la soluzione Marketo.

1. Fai clic su **[!UICONTROL Import]**.

   ![](assets/image2014-12-12-9-3a5-3a27-1.png)

1. Nella nuova finestra, fare clic su **[!UICONTROL Browse]**.

   ![](assets/image2014-12-12-9-3a5-3a36-1.png)

1. Nel computer, individuare e installare la soluzione appena scaricata.

1. Fai clic su **[!UICONTROL Next]**.

   ![](assets/seven.png)

1. La soluzione verrà caricata. Puoi visualizzare il contenuto del pacchetto, se lo desideri. Fai clic su **[!UICONTROL Next]**.

   ![](assets/image2014-12-12-9-3a6-3a10-1.png)

1. Assicurarsi di lasciare selezionata la casella e fare clic su **[!UICONTROL Import]**.

   ![](assets/image2014-12-12-9-3a6-3a19-1.png)

1. Scaricare il file di registro, quindi fare clic su **[!UICONTROL Close]**.

   ![](assets/image2014-12-12-9-3a6-3a29-1.png)

1. Fantastico! Dovresti vedere la soluzione ora. Se non è presente, aggiorna lo schermo.

   ![](assets/eleven.png)

1. Fai clic su **[!UICONTROL Publish Customization]**.

   >[!NOTE]
   >
   >Assicurarsi di abilitare la sincronizzazione globale di [!DNL MS Dynamics].

## Connetti Marketo e [!DNL Sales Insight] {#connect-marketo-and-sales-insight}

Colleghiamo l&#39;istanza di Marketo a [!DNL Sales Insight] in [!DNL Dynamics]. Ecco come:

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

1. Accedi a Marketo e passa alla sezione **[!UICONTROL Admin]**.

   ![](assets/image2014-12-12-9-3a6-3a50-1.png)

1. Nella sezione [!UICONTROL Sales Insight] fare clic su **[!UICONTROL Edit API Configuration]**.

   ![](assets/image2014-12-12-9-3a7-3a0-1.png)

1. Copiare **[!UICONTROL Marketo Host]**, **[!UICONTROL API URL]** e **[!UICONTROL API User Id]** per utilizzarli in un passaggio successivo. Immettere una chiave segreta API e fare clic su **[!UICONTROL Save]**.

   >[!CAUTION]
   >
   >Non utilizzare una e commerciale (&amp;) nella chiave segreta API.

   ![](assets/image2014-12-12-9-3a7-3a9-1.png)

   >[!NOTE]
   >
   >I campi seguenti devono essere sincronizzati con Marketo affinché _sia lead che contatto_ per [!DNL Sales Insight] funzionino:
   >
   >* Priorità
   >* Urgenza
   >* Punteggio relativo
   >
   >Se manca uno di questi campi, in Marketo verrà visualizzato un messaggio di errore con il nome dei campi mancanti. Per risolvere il problema, eseguire [questa procedura](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. Torna tra [!DNL Microsoft Dynamics], passa a **[!UICONTROL Settings]**.

   ![](assets/image2014-12-12-9-3a7-3a25-1.png)

1. In **[!UICONTROL Settings]**, fare clic su **[!UICONTROL Marketo API Config]**.

   ![](assets/image2014-12-12-9-3a7-3a34-1.png)

1. Fai clic su **[!UICONTROL New]**.

   ![](assets/image2014-12-12-9-3a8-3a8-1.png)

1. Immettere le informazioni ottenute da Marketo in precedenza e fare clic su **[!UICONTROL Save]**.

   ![](assets/image2014-12-12-9-3a8-3a17-1.png)

## Abilita sincronizzazione {#enable-sync}

1. In Marketo, fare clic su **[!UICONTROL Admin]**.

   ![](assets/enable-one.png)

1. In Integrazione, selezionare **[!UICONTROL Microsoft Dynamics]**.

   ![](assets/enable-two.png)

1. Fai clic su **[!UICONTROL Enable Sync]**.

   ![](assets/enable-three.png)

1. Fai clic su **[!UICONTROL Edit]** accanto a [!UICONTROL Field Sync Details].

   ![](assets/enable-four.png)

1. _seleziona automaticamente_ i campi MSI precedentemente disabilitati ([!UICONTROL Urgency], [!UICONTROL Relative Score] e [!UICONTROL Priority]). Fai clic su **[!UICONTROL Save]** per avviare la sincronizzazione dei dati.

   ![](assets/enable-five.png)

## Imposta accesso utente {#set-user-access}

Infine, devi fornire a utenti specifici l&#39;accesso per utilizzare [!DNL Marketo Sales Insight].

1. Vai a **[!UICONTROL Settings]**.

   ![](assets/image2014-12-12-9-3a8-3a34-1.png)

1. Vai a **[!UICONTROL Security]**.

   ![](assets/image2015-4-29-14-3a56-3a33-1.png)

1. Fai clic su **[!UICONTROL Users]**.

   ![](assets/image2015-4-29-14-3a57-3a46-1.png)

1. Selezionare gli utenti a cui si desidera concedere l&#39;accesso a [!DNL Sales Insight] e fare clic su **[!UICONTROL Manage Roles]**.

   ![](assets/image2015-4-29-14-3a59-3a31-1.png)

1. Selezionare la mansione [!DNL Marketo Sales Insight] e fare clic su **[!UICONTROL OK]**.

   ![](assets/image2014-12-12-9-3a9-3a22-1.png)

   E dovreste aver finito! Infine, per eseguire il test, accedere a [!DNL Dynamics] come utente che ha accesso a [!DNL Marketo Sales Insight] e controllare un lead o un contatto.

   ![](assets/image2015-4-29-15-3a2-3a27-1.png)

>[!MORELIKETHIS]
>
>[Impostazione di stelle e fiamme per record lead/contatti](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
