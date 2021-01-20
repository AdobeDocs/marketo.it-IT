---
unique-page-id: 1146901
description: Utilizzo della logica avanzata della regola degli elenchi avanzati - Documenti Marketo - Documentazione del prodotto
title: Utilizzo della logica delle regole avanzate per gli elenchi avanzati
translation-type: tm+mt
source-git-commit: 5b9f48c98464c79bcdca2e335f6a4a2edce98ce4
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---


# Utilizzo della logica della regola avanzata dell&#39;elenco avanzato {#using-advanced-smart-list-rule-logic}

Potete trovare le persone esatte necessarie applicando la logica della regola di elenchi avanzati a più filtri all&#39;interno di un elenco avanzato. Ecco come.

>[!PREREQUISITES]
>
>* [Trovare e aggiungere filtri a un elenco avanzato](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)
>* [Definire i filtri per elenchi avanzati](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/define-smart-list-filters.md)


>[!NOTE]
>
>La logica di filtro avanzata è disponibile solo se sono presenti tre o più filtri nell’elenco avanzato.

## Aggiungere una logica a un elenco avanzato {#add-logic-to-a-smart-list}

Per impostazione predefinita, nell&#39;elenco smart vengono visualizzate le persone che corrispondono ai filtri **ALL** (filtri 1 _e_ 2 _e_ 3). È possibile modificare la logica delle regole per individuare le persone che corrispondono a **ANY** dei filtri definiti (filtri 1 _o_ 2 _o_ 3), oppure utilizzare filtri avanzati (filtri 1 _e_ 2 _o_ 3).

In questo esempio, supponiamo di voler trovare persone in California _e_ con un punteggio di almeno 50 punti _o_ con lo stato &quot;Sales Qualified&quot;.

1. Selezionare **Usa filtri avanzati** dall&#39;elenco a discesa.

   ![](assets/one.png)

   >[!NOTE]
   >
   >L&#39;utilizzo di filtri **Advanced** riduce la necessità di creare elenchi avanzati con il filtro Member of Smart List. Questo consente di ottimizzare le prestazioni.

1. La casella di testo **Filtri avanzati** visualizzerà &quot;e&quot; come valore predefinito tra tutti i filtri.

   ![](assets/two-2.png)

1. Digitare un paio di parentesi intorno a &quot;2 e 3&quot;.

   ![](assets/three-2.png)

   >[!CAUTION]
   >
   >È necessario utilizzare &quot;and&quot; prima di &quot;or&quot; quando si immette la logica della regola.

1. Cambia &quot;e&quot; tra &quot;2 e 3&quot; e &quot;or&quot;.

   ![](assets/four-1.png)

## Utilizzare le parentesi per il mixaggio &quot;And&quot; e &quot;OR {#use-parentheses-when-mixing-and-and-or}

La combinazione di logica &quot;and&quot; e &quot;or&quot; richiede parentesi per chiarire la propria intenzione.

![](assets/advancedfilters-parent.png)

## Usa parentesi nidificate per quattro o più filtri, se necessario{#use-nested-parentheses-for-four-or-more-filters-if-needed}

A seconda delle intenzioni, potrebbe essere necessario aggiungere parentesi nidificate quando si utilizzano quattro o più filtri.

![](assets/advancedfilters-nested.png)

>[!TIP]
>
>Se si immette una regola non valida, sotto la regola verrà visualizzata una linea rossa. Scorrete il testo per visualizzare il relativo messaggio di errore.
