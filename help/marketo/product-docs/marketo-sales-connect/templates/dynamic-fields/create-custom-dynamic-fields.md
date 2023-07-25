---
unique-page-id: 14352508
description: Creare campi dinamici personalizzati - Documentazione di Marketo - Documentazione del prodotto
title: Creare campi dinamici personalizzati
exl-id: 860511d2-4a8a-47a4-8362-ba4e715e44e9
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---

# Creare campi dinamici personalizzati {#create-custom-dynamic-fields}

Esistono due modi per creare campi dinamici personalizzati.

## Salvataggio dei campi personalizzati per uno o più contatti {#saving-custom-fields-for-one-or-a-few-contacts}

1. Fare clic sul nome di un contatto nella pagina Persone.

1. Scegli l’elenco a discesa accanto a Annulla iscrizione e seleziona **Modifica**.

1. Scorri verso il basso fino alla parte inferiore della pagina di modifica. Puoi quindi creare un nome e un valore per il campo.

1. Clic **Salva**.

## Salvataggio di campi personalizzati per molti contatti {#saving-custom-fields-for-many-contacts}

1. Crea un foglio di calcolo CSV con i campi personalizzati nella rispettiva colonna.

1. Segui le [normale processo di caricamento CSV](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md), interrompendosi nella schermata di mappatura campi.

1. Invece di uno dei campi predefiniti, scegli **Aggiungi un nuovo campo personalizzato** dal menu a discesa.

1. Inserisci il nome del campo desiderato e fai clic su **OK**.

1. Completa il caricamento del file CSV. I contatti verranno forniti con il campo personalizzato aggiunto.

>[!NOTE]
>
>Dopo aver creato il campo personalizzato, potrebbero essere necessari circa 30 minuti affinché venga visualizzato nel menu a discesa del campo dinamico nell’editor modelli.

## Come utilizzare i campi personalizzati in un modello {#how-to-use-your-custom-fields-in-a-template}

Una volta archiviati i campi personalizzati con i metodi di cui sopra, potrai fare riferimento a essi nei modelli.

1. [Creare un modello](/help/marketo/product-docs/marketo-sales-connect/templates/create-a-new-template.md) e fai clic su **Campi dinamici** come faresti normalmente.

1. Seleziona **Campi personalizzati** dall’elenco a discesa visualizzato.

1. Potrai visualizzare i campi personalizzati pre-memorizzati e selezionarne uno da compilare nel modello.
