---
unique-page-id: 557316
description: Definire i filtri per elenchi avanzati - Documentazione di Marketo - Documentazione del prodotto
title: Definire i filtri per elenchi avanzati
exl-id: ab08c5be-0afa-46d5-9f29-99e1f6b99dea
feature: Smart Lists
source-git-commit: 4bf27f7eb534ec76983a898d020f0b8c336a36dc
workflow-type: tm+mt
source-wordcount: '185'
ht-degree: 0%

---

# Definire i filtri per elenchi avanzati {#define-smart-list-filters}

>[!PREREQUISITES]
>
>* [Creare un elenco avanzato](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"}
>* [Trova e aggiungi filtri agli elenchi avanzati](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"}

Ora che hai [creato un elenco avanzato](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md){target="_blank"} e [aggiunto filtri](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md){target="_blank"}, definiamo i filtri. Ecco come.

Continuando il nostro esempio, definiamo questi filtri per trovare tutte le persone in California con un punteggio superiore a 50.

1. Vai a **[!UICONTROL Attività di marketing]**.

   ![](assets/define-smart-list-filters-1.png)

1. Selezionare l&#39;elenco avanzato desiderato e fare clic sulla scheda **[!UICONTROL Elenco avanzato]**.

   ![](assets/define-smart-list-filters-2.png)

1. Trova e seleziona &quot;CA&quot; per il filtro **[!UICONTROL State]**.

   ![](assets/define-smart-list-filters-3.png)

   >[!NOTE]
   >
   >Potresti memorizzare sia &quot;California&quot; che &quot;CA&quot;. Per filtrare entrambi i valori e includere _tutte_ persone dalla California, scopri come [aggiungere più valori a un filtro Elenco avanzato](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-multiple-values-to-a-smart-list-filter.md){target="_blank"}.

1. Scegli l&#39;operatore **[!UICONTROL maggiore di]** e immetti &quot;50&quot;.

   ![](assets/define-smart-list-filters-4.png)

>[!TIP]
>
>Se ritieni di poter avere alcuni record nel database che contengono indirizzi e-mail incompleti (ad esempio, solo &quot;@adobe.com&quot;), utilizza due filtri per l’indirizzo e-mail quando utilizzi l’operatore &quot;contiene&quot;. Un filtro con &quot;contiene @adobe.com&quot; e un filtro separato con &quot;contiene adobe.com&quot; (omettendo il simbolo @).

Ora sai come creare un elenco avanzato e aggiungere/definire filtri.
