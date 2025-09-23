---
unique-page-id: 4719312
description: Aggiungere/rimuovere valori dall’elenco di selezione - Documentazione di Marketo - Documentazione del prodotto
title: Aggiungere/Rimuovere valori elenco a discesa
exl-id: f1230c43-10cb-47ff-89d7-9f835b034db0
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 3%

---

# Aggiungere/Rimuovere valori elenco a discesa {#add-remove-picklist-values}

Di seguito sono riportati alcuni aspetti relativi all&#39;aggiunta e alla rimozione dei valori degli elenchi di selezione in [!DNL Salesforce].

## Aggiunta di valori di elenco a discesa {#adding-picklist-values}

1. Se in Salesforce viene aggiunto un valore aggiuntivo a un tipo di campo dell&#39;elenco a discesa, riceverai una [notifica](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications.md){target="_blank"} che identifica i moduli su cui questo influirà.

   ![](assets/image2015-1-21-14-3a4-3a7.png)

1. Vai all&#39;editor dei moduli e [aggiungi il valore aggiuntivo](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md){target="_blank"} all&#39;elenco dei suggerimenti.

## Rimuovi valori elenco a discesa {#remove-picklist-values}

Quando un valore dell&#39;elenco a discesa viene rimosso da un campo in [!DNL Salesforce], sarà necessario rimuovere manualmente questo valore da tutti i moduli che ospitano questo campo.

>[!NOTE]
>
>Se un campo lead e un campo contatto in Salesforce hanno valori diversi, i valori in comune saranno disponibili per l’utilizzo in Marketo Engage.

Se un campo lead e un campo contatto in [!DNL Salesforce] hanno valori diversi:

1. L’aggiunta di un valore aggiuntivo in SFDC a un elenco a discesa genera una notifica.
1. La notifica ti indicherà dove viene utilizzata. È ora possibile aggiungere questo nuovo valore come opzione nel modulo, se necessario.

Se un elenco di selezione di un lead SFDC ha valori diversi rispetto a un elenco di selezione di un contatto SFDC, i valori comuni verranno utilizzati come opzioni di valore predefinite nel modulo.

Se si rimuove un valore da un elenco a discesa, sarà necessario rimuoverlo manualmente come opzione dai moduli.
