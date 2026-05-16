---
unique-page-id: 11383953
description: Scopri come impostare le conversioni offline di Facebook in Marketo. Invia i dati di conversione da Marketo a Facebook per l’ottimizzazione degli annunci.
title: Configurare le conversioni offline di Facebook
exl-id: e1974943-8fc8-41f6-be7e-1b594de13db6
feature: Integrations
TQID: https://experienceleague.adobe.com/p5G-mS4yYAv-TvloYNSl52-IpEhQl8UuQwBN4M5KA2U
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b13bd2ad-8e65-49e5-9691-2a0d31067b35
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
  - id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 302
ht-degree: 3%

---

# Configura [!DNL Facebook] conversioni offline {#set-up-facebook-offline-conversions}

Inviando di nuovo i dati di conversione offline a [!DNL Facebook] per le persone create tramite annunci lead, il tuo team pubblicitario può ottimizzare la spesa pubblicitaria meglio che mai. Segui questi passaggi per configurarlo.

>[!PREREQUISITES]
>
>Devi [configurare i lead Ads di Facebook](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md).

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

   È stata completata l&#39;attivazione di [!DNL Facebook] conversioni offline. Procedi alla Modeler Ciclo ricavi per mappare le fasi.

   ![](assets/image2016-11-29-13-3a16-3a55.png)

## Configurazione Modeler del ciclo dei ricavi {#revenue-cycle-modeler-configuration}

1. Passa a **[!UICONTROL Analytics]**.

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

1. Approva il modello e hai terminato.

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
