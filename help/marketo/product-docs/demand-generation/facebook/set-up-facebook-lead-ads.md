---
unique-page-id: 11379622
description: Configurare i lead Ads di Facebook - Documentazione di Marketo - Documentazione del prodotto
title: Configurare gli annunci lead di Facebook
exl-id: 24cb74da-6b46-45de-ba4a-66e3d490afd7
feature: Integrations
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---

# Configurare gli annunci lead di Facebook {#set-up-facebook-lead-ads}

Utilizzare [Annunci lead facebook](https://www.facebook.com/business/a/lead-ads) per eseguire campagne pubblicitarie in Facebook e generare lead per Marketo.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

>[!AVAILABILITY]
>
>Per aggiungere i lead Ads di Facebook alla tua istanza, contatta il team dell’account Adobe (il tuo Account Manager).

1. Vai a Marketo **Amministratore**.

   ![](assets/image2016-11-29-10-3a50-3a29.png)

1. Vai a **LaunchPoint**, fai clic su **Nuovo,** e seleziona **Nuovo servizio**.

   ![](assets/image2016-11-29-10-3a51-3a11.png)

1. Immetti un **Nome visualizzato** per il servizio, seleziona **Annunci lead facebook** dal menu a discesa, quindi fai clic su **Crea**.

   ![](assets/image2016-11-29-10-3a51-3a47.png)

1. Apri una nuova scheda nello stesso browser e vai a [facebook.com](https://www.facebook.com). Accedi a Facebook utilizzando l’account che desideri utilizzare per l’integrazione.

   >[!NOTE]
   >
   >L’account Facebook dovrà accedere a tutte le pagine aziendali Facebook da cui desideri richiamare annunci lead.

   ![](assets/image2016-11-29-10-3a52-3a29.png)

1. Dopo aver effettuato l’accesso a Facebook, torna a Marketo e fai clic su **Autorizza**.

   ![](assets/image2016-11-29-10-3a52-3a51.png)

1. Se richiesto, fare clic su **OK** per accettare l’installazione dell’app Marketo in Facebook.

   ![](assets/image2016-11-29-10-3a56-3a3.png)

1. Noterai che ora sei autorizzato. Clic **Successivo**.

   ![](assets/image2016-11-29-10-3a56-3a28.png)

1. Seleziona le pagine da cui Marketo deve richiamare i lead Ads di Facebook e fai clic su **Successivo**.

   >[!TIP]
   >
   >Se non trovi una pagina prevista, accertati che l’account Facebook utilizzato per l’autenticazione sia aggiunto alla pagina in Facebook e riprova.

   ![](assets/image2016-11-29-10-3a58-3a36.png)

1. Per accettare le mappature predefinite dei campi da Facebook a Marketo, fai clic su **Crea**.

   >[!TIP]
   >
   >Modificando le mappature, puoi personalizzare la posizione in cui vengono memorizzati i dati degli annunci lead in Marketo. È inoltre possibile [recuperare i dati dalle domande personalizzate relative agli annunci lead](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads/map-custom-fields-to-marketo.md).

   >[!CAUTION]
   >
   >Marketo non supporta la mappatura di due campi Facebook in un singolo campo Marketo, solo da 1 a 1. Se si esegue il mapping da 2 a 1, i lead potrebbero non essere in grado di accedere al sistema Marketo.

   ![](assets/image2016-11-29-11-3a0-3a2.png)

   Ben fatto! I lead inizieranno a fluire in Marketo man mano che eseguirai campagne Lead Ad di Facebook di successo.

   ![](assets/image2016-11-29-12-3a32-3a54.png)

>[!MORELIKETHIS]
>
>* [Assegnare/rimuovere le autorizzazioni in Gestione accesso lead (Facebook)](https://www.facebook.com/business/help/540596413257598?id=735435806665862)
>* [Utilizzare filtri e attivatori per annunci lead in una campagna avanzata](/help/marketo/product-docs/demand-generation/facebook/use-lead-ads-filters-and-triggers-in-a-smart-campaign.md)
>* [Mappa campi personalizzati su Marketo](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads/map-custom-fields-to-marketo.md)
