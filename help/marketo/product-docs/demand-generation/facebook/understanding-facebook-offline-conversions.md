---
unique-page-id: 11383945
description: Informazioni sulle conversioni offline di Facebook - Documentazione di Marketo - Documentazione del prodotto
title: Informazioni sulle conversioni offline di Facebook
exl-id: e0995ebc-47fb-4f10-b767-4fe9f572b2d2
feature: Integrations
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '224'
ht-degree: 0%

---

# Informazioni su [!DNL Facebook] conversioni offline {#understanding-facebook-offline-conversions}

Le campagne Facebook Lead Ads generano lead e li inviano a Marketo per l’utilizzo in campagne di marketing. Tuttavia, senza visibilità sulle conversioni offline, l&#39;inserzionista [!DNL Facebook] non può sapere quali annunci sono più efficaci. Ecco un esempio.

>[!NOTE]
>
>**Esempio**
>
>[!UICONTROL Facebook Lead Ads] esegue tre annunci.
>
>* L’annuncio 1 genera 20 lead
>* L’annuncio 2 genera 30 lead
>* L’annuncio 3 genera 50 lead
>
>Solo sulla base di questi numeri, l’annuncio 3 sembra il più efficace.
>
>Tuttavia, osservando i dati sul lato Marketo, si sviluppa una storia diversa.
>
>* L&#39;annuncio 1 genera 10 vendite
>* L’annuncio 3 genera 2 vendite
>
>Ciò significa che l’annuncio 1, nonostante la generazione di meno lead, aveva un tasso di successo del 50%, mentre l’annuncio 3 non era affatto efficace.
>
>Senza conversioni offline, l&#39;inserzionista probabilmente investirebbe più soldi in Ad 3. Con i dati di conversione offline, l’inserzionista investirà più probabilmente in Ad 1.

Puoi [configurare le conversioni offline di Facebook](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions.md) per inviare le prestazioni degli annunci offline a [!DNL Facebook].

1. Assicurarsi che l&#39;integrazione [[!DNL Facebook] [!UICONTROL LaunchPoint]](/help/marketo/product-docs/demand-generation/ad-network-integrations/add-facebook-custom-audiences-as-a-launchpoint-service.md) sia aggiornata.
1. Mappare le fasi nel modello del ciclo dei ricavi alle fasi di conversione offline in [!DNL Facebook].
1. Quando un lead [!DNL Facebook] viene generato da un annuncio lead [!DNL Facebook] e raggiunge una fase mappata, Marketo invia i dati di conversione offline a [!DNL Facebook] diverse volte al giorno tramite un&#39;API protetta e automatizzata. I dati vengono visualizzati nel report di [!DNL Facebook] Ads Manager.

>[!MORELIKETHIS]
>
>[Configura [!DNL Facebook] Conversioni offline](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-offline-conversions.md)
