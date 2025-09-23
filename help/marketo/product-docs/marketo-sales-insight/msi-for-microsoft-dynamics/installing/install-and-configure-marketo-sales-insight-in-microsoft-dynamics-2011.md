---
unique-page-id: 3571735
description: Installare e configurare Marketo Sales Insight in Microsoft Dynamics 2011 - Documentazione Marketo - Documentazione del prodotto
title: Installare e configurare Marketo Sales Insight in Microsoft Dynamics 2011
exl-id: 40622dcc-7129-4392-95dc-ca829c15c3a6
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 5%

---

# Installa e configura [!DNL Marketo Sales Insight] in [!DNL Microsoft Dynamics 2011] {#install-and-configure-marketo-sales-insight-in-microsoft-dynamics}

[!DNL Marketo Sales Insight] è uno strumento fantastico per il tuo team di vendita. Seguono istruzioni dettagliate su come installarlo e configurarlo in [!DNL Microsoft Dynamics 2011] locale.

>[!PREREQUISITES]
>
>Completa l&#39;integrazione Marketo-Microsoft.
>
>[Scarica la soluzione corretta](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md) per la tua versione di [!DNL Microsoft Dynamics] CRM.

## Importa soluzione {#import-solution}

1. Accedi a [!DNL Microsoft Dynamics] CRM. Fare clic su **[!UICONTROL Settings]** nel menu in basso a sinistra.

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. Selezionare **[!UICONTROL Solutions]** nella struttura.

   ![](assets/image2015-5-4-10-3a41-3a56.png)

1. Fai clic su **Importa** ( ![](assets/image2015-5-4-10-3a45-3a44.png)).

   ![](assets/image2015-5-4-10-3a42-3a38.png)

   >[!NOTE]
   >
   >Prima di procedere, dovresti avere già [installato e configurato](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/install-and-configure-marketo-sales-insight-in-microsoft-dynamics-2011.md) la soluzione Marketo.

1. Fare clic su **[!UICONTROL Browse]**. Selezionare la soluzione [!DNL Marketo Sales Insight] [scaricata](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/installing/download-the-marketo-sales-insight-solution-for-microsoft-dynamics.md). Fai clic su **[!UICONTROL Next]**.

   ![](assets/image2015-5-4-10-3a55-3a15.png)

1. Verificare i dettagli della soluzione e fare clic su **[!UICONTROL Next]**.

   ![](assets/image2015-5-4-10-3a57-3a31.png)

1. Assicurati che l’opzione Messaggio di SDK sia selezionata. Fai clic su **[!UICONTROL Next]**.

   ![](assets/image2015-5-4-11-3a43-3a37.png)

1. Ora attendi il completamento dell’importazione.

   ![](assets/image2015-5-4-11-3a0-3a58.png)

1. Fai clic su **[!UICONTROL Close]**.

   ![](assets/crmhand.png)

1. [!DNL Marketo Sales Insight] verrà ora visualizzato nell&#39;elenco delle soluzioni. Yay!

   ![](assets/image2015-5-4-11-3a2-3a37.png)

1. Seleziona [!DNL Marketo Sales Insight] e fai clic su **Pubblica tutte le personalizzazioni** ( ![](assets/image2015-5-4-11-3a7-3a8.png)).

   ![](assets/image2015-5-4-11-3a8-3a27.png)

## Connettere Marketo e Sales Insight  {#connect-marketo-and-sales-insight}

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

1. Accedere a Marketo e fare clic su **[!UICONTROL Admin]**.

   ![](assets/image2014-12-12-9-3a6-3a50.png)

1. Nella sezione **[!UICONTROL Sales Insight]** fare clic su **[!UICONTROL Edit API Configuration]**.

   ![](assets/image2014-12-12-9-3a7-3a0.png)

1. Copiare **[!UICONTROL Marketo Host]**, **[!UICONTROL API URL]** e **[!UICONTROL API User Id]** per utilizzarli in un passaggio successivo. Immettere un **[!UICONTROL API Secret Key]** desiderato e fare clic su **[!UICONTROL Save]**.

   >[!CAUTION]
   >
   >Non utilizzare una e commerciale (&amp;) nella chiave segreta API.

   ![](assets/image2015-5-4-11-3a16-3a3.png)

   >[!NOTE]
   >
   >I campi seguenti devono essere sincronizzati con Marketo Insight affinché _lead e contatto_ funzionino correttamente:
   >
   >* Priorità
   >* Urgenza
   >* Punteggio relativo
   >
   >Se manca uno di questi campi, in Marketo verrà visualizzato un messaggio di errore con il nome dei campi mancanti. Per risolvere il problema, eseguire [questa procedura](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/required-fields-for-syncing-marketo-with-dynamics.md).

1. Torna a Dynamics, seleziona **[!UICONTROL Settings]**.

   ![](assets/image2015-5-4-10-3a39-3a44.png)

1. Selezionare **[!UICONTROL Marketo API Config]** nella struttura.

   ![](assets/image2015-5-4-11-3a22-3a41.png)

1. Fai clic su **[!UICONTROL Default Configuration]**.

   ![](assets/image2015-5-4-11-3a26-3a10.png)

1. Immetti le informazioni ottenute da Marketo in precedenza.

   ![](assets/image2015-5-4-11-3a27-3a16.png)

1. Fai clic su **[!UICONTROL Save]**.

   ![](assets/image2015-5-4-11-3a28-3a13.png)

## Imposta accesso utente {#set-user-access}

Configurare i ruoli utente per consentire a utenti specifici l&#39;accesso a [!DNL Sales Insight].

1. Seleziona **[!UICONTROL Settings]**.

   ![](assets/image2015-5-4-11-3a30-3a54.png)

1. Selezionare **[!UICONTROL Administration]** nella struttura.

   ![](assets/image2015-5-4-11-3a31-3a39.png)

1. Fai clic su **[!UICONTROL Users]**.

   ![](assets/image2015-5-4-11-3a32-3a25.png)

1. Selezionare gli utenti a cui si desidera concedere l&#39;accesso e fare clic su **[!UICONTROL Manage Roles]**.

   ![](assets/image2015-5-4-11-3a35-3a8.png)

1. Selezionare la mansione **[!UICONTROL Marketo Sales Insight]** e fare clic su **[!UICONTROL OK]**.

   ![](assets/image2015-5-4-11-3a36-3a59.png)

   Ed è tutto! Tutti gli utenti con accesso potranno ora visualizzare la sezione sales insight nella vista lead/dettagli contatto.

   ![](assets/image2015-5-4-11-3a39-3a23.png)

   Congratulazioni. Hai liberato la potenza di [!DNL Marketo Sales Insight].

>[!MORELIKETHIS]
>
>[Impostazione di stelle e fiamme per record lead/contatti](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
