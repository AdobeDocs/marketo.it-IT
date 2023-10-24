---
unique-page-id: 557316
description: Definire i filtri per elenchi avanzati - Documentazione di Marketo - Documentazione del prodotto
title: Definire i filtri per elenchi avanzati
exl-id: ab08c5be-0afa-46d5-9f29-99e1f6b99dea
feature: Smart Lists
source-git-commit: 198d7d7fd4c1c312aeb30fa922fd89863ac87f81
workflow-type: tm+mt
source-wordcount: '180'
ht-degree: 0%

---

# Definire i filtri per elenchi avanzati {#define-smart-list-filters}

>[!PREREQUISITES]
>
>* [Creare un elenco avanzato](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}
>* [Trovare ed aggiungere filtri agli elenchi avanzati](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"}

Ora che hai [ha creato un elenco avanzato](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"} and [added filters](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"} definiamo i filtri. Ecco come.

Continuando il nostro esempio, definiamo questi filtri per trovare tutte le persone in California con un punteggio superiore a 50.

1. Vai a **[!UICONTROL Attività di marketing]**.

   ![](assets/login-marketing-activities-1.png)

1. Seleziona lo Smart List e fai clic su **[!UICONTROL Elenco avanzato]** scheda.

   ![](assets/smarlist-choosefilters.png)

1. Trova e seleziona &quot;CA&quot; per **[!UICONTROL Stato]** filtro.

   ![](assets/smartlistdefinefilters.png)

   >[!NOTE]
   >
   >Potresti memorizzare sia &quot;California&quot; che &quot;CA&quot;. Per filtrare entrambi i valori e includere _tutto_ persone dalla California, imparare a  [aggiungere più valori a un filtro Elenco avanzato](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-multiple-values-to-a-smart-list-filter.md){target="_blank"}.

1. Scegli il **[!UICONTROL maggiore di]** e immettere &quot;50&quot;.

   ![](assets/smartlistfilter-personscore.png)

>[!TIP]
>
>Se ritieni di poter avere alcuni record nel database che contengono indirizzi e-mail incompleti (ad esempio, solo &quot;@adobe.com&quot;), utilizza due filtri per l’indirizzo e-mail quando utilizzi l’operatore &quot;contiene&quot;. Un filtro con &quot;contiene @adobe.com&quot; e un filtro separato con &quot;contiene adobe.com&quot; (omettendo il simbolo @).

Ora sai come creare un elenco avanzato e aggiungere/definire filtri.
