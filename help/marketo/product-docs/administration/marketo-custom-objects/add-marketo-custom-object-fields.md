---
unique-page-id: 10093688
description: Aggiungi campi di oggetti personalizzati Marketo - Documenti Marketo - Documentazione del prodotto
title: Aggiungi campi oggetto personalizzati Marketo
translation-type: tm+mt
source-git-commit: 65182770291dc14fbe915a40403fc09b433aae86
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---


# Aggiungi campi oggetto personalizzati Marketo {#add-marketo-custom-object-fields}

Dopo aver creato un oggetto personalizzato, è necessario aggiungergli dei campi per soddisfare le esigenze aziendali.

I campi definiscono le informazioni specifiche utilizzate da un oggetto personalizzato. I campi di collegamento hanno un lavoro speciale, per collegare oggetti personalizzati e sono trattati in un [articolo separato](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md).

1. Fare clic su **Amministratore** e in **Gestione database** selezionare **Oggetti personalizzati Marketo**.

   ![](assets/image2016-1-18-9-3a2-3a6.png)

1. Selezionare l’oggetto a cui si desidera aggiungere il campo a destra.

   ![](assets/image2016-1-18-9-3a5-3a3.png)

1. Nella scheda **Campi** , fai clic su **Nuovo campo**.

   ![](assets/image2015-9-15-16-3a53-3a40.png)

   >[!NOTE]
   >
   >I tre campi indicati sopra vengono creati automaticamente da Marketo al momento della creazione di un oggetto personalizzato. Marketo gestisce automaticamente questi campi e non è possibile modificarli o eliminarli.

1. Immetti un nome e una descrizione visualizzati.

   ![](assets/image2015-10-5-11-3a35-3a48.png)

   >[!NOTE]
   >
   >Il nome dell’API può essere modificato solo fino all’approvazione.

1. A questo punto, scegli un tipo di dati appropriato dall’elenco.

   ![](assets/image2015-10-5-11-3a37-3a24.png)

1. Se desideri utilizzare il nuovo campo come identificatore univoco, solleva il cursore Dedupe. Fai clic su **Salva** per terminare.

   ![](assets/image2015-10-5-11-3a40-3a12.png)

   >[!TIP]
   >
   >I campi di deduplicazione possono essere utilizzati per recuperare, aggiornare o eliminare oggetti personalizzati. Ogni definizione di oggetto personalizzato deve contenere almeno un campo di deduplicazione (e non più di tre).

1. Aggiungi tutti gli altri campi necessari.

   >[!NOTE]
   >
   >Se stai creando una struttura uno-a-molti, devi aggiungere un campo Collegamento all’oggetto personalizzato. Per una struttura molti-a-molti, non è necessario un campo di collegamento nell’oggetto personalizzato, ma è necessario aggiungere due campi di collegamento nell’oggetto intermedio. Per ulteriori informazioni sui tipi di oggetti personalizzati, consulta [Aggiungi campi di collegamento oggetto personalizzato Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md) e [Informazioni sugli oggetti personalizzati Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) .

>[!MORELIKETHIS]
>
>* [Aggiungi campi di collegamento a oggetti personalizzati Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md)
>* [Modificare ed eliminare un oggetto personalizzato Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-a-marketo-custom-object.md)
>* [Modificare ed eliminare i campi oggetto personalizzati Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-marketo-custom-object-fields.md)
>* [Informazioni sugli oggetti personalizzati Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)

