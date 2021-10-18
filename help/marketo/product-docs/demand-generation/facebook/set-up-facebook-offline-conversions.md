---
unique-page-id: 11383953
description: Configurare le conversioni offline di Facebook - Documentazione Marketo - Documentazione del prodotto
title: Configurare le conversioni offline di Facebook
exl-id: e1974943-8fc8-41f6-be7e-1b594de13db6
source-git-commit: 41d8762203786bac9aea03ac978daa0549ac8e93
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 0%

---

# Configurare le conversioni offline di Facebook {#set-up-facebook-offline-conversions}

Inviando i dati di conversione offline a Facebook per le persone create tramite Lead Ads, il team pubblicitario può ottimizzare la spesa pubblicitaria in modo migliore che mai. Ecco come configurarlo.

>[!PREREQUISITES]
>
>* Devi [configurare Facebook Lead Ads](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md).
>* È necessario disporre di un modello approvato in [Modellatore del ciclo dei ricavi](/help/marketo/product-docs/reporting/revenue-cycle-analytics/revenue-cycle-models/understanding-revenue-models.md).


## Configurazione amministratore {#admin-configuration}

1. Vai a Marketo **Amministratore**.

   ![](assets/image2016-11-29-13-3a8-3a45.png)

1. Vai a **LaunchPoint** e fai doppio clic sul servizio Facebook Lead Ads creato in precedenza.

   >[!NOTE]
   >
   >Se non l&#39;hai fatto, vai avanti e [Imposta annunci lead Facebook](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)Poi torna qui.

   ![](assets/image2016-11-29-13-3a10-3a43.png)

1. Se lo desideri, modifica la **Nome visualizzato** per includere le conversioni offline. Fai clic su **Successivo**.

   ![](assets/image2016-11-29-13-3a12-3a19.png)

1. Controlla **Abilita conversioni offline** e fai clic su **Successivo**.

   ![](assets/image2016-11-29-13-3a13-3a32.png)

1. Fai clic su **Successivo**.

   ![](assets/image2016-11-29-13-3a14-3a17.png)

1. Fai clic su **Salva**.

   ![](assets/image2016-11-29-13-3a14-3a52.png)

   Dolce! Hai quasi finito di abilitare le conversioni offline di Facebook. Saltiamo sul modello del ciclo dei ricavi per mappare le fasi.

   ![](assets/image2016-11-29-13-3a16-3a55.png)

## Configurazione del modello del ciclo dei ricavi {#revenue-cycle-modeler-configuration}

1. Vai a **Analytics**.

   ![](assets/image2016-11-29-13-3a29-3a23.png)

1. Seleziona il modello e fai clic su **Modifica bozza**.

   ![](assets/image2016-11-29-13-3a31-3a6.png)

   >[!NOTE]
   >
   >Al momento, ci sono 10 eventi Facebook che puoi mappare le fasi del ciclo di ricavi su:
   >
   >* Somma delle informazioni di pagamento
   >* Aggiunge al carrello
   >* Aggiunge all&#39;elenco dei desideri
   >* Registrazioni completate
   >* Pagamenti avviati
   >* Persona
   >* Altro
   >* Acquisto
   >* Ricerche
   >* Visualizzazioni contenuto


1. Seleziona l’area di visualizzazione da mappare, quindi dalla **Conversione facebook** a discesa, seleziona l’evento Facebook in cui desideri mapparlo. Ripeti questo passaggio per mappare tutti gli stadi del tuo RCM sugli stadi di conversione offline in Facebook.

   ![](assets/1-1.png)

1. Al termine della mappatura, chiudete il modello.

   ![](assets/2.png)

1. Approva il tuo modello e hai finito!

   ![](assets/image2016-11-29-15-3a6-3a30.png)

   Ora, quando i lead di annunci lead raggiungono le fasi mappate, le conversioni vengono inviate a Facebook per la generazione di rapporti.

   >[!CAUTION]
   >
   >Controlla il tuo account Facebook e assicurati che [gli annunci sono associati](https://www.facebook.com/business/url/?href=%2Fbusiness%2Fhelp%2Fwww%2F1776828022605281&amp;cmsid&amp;creative=link&amp;creative_detail=advertiser-help-center&amp;create_type&amp;destination_cms_id&amp;orig_http_referrer) al set di eventi Conversioni offline Marketo. In caso contrario, l’attribuzione degli annunci potrebbe non funzionare.

   >[!NOTE]
   >
   >I dati di conversione offline vengono inviati da Marketo a Facebook diverse volte al giorno.

>[!MORELIKETHIS]
>
>[Informazioni sulle conversioni offline di Facebook](/help/marketo/product-docs/demand-generation/facebook/understanding-facebook-offline-conversions.md)
