---
unique-page-id: 11383953
description: Configurare le conversioni offline di Facebook - Documentazione di Marketo - Documentazione del prodotto
title: Configurare le conversioni offline di Facebook
exl-id: e1974943-8fc8-41f6-be7e-1b594de13db6
feature: Integrations
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 1%

---

# Configura [!DNL Facebook] conversioni offline {#set-up-facebook-offline-conversions}

Inviando di nuovo i dati di conversione offline a [!DNL Facebook] per le persone create tramite annunci lead, il tuo team pubblicitario può ottimizzare la spesa pubblicitaria meglio che mai. Ecco come configurarlo.

>[!PREREQUISITES]
>
>* Devi [configurare i lead Ads di Facebook](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md).
>* È necessario disporre di un modello approvato in [Revenue Cycle Modeler](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/understanding-revenue-models.md).

## Configurazione amministratore {#admin-configuration}

1. Passare a Marketo **[!UICONTROL Admin]**.

   ![](assets/image2016-11-29-13-3a8-3a45.png)

1. Vai a **[!UICONTROL LaunchPoint]** e fai doppio clic sul servizio Annunci lead di Facebook creato in precedenza.

   >[!NOTE]
   >
   >Se non l&#39;hai ancora fatto, [Configura [!UICONTROL Facebook Lead Ads]](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md), quindi torna qui.

   ![](assets/image2016-11-29-13-3a10-3a43.png)

1. Se lo desideri, modifica **[!UICONTROL Display Name]** per includere le conversioni offline. Fai clic su **[!UICONTROL Next]**.

   ![](assets/image2016-11-29-13-3a12-3a19.png)

1. Selezionare **[!UICONTROL Enable Offline Conversions]** e fare clic su **[!UICONTROL Next]**.

   ![](assets/image2016-11-29-13-3a13-3a32.png)

1. Fai clic su **[!UICONTROL Next]**.

   ![](assets/image2016-11-29-13-3a14-3a17.png)

1. Fai clic su **[!UICONTROL Save]**.

   ![](assets/image2016-11-29-13-3a14-3a52.png)

   Dolce! Hai terminato a metà l&#39;abilitazione di [!DNL Facebook] Conversioni offline. Passiamo al Modeler del ciclo dei ricavi per mappare le fasi.

   ![](assets/image2016-11-29-13-3a16-3a55.png)

## Configurazione Modeler del ciclo dei ricavi {#revenue-cycle-modeler-configuration}

1. Vai a **[!UICONTROL Analytics]**.

   ![](assets/image2016-11-29-13-3a29-3a23.png)

1. Selezionare il modello e fare clic su **[!UICONTROL Edit Draft]**.

   ![](assets/image2016-11-29-13-3a31-3a6.png)

   >[!NOTE]
   >
   >Attualmente, sono presenti 10 [!DNL Facebook] eventi a cui è possibile mappare le fasi del ciclo dei ricavi:
   >
   >* Aggiunte di informazioni di pagamento
   >* Aggiunte al carrello
   >* Aggiunte alla lista dei desideri
   >* Registrazioni completate
   >* Pagamenti avviati
   >* Persona
   >* Altro
   >* Acquisto
   >* Ricerche
   >* Visualizzazioni contenuto

1. Selezionare la fase da mappare, quindi dal menu a discesa **[!UICONTROL Facebook Conversion]** selezionare l&#39;evento [!DNL Facebook] a cui si desidera mappare l&#39;evento. Ripetere questo passaggio per mappare tutte le fasi di RCM alle fasi di conversione offline in [!DNL Facebook].

   ![](assets/1-1.png)

1. Al termine della mappatura, chiudete il modello.

   ![](assets/2.png)

1. Approva il tuo modello e hai finito!

   ![](assets/image2016-11-29-15-3a6-3a30.png)

   Ora, quando i lead ad raggiungono le fasi mappate, le conversioni vengono inviate a [!DNL Facebook] per il reporting.

   >[!CAUTION]
   >
   >Controlla il tuo account [!DNL Facebook] e assicurati che tutti gli [annunci siano associati](https://www.facebook.com/business/url/?href=%2Fbusiness%2Fhelp%2Fwww%2F1776828022605281&cmsid&creative=link&creative_detail=advertiser-help-center&create_type&destination_cms_id&orig_http_referrer) al set di eventi per conversioni offline di Marketo. In caso contrario, l’attribuzione potrebbe non funzionare.

   >[!NOTE]
   >
   >I dati di conversione offline vengono inviati da Marketo a [!DNL Facebook] diverse volte al giorno.

>[!MORELIKETHIS]
>
>[Informazioni [!DNL Facebook] Sulle Conversioni Offline](/help/marketo/product-docs/demand-generation/facebook/understanding-facebook-offline-conversions.md)
