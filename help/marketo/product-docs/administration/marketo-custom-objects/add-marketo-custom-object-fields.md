---
unique-page-id: 10093688
description: Aggiungere campi oggetto personalizzati Marketo - Documentazione Marketo - Documentazione del prodotto
title: Aggiungi campi oggetto personalizzati Marketo
exl-id: 6d776d97-93e2-4708-9ce5-2172e02b71c3
feature: Custom Objects
source-git-commit: 99c38fd24631e94a9554bf09de11e8eb607150d6
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---

# Aggiungi campi oggetto personalizzati Marketo {#add-marketo-custom-object-fields}

Dopo aver creato un oggetto personalizzato, devi aggiungervi dei campi per soddisfare le tue esigenze aziendali.

I campi definiscono le informazioni specifiche utilizzate da un oggetto personalizzato. I campi di collegamento hanno un processo speciale per connettere oggetti personalizzati e sono trattati in un [articolo separato](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md).

1. Vai all&#39;area **[!UICONTROL Amministratore]**.

   ![](assets/add-marketo-custom-object-fields-1.png)

1. Fare clic su **[!UICONTROL Oggetti personalizzati Marketo]**.

   ![](assets/add-marketo-custom-object-fields-2.png)

1. Selezionare l&#39;oggetto a cui si desidera aggiungere il campo a destra.

   ![](assets/add-marketo-custom-object-fields-3.png)

1. Fai clic sulla scheda **[!UICONTROL Campi]**, quindi **[!UICONTROL Nuovo campo]**.

   ![](assets/add-marketo-custom-object-fields-4.png)

   >[!NOTE]
   >
   >I tre campi mostrati sopra vengono creati automaticamente da Marketo quando si crea un oggetto personalizzato. Marketo gestisce questi campi automaticamente e non è possibile modificarli o eliminarli.

1. Immettere un [!UICONTROL Nome visualizzato] e (facoltativo) [!UICONTROL Descrizione].

   ![](assets/add-marketo-custom-object-fields-5.png)

   >[!NOTE]
   >
   >Il nome API può essere modificato solo fino a quando non viene approvato.

1. Scegliere un tipo di dati [!UICONTROL appropriato] dall&#39;elenco.

   ![](assets/add-marketo-custom-object-fields-6.png)

1. Per utilizzare il nuovo campo come identificatore univoco, trascina il cursore [!UICONTROL Dedupe]. Fai clic su **[!UICONTROL Salva]** per terminare.

   ![](assets/add-marketo-custom-object-fields-7.png)

   >[!TIP]
   >
   >I campi di deduplicazione possono essere utilizzati per recuperare, aggiornare o eliminare oggetti personalizzati. Ogni definizione di oggetto personalizzato deve contenere almeno un campo di deduplicazione (e non più di tre).

1. Aggiungi tutti gli altri campi necessari.

   >[!NOTE]
   >
   >Se stai creando una struttura uno-a-molti, devi aggiungere un campo Collegamento all&#39;oggetto personalizzato. Per una struttura molti-a-molti, non è necessario un campo collegamento nell&#39;oggetto personalizzato, ma è necessario aggiungere due campi collegamento nell&#39;oggetto intermedio. Per ulteriori informazioni sui tipi di oggetti personalizzati, vedere [Aggiungere campi collegamento di oggetti personalizzati di Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md) per creare i campi collegamento e [Informazioni sugli oggetti personalizzati di Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md).

>[!MORELIKETHIS]
>
>* [Aggiungi campi collegamento oggetto personalizzato Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md)
>* [Modifica ed elimina un oggetto personalizzato di Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-a-marketo-custom-object.md)
>* [Modifica ed elimina campi oggetto personalizzati di Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-marketo-custom-object-fields.md)
>* [Informazioni sugli oggetti personalizzati di Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
