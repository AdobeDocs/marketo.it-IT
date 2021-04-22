---
unique-page-id: 1146901
description: Utilizzo della logica avanzata delle regole dell’elenco avanzato - Documentazione di Marketo - Documentazione del prodotto
title: Utilizzo della logica avanzata delle regole dell’elenco avanzato
exl-id: fc41b6fd-c65e-4c44-b0ee-7bb5c77c51fb
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '288'
ht-degree: 0%

---

# Utilizzo della logica avanzata delle regole dell’elenco avanzato {#using-advanced-smart-list-rule-logic}

Puoi trovare le persone giuste applicando la logica della regola di elenco avanzato a più filtri all’interno di un elenco avanzato. Ecco come.

>[!PREREQUISITES]
>
>* [Ricerca e aggiunta di filtri a un elenco avanzato](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)
>* [Definire i filtri degli elenchi avanzati](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/define-smart-list-filters.md)


>[!NOTE]
>
>La logica di filtro avanzata è disponibile solo se sono presenti tre o più filtri nell’elenco avanzato.

## Aggiungi logica a un elenco avanzato {#add-logic-to-a-smart-list}

Per impostazione predefinita, nell’elenco smart sono presenti le persone che corrispondono ai filtri **ALL** (filtri 1 _e_ 2 _e_ 3). È possibile modificare la logica delle regole per individuare le persone corrispondenti a **ANY** dei filtri definiti (filtri 1 _o_ 2 _o_ 3) o utilizzare filtri avanzati (filtri 1 _e_ 2 _o_ 3).

In questo esempio, supponiamo che desideri trovare persone in California _e_ con un punteggio di almeno 50 punti _o_ con lo stato &quot;Qualificato per le vendite&quot;.

1. Seleziona **Usa filtri avanzati** dal menu a discesa.

   ![](assets/one.png)

   >[!NOTE]
   >
   >L’utilizzo di filtri **Avanzate** riduce la necessità di creare elenchi avanzati con il filtro Membro di Smart List. Questo consente di ottimizzare le prestazioni.

1. La casella di testo **Filtri avanzati** visualizza &quot;e&quot; come valore predefinito tra tutti i filtri.

   ![](assets/two-2.png)

1. Digita un paio di parentesi intorno a &quot;2 e 3&quot;.

   ![](assets/three-2.png)

   >[!CAUTION]
   >
   >È necessario utilizzare &quot;e&quot; prima di &quot;o&quot; quando si immette la logica delle regole.

1. Cambia il valore &quot;e&quot; tra &quot;2 e 3&quot; in &quot;o&quot;.

   ![](assets/four-1.png)

## Usa le parentesi quando mischi &quot;And&quot; e &quot;Or {#use-parentheses-when-mixing-and-and-or}

La combinazione di logica &quot;e&quot; e &quot;o&quot; richiede parentesi per chiarire la tua intenzione.

![](assets/advancedfilters-parent.png)

## Usa parentesi nidificate per quattro o più filtri se necessario {#use-nested-parentheses-for-four-or-more-filters-if-needed}

A seconda delle tue intenzioni, potresti dover aggiungere parentesi nidificate quando utilizzi quattro o più filtri.

![](assets/advancedfilters-nested.png)

>[!TIP]
>
>Se immetti una regola non valida, sotto la regola viene visualizzata una linea rossa. Scorri il testo per visualizzare il relativo messaggio di errore.
