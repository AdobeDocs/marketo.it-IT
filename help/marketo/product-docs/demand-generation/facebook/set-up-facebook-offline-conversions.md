---
unique-page-id: 11383953
description: Configurare le conversioni offline di Facebook - Documentazione di Marketo - Documentazione del prodotto
title: Configurare le conversioni offline di Facebook
exl-id: e1974943-8fc8-41f6-be7e-1b594de13db6
feature: Integrations
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---

# Configurare le conversioni offline di Facebook {#set-up-facebook-offline-conversions}

Inviando di nuovo i dati di conversione offline a Facebook per le persone create tramite Annunci lead, il team pubblicitario può ottimizzare la spesa pubblicitaria in modo migliore che mai. Ecco come configurarlo.

>[!PREREQUISITES]
>
>* Devi [configurare gli annunci lead Facebook](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md).
>* È necessario disporre di un modello approvato in [Modellatore ciclo ricavi](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/understanding-revenue-models.md).

## Configurazione amministratore {#admin-configuration}

1. Vai a Marketo **Amministratore**.

   ![](assets/image2016-11-29-13-3a8-3a45.png)

1. Vai a **LaunchPoint** e fare doppio clic sul servizio Facebook Lead Ads creato in precedenza.

   >[!NOTE]
   >
   >Se non l&#39;hai ancora fatto, continua e [Configurazione annunci lead Facebook](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md), quindi torna qui.

   ![](assets/image2016-11-29-13-3a10-3a43.png)

1. Se lo desideri, modifica il **Nome visualizzato** per includere le conversioni offline. Clic **Successivo**.

   ![](assets/image2016-11-29-13-3a12-3a19.png)

1. Verifica **Abilita conversioni offline** e fai clic su **Successivo**.

   ![](assets/image2016-11-29-13-3a13-3a32.png)

1. Clic **Successivo**.

   ![](assets/image2016-11-29-13-3a14-3a17.png)

1. Clic **Salva**.

   ![](assets/image2016-11-29-13-3a14-3a52.png)

   Dolce! Hai terminato a metà l’abilitazione delle conversioni offline di Facebook. Passiamo al Revenue Cycle Modeler per mappare le fasi.

   ![](assets/image2016-11-29-13-3a16-3a55.png)

## Configurazione Modeler ciclo ricavi {#revenue-cycle-modeler-configuration}

1. Vai a **Analytics**.

   ![](assets/image2016-11-29-13-3a29-3a23.png)

1. Seleziona il modello e fai clic su **Modifica bozza**.

   ![](assets/image2016-11-29-13-3a31-3a6.png)

   >[!NOTE]
   >
   >Attualmente, sono presenti 10 eventi Facebook su cui è possibile mappare le fasi del ciclo dei ricavi per:
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

1. Seleziona la fase da mappare, quindi dalla **Conversione facebook** selezionare l&#39;evento Facebook a cui si desidera associarlo. Ripetere questo passaggio per mappare tutte le fasi di RCM in fasi di conversione offline in Facebook.

   ![](assets/1-1.png)

1. Al termine della mappatura, chiudete il modello.

   ![](assets/2.png)

1. Approva il tuo modello e hai finito!

   ![](assets/image2016-11-29-15-3a6-3a30.png)

   Ora, quando i lead lead ad raggiungono le fasi mappate, le conversioni vengono inviate a Facebook per il reporting.

   >[!CAUTION]
   >
   >Controlla il tuo account Facebook e assicurati che tutti [gli annunci sono associati](https://www.facebook.com/business/url/?href=%2Fbusiness%2Fhelp%2Fwww%2F1776828022605281&amp;cmsid&amp;creative=link&amp;creative_detail=advertiser-help-center&amp;create_type&amp;destination_cms_id&amp;orig_http_referrer) al set di eventi Marketo Offline Conversions. In caso contrario, l’attribuzione potrebbe non funzionare.

   >[!NOTE]
   >
   >I dati di conversione offline vengono inviati da Marketo a Facebook diverse volte al giorno.

>[!MORELIKETHIS]
>
>[Informazioni sulle conversioni offline di Facebook](/help/marketo/product-docs/demand-generation/facebook/understanding-facebook-offline-conversions.md)
