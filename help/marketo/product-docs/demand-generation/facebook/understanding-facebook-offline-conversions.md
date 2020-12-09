---
unique-page-id: 11383945
description: Informazioni sulle conversioni offline di Facebook - Documenti Marketo - Documentazione prodotto
title: Informazioni sulle conversioni offline di Facebook
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 0%

---


# Informazioni sulle conversioni offline di Facebook {#understanding-facebook-offline-conversions}

Le campagne lead Ads di Facebook generano lead e li inviano a Marketo per l&#39;utilizzo nelle campagne di marketing. Tuttavia, senza visibilità nelle conversioni offline, l&#39;inserzionista Facebook non può sapere quali annunci sono più efficaci. Ecco un esempio.

>[!NOTE]
>
>**Esempio**
>
>Facebook Lead Ads esegue tre annunci.
>
>* Ad 1 genera 20 lead
>* Ad 2 genera 30 lead
>* Ad 3 genera 50 lead

>
>
Basandosi solo su questi numeri, Ad 3 sembra il più efficace.
>
>Tuttavia, quando si esaminano i dati dal lato di Marketo, si sviluppa una storia diversa.
>
>* L&#39;annuncio 1 genera 10 vendite
>* Ad 3 genera 2 vendite

>
>
Ciò significa che l&#39;annuncio 1, nonostante avesse generato meno lead, aveva un tasso di successo del 50%, mentre l&#39;annuncio 3 non era affatto efficace.
>
>Senza le conversioni offline, l&#39;inserzionista probabilmente investirebbe più soldi in Ad 3. Con i dati di conversione offline, l&#39;inserzionista investirà più probabilmente in Ad 1.

Potete [impostare le conversioni](set-up-facebook-offline-conversions.md) offline di Facebook per inviare le prestazioni degli annunci offline a Facebook.

1. Accertati che l’integrazione [con LaunchPoint di](../../../product-docs/demand-generation/ad-network-integrations/add-facebook-custom-audiences-as-a-launchpoint-service.md) Facebook sia aggiornata.
1. Mappa le fasi del modello del ciclo di ricavi sulle fasi di conversione offline su Facebook.
1. Quando un lead Facebook viene generato da un annuncio lead Facebook e raggiunge una fase mappata, Marketo invia i dati di conversione offline a Facebook diverse volte al giorno tramite un&#39;API sicura e automatizzata. I dati vengono visualizzati nel report Facebook Ads Manager (Gestione annunci Facebook).

>[!MORELIKETHIS]
>
>* [Configurare le conversioni offline di Facebook](set-up-facebook-offline-conversions.md)

>



