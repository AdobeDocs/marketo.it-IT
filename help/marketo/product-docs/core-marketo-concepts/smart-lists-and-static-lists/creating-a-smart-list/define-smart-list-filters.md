---
unique-page-id: 557316
description: Definire i filtri degli elenchi avanzati - Documenti Marketo - Documentazione del prodotto
title: Definire i filtri degli elenchi avanzati
exl-id: ab08c5be-0afa-46d5-9f29-99e1f6b99dea
source-git-commit: 4b1b91a933a7a6d103fe0d44ece9ea95759edc5f
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 0%

---

# Definire i filtri degli elenchi avanzati {#define-smart-list-filters}

>[!PREREQUISITES]
>
>* [Creare un elenco avanzato](create-a-smart-list.md)
>* [Ricerca e aggiunta di filtri agli elenchi avanzati](find-and-add-filters-to-a-smart-list.md)


Ora che hai [creazione di un elenco smart](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) e [filtri aggiunti](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md) definiamo i filtri. Ecco come.

Continuando il nostro esempio, definiamo questi filtri per trovare tutte le persone in California con un punteggio superiore a 50.

1. Vai a **Attività di marketing**.

   ![](assets/login-marketing-activities-1.png)

1. Seleziona l’elenco avanzato e fai clic sul pulsante **Elenco avanzato** scheda .

   ![](assets/smarlist-choosefilters.png)

1. Trova e seleziona **CA** per **Stato** filtro.

   ![](assets/smartlistdefinefilters.png)

   >[!NOTE]
   >
   >È possibile memorizzare entrambi **California** e **CA**. Per filtrare entrambi i valori e includere _tutto_ persone dalla California, impara come  [aggiungere più valori a un filtro elenco avanzato](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/using-smart-lists/add-multiple-values-to-a-smart-list-filter.md).

1. Scegli la **maggiore di** operatore ed immetti **50**.

   ![](assets/smartlistfilter-personscore.png)

>[!TIP]
>
>Se pensi di avere alcuni record nel database che contengono indirizzi e-mail incompleti (ad esempio, solo &quot;@adobe.com&quot;), utilizza **due** L’indirizzo e-mail filtra quando utilizzi l’operatore &quot;contiene&quot;. Un filtro con &quot;contiene @adobe.com&quot; e un filtro separato con &quot;contiene adobe.com&quot; (lasciando fuori il simbolo @).

Ora è possibile creare un elenco avanzato e aggiungere/definire filtri.
