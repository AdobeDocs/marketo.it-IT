---
unique-page-id: 557316
description: Definire i filtri per elenchi avanzati - Documentazione di Marketo - Documentazione del prodotto
title: Definire i filtri per elenchi avanzati
exl-id: ab08c5be-0afa-46d5-9f29-99e1f6b99dea
feature: Smart Lists
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 0%

---

# Definire i filtri per elenchi avanzati {#define-smart-list-filters}

>[!PREREQUISITES]
>
>* [Creare un elenco avanzato](create-a-smart-list.md)
>* [Trovare ed aggiungere filtri agli elenchi avanzati](find-and-add-filters-to-a-smart-list.md)

Ora che hai [ha creato un elenco avanzato](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) e [filtri aggiunti](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md) definiamo i filtri. Ecco come.

Continuando il nostro esempio, definiamo questi filtri per trovare tutte le persone in California con un punteggio superiore a 50.

1. Vai a **Attività di marketing**.

   ![](assets/login-marketing-activities-1.png)

1. Seleziona l’elenco avanzato e fai clic su **Elenco avanzato** scheda.

   ![](assets/smarlist-choosefilters.png)

1. Trova e seleziona **CA** per **Stato** filtro.

   ![](assets/smartlistdefinefilters.png)

   >[!NOTE]
   >
   >È possibile che siano archiviati entrambi **California** e **CA**. Per filtrare entrambi i valori e includere _tutto_ persone dalla California, imparare a  [aggiungere più valori a un filtro elenco avanzato](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-multiple-values-to-a-smart-list-filter.md).

1. Scegli il **maggiore di** e immettere **50**.

   ![](assets/smartlistfilter-personscore.png)

>[!TIP]
>
>Se pensi di avere alcuni record nel tuo database che contengono indirizzi e-mail incompleti (ad esempio, solo &quot;@adobe.com&quot;), utilizza **due** I filtri per l’indirizzo e-mail quando utilizzi l’operatore &quot;contiene&quot;. Un filtro con &quot;contiene @adobe.com&quot; e un filtro separato con &quot;contiene adobe.com&quot; (omettendo il simbolo @).

Ora sai come creare un elenco avanzato e aggiungere/definire filtri.
