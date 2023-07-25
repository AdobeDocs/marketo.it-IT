---
unique-page-id: 1146901
description: Utilizzo della logica avanzata per le regole di elenco avanzato - Documentazione di Marketo - Documentazione del prodotto
title: Utilizzo della logica avanzata della regola di elenco avanzato
exl-id: fc41b6fd-c65e-4c44-b0ee-7bb5c77c51fb
feature: Smart Lists
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# Utilizzo della logica avanzata della regola di elenco avanzato {#using-advanced-smart-list-rule-logic}

Per trovare le persone giuste necessarie, applica una logica di regola per un elenco avanzato a più filtri all’interno di un elenco avanzato. Ecco come.

>[!PREREQUISITES]
>
>* [Trovare e aggiungere filtri a un elenco avanzato](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)
>* [Definire i filtri per elenchi avanzati](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/define-smart-list-filters.md)

>[!NOTE]
>
>La logica di filtro avanzata è disponibile solo se nell’elenco avanzato sono presenti tre o più filtri.

## Aggiungere logica a un elenco avanzato {#add-logic-to-a-smart-list}

Per impostazione predefinita, l’elenco avanzato individua le persone corrispondenti **TUTTI** filtri (filtri 1) _e_ 2 _e_ 3). Puoi cambiare la logica della regola per trovare le persone che corrispondono a **QUALSIASI** dei filtri definiti (filtri 1 _o_ 2 _o_ 3), oppure utilizzare filtri avanzati (filtri 1 _e_ 2 _o_ 3).

In questo esempio, supponiamo che tu voglia trovare persone in California _e_ con un punteggio di almeno 50 punti _o_ con lo stato &quot;Vendite qualificate&quot;.

1. Seleziona **Utilizzare filtri avanzati** dal menu a discesa.

   ![](assets/one.png)

   >[!NOTE]
   >
   >Utilizzo di **Avanzate** I filtri riducono la necessità di creare elenchi avanzati con il filtro Membro di elenco avanzato. Questo consente di ottimizzare le prestazioni.

1. Il **Filtri avanzati** La casella di testo visualizzerà &quot;e&quot; come valore predefinito tra tutti i filtri.

   ![](assets/two-2.png)

1. Digita una coppia di parentesi intorno a &quot;2 e 3&quot;.

   ![](assets/three-2.png)

   >[!CAUTION]
   >
   >Utilizza &quot;e&quot; prima di &quot;o&quot; quando immetti la logica della regola.

1. Modificare &quot;and&quot; tra &quot;2 e 3&quot; in &quot;or&quot;.

   ![](assets/four-1.png)

## Utilizzare Le Parentesi Quando Si Miscelano &quot;And&quot; E &quot;Or&quot; {#use-parentheses-when-mixing-and-and-or}

La combinazione delle logiche &quot;and&quot; e &quot;or&quot; richiede parentesi per rendere chiara la tua intenzione.

![](assets/advancedfilters-parent.png)

## Usa parentesi nidificate per quattro o più filtri, se necessario {#use-nested-parentheses-for-four-or-more-filters-if-needed}

A seconda dell’intenzione, potrebbe essere necessario aggiungere parentesi nidificate quando si utilizzano quattro o più filtri.

![](assets/advancedfilters-nested.png)

>[!TIP]
>
>Se si immette una regola non valida, sotto la regola verrà visualizzata una riga rossa. Scorri il testo per visualizzare il relativo messaggio di errore.
