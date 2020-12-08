---
unique-page-id: 4719312
description: Aggiungere/rimuovere i valori degli elenchi di prelievo - Documenti Marketo - Documentazione prodotto
title: Aggiungi/rimuovi valori elenco di selezione
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---


# Aggiungi/rimuovi valori elenco di selezione {#add-remove-picklist-values}

Seguono alcune informazioni sull’aggiunta e la rimozione dei valori degli elenchi di selezione in Salesforce.

## Aggiunta Di Valori Di Elenco Di Pagine {#adding-picklist-values}

1. Se a un tipo di campo elenco di selezione viene aggiunto un valore aggiuntivo in Salesforce, riceverai una [notifica](../../../product-docs/core-marketo-concepts/miscellaneous/understanding-notifications.md) che identifica i moduli interessati.

   ![](assets/image2015-1-21-14-3a4-3a7.png)

1. Passate all’editor del modulo e [aggiungete il valore](../../../product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md) aggiuntivo all’elenco dei suggerimenti.

## Rimuovi valori elenco di selezione {#remove-picklist-values}

Quando un valore di elenco di selezione viene rimosso da un campo in Salesforce, sarà necessario rimuovere manualmente questo valore da tutti i moduli che ospitano il campo.

>[!NOTE]
>
>Se un campo lead e un campo di contatto in Salesforce hanno valori diversi, i valori in comune saranno disponibili per l’uso in Marketo.

Se un campo lead e un campo contatto in Salesforce hanno valori diversi:

1. Se si aggiunge un valore aggiuntivo in SFDC a un elenco di selezione, verrà visualizzata una notifica.
1. La notifica vi dirà dove viene utilizzata. È ora possibile aggiungere questo nuovo valore come opzione nel modulo, se lo si desidera.

Se un elenco di selezione di un lead SFDC ha valori diversi rispetto a un elenco di selezione per un contatto SFDC, i valori comuni saranno utilizzati come opzioni di valore predefinite nel modulo.

Se si rimuove un valore da un elenco di selezione, sarà necessario rimuoverlo manualmente come opzione dai moduli.
