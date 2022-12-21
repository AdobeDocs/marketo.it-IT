---
unique-page-id: 11383945
description: Informazioni sulle conversioni offline di Facebook - Documentazione di Marketo - Documentazione del prodotto
title: Informazioni sulle conversioni offline di Facebook
exl-id: e0995ebc-47fb-4f10-b767-4fe9f572b2d2
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 0%

---

# Informazioni sulle conversioni offline di Facebook {#understanding-facebook-offline-conversions}

Le campagne facebook Lead Ads generano lead e li inviano a Marketo per l’utilizzo nelle campagne di marketing. Tuttavia, senza visibilità nelle conversioni offline, l&#39;inserzionista Facebook non può sapere quali annunci sono più efficaci. Ecco un esempio.

>[!NOTE]
>
>**Esempio**
>
>Facebook Lead Ads esegue tre annunci.
>
>* L’annuncio 1 genera 20 lead
>* L’annuncio 2 genera 30 lead
>* L’annuncio 3 genera 50 lead
>
>Basato solo su questi numeri, l&#39;Ad 3 sembra il più efficace.
>
>Tuttavia, quando si esaminano i dati sul lato Marketo, si sviluppa una storia diversa.
>
>* L’annuncio 1 genera 10 vendite
>* L&#39;annuncio 3 genera 2 vendite
>
>Ciò significa che l&#39;Ad 1, nonostante generasse meno lead, aveva un tasso di successo del 50%, mentre l&#39;Ad 3 non era affatto efficace.
>
>Senza conversioni offline, l&#39;inserzionista probabilmente investirà più denaro in Ad 3. Con i dati di conversione offline, l’inserzionista probabilmente investirà in Ad 1.

È possibile [configurare le conversioni offline di Facebook](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions.md) per inviare le prestazioni degli annunci offline a Facebook.

1. Assicurati che [Integrazione facebook LaunchPoint](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-facebook-custom-audiences-as-a-launchpoint-service.md) è aggiornato.
1. Mappa le fasi nel modello del ciclo di ricavi alle fasi di conversione offline su Facebook.
1. Quando un lead Facebook viene generato da un annuncio lead Facebook e raggiunge una fase mappata, Marketo invia i dati di conversione offline a Facebook diverse volte al giorno tramite un’API sicura e automatizzata. I dati vengono visualizzati nel rapporto di Facebook Ads Manager.

>[!MORELIKETHIS]
>
>[Configurazione delle conversioni offline di Facebook](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions.md)
