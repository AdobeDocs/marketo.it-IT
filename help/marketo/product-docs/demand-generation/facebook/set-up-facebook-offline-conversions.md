---
unique-page-id: 11383953
description: Configurare le conversioni offline di Facebook - Documenti Marketo - Documentazione del prodotto
title: Configurare le conversioni offline di Facebook
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 0%

---


# Configurare le conversioni offline di Facebook {#set-up-facebook-offline-conversions}

Inviando dati di conversione offline a Facebook per le persone create tramite gli annunci lead, il team pubblicitario può ottimizzare la spesa pubblicitaria in modo migliore che mai. Ecco come impostarlo.

>[!PREREQUISITES]
>
>* Devi [configurare gli annunci](set-up-facebook-lead-ads.md)lead di Facebook.
>* È necessario avere un modello approvato in [Revenue Cycle Modeler](http://docs.marketo.com/display/docs/revenue+cycle+models).

>



## Configurazione amministratore {#admin-configuration}

1. Vai ad **Amministratore** Marketo.

   ![](assets/image2016-11-29-13-3a8-3a45.png)

1. Passate a **LaunchPoint** e fate doppio clic sul servizio Annunci lead di Facebook creato in precedenza.

   >[!NOTE]
   >
   >Se non l&#39;avete ancora fatto, andate avanti e [configurate Facebook Lead Ads](set-up-facebook-lead-ads.md), quindi tornate qui.

   ![](assets/image2016-11-29-13-3a10-3a43.png)

1. Se lo desiderate, modificate il Nome **** visualizzato per includere le conversioni offline. Fate clic su **Avanti**.

   ![](assets/image2016-11-29-13-3a12-3a19.png)

1. Selezionate **Abilita conversioni** offline e fate clic su **Avanti**.

   ![](assets/image2016-11-29-13-3a13-3a32.png)

1. Fate clic su **Avanti**.

   ![](assets/image2016-11-29-13-3a14-3a17.png)

1. Fate clic su **Salva**.

   ![](assets/image2016-11-29-13-3a14-3a52.png)

   Dolce! L&#39;attivazione delle conversioni offline di Facebook è stata completata a metà. Andiamo al Modellatore del ciclo delle entrate per mappare le fasi.

   ![](assets/image2016-11-29-13-3a16-3a55.png)

## Configurazione del modello del ciclo delle entrate {#revenue-cycle-modeler-configuration}

1. Vai ad **Analytics**.

   ![](assets/image2016-11-29-13-3a29-3a23.png)

1. Selezionate il modello e fate clic su **Modifica bozza**.

   ![](assets/image2016-11-29-13-3a31-3a6.png)

   >[!NOTE]
   >
   >Attualmente, sono disponibili 10 eventi Facebook per mappare le fasi del ciclo di ricavi su:
   >
   >    
   >    
   >    * Aggiungi informazioni di pagamento
   >    * Aggiungi al carrello
   >    * Aggiunge all&#39;elenco dei desideri
   >    * Registrazioni completate
   >    * Checkout avviati
   >    * Person
   >    * Altro
   >    * Purchase
   >    * Ricerche
   >    * Visualizzazioni contenuto


1. Selezionate il passaggio da mappare, quindi dall’elenco a discesa Conversione **** Facebook, selezionate l’evento Facebook a cui desiderate mappare. Ripetete questo passaggio per mappare tutti gli stadi di RCM sulle fasi di conversione offline di Facebook.

   ![](assets/1-1.png)

1. Al termine della mappatura, chiudere il modello.

   ![](assets/2.png)

1. Approva il tuo modello e hai finito!

   ![](assets/image2016-11-29-15-3a6-3a30.png)

   Ora, quando i lead Lead Ad raggiungono le fasi mappate, le conversioni vengono inviate a Facebook per generare report.

   >[!CAUTION]
   >
   >Controllate il vostro account Facebook e accertatevi che tutti [gli annunci siano associati](https://www.facebook.com/business/url/?href=%2Fbusiness%2Fhelp%2Fwww%2F1776828022605281&amp;cmsid&amp;creative=link&amp;creative_detail=advertiser-help-center&amp;create_type&amp;destination_cms_id&amp;orig_http_referrer) al set di eventi di conversione offline di Marketo. In caso contrario, l&#39;attribuzione degli annunci potrebbe non funzionare.

   >[!NOTE]
   >
   >I dati di conversione offline vengono inviati da Marketo a Facebook più volte al giorno.

>[!NOTE]
>
>**Articoli correlati**
>
>* [Informazioni sulle conversioni offline di Facebook](understanding-facebook-offline-conversions.md)

>



