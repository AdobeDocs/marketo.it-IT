---
unique-page-id: 14352508
description: Creare campi dinamici personalizzati - Documentazione di Marketo - Documentazione del prodotto
title: Creare campi dinamici personalizzati
exl-id: 860511d2-4a8a-47a4-8362-ba4e715e44e9
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '223'
ht-degree: 4%

---

# Creare campi dinamici personalizzati {#create-custom-dynamic-fields}

Esistono due modi per creare campi dinamici personalizzati.

## Salvataggio dei campi personalizzati per uno o più contatti {#saving-custom-fields-for-one-or-a-few-contacts}

1. Fare clic sul nome di un contatto nella pagina [!UICONTROL People].

1. Scegliere il menu a discesa accanto a [!UICONTROL Unsubscribe] e selezionare **[!UICONTROL Edit]**.

1. Scorri verso il basso fino alla parte inferiore della pagina di modifica. Puoi quindi creare un nome e un valore per il campo.

1. Fai clic su **[!UICONTROL Save]**.

## Salvataggio di campi personalizzati per molti contatti {#saving-custom-fields-for-many-contacts}

1. Crea un foglio di calcolo CSV con i campi personalizzati nella rispettiva colonna.

1. Segui il [normale processo di caricamento CSV](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md), interrompendo la schermata di mappatura campi.

1. Invece di uno dei campi predefiniti, scegli **[!UICONTROL Add a new Custom Field]** dal menu a discesa.

1. Immettere il nome del campo desiderato e fare clic su **[!UICONTROL OK]**.

1. Completa il caricamento del file CSV. I contatti verranno forniti con il campo personalizzato aggiunto.

>[!NOTE]
>
>Dopo aver creato il campo personalizzato, potrebbero essere necessari circa 30 minuti affinché venga visualizzato nel menu a discesa del campo dinamico nell’editor modelli.

## Come utilizzare i campi personalizzati in un modello {#how-to-use-your-custom-fields-in-a-template}

Una volta archiviati i campi personalizzati con i metodi di cui sopra, potrai fare riferimento a essi nei modelli.

1. [Crea un modello](/help/marketo/product-docs/marketo-sales-connect/templates/create-a-new-template.md) e fai clic sul pulsante **[!UICONTROL Dynamic Fields]** come faresti normalmente.

1. Selezionare **[!UICONTROL Custom Fields]** dal menu a discesa visualizzato.

1. Potrai visualizzare i campi personalizzati pre-memorizzati e selezionarne uno da compilare nel modello.
