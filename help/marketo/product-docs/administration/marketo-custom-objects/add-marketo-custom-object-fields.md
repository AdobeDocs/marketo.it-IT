---
unique-page-id: 10093688
description: Aggiungi campi oggetto personalizzati Marketo - Documenti Marketo - Documentazione prodotto
title: Aggiungi campi oggetto personalizzati Marketo
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---


# Aggiungi campi oggetto personalizzati Marketo {#add-marketo-custom-object-fields}

Dopo aver creato un oggetto personalizzato, è necessario aggiungere campi per soddisfare le esigenze aziendali.

I campi definiscono le informazioni specifiche utilizzate da un oggetto personalizzato. I campi di collegamento hanno un lavoro speciale, per collegare oggetti personalizzati e sono trattati in un [articolo separato](add-marketo-custom-object-link-fields.md).

1. Fare clic su **Admin** e in **Database Management** selezionare **Marketo Custom Objects**.

   ![](assets/image2016-1-18-9-3a2-3a6.png)

1. Selezionare l&#39;oggetto a cui si desidera aggiungere il campo sulla destra.

   ![](assets/image2016-1-18-9-3a5-3a3.png)

1. Nella scheda **Fields **, fare clic su **New Field**.

   ![](assets/image2015-9-15-16-3a53-3a40.png)

   >[!NOTE]
   >
   >I tre campi indicati sopra vengono creati automaticamente da Marketo quando si crea un oggetto personalizzato. Marketo gestisce automaticamente questi campi e non è possibile modificarli o eliminarli.

1. Immettete un nome e una descrizione da visualizzare.

   ![](assets/image2015-10-5-11-3a35-3a48.png)

   >[!NOTE]
   >
   >Il nome dell&#39;API può essere modificato solo fino all&#39;approvazione.

1. A questo punto, scegliete un tipo di dati appropriato dall’elenco.

   ![](assets/image2015-10-5-11-3a37-3a24.png)

1. Se desiderate usare il nuovo campo come identificatore univoco, trascinate il cursore Dedupe. Fare clic su **Save **per terminare.

   ![](assets/image2015-10-5-11-3a40-3a12.png)

   >[!TIP]
   >
   >Quando create un campo duplicato, potete utilizzarlo per rimuovere i campi duplicati nel database.

1. Aggiungete eventuali altri campi.

   >[!NOTE]
   >
   >**Promemoria**
   >
   >
   >Se si sta creando una struttura uno-molti, è necessario aggiungere un campo Collegamento all&#39;oggetto personalizzato. Per una struttura molti-a-molti, non è necessario un campo di collegamento nell&#39;oggetto personalizzato, ma è necessario aggiungere due campi di collegamento nell&#39;oggetto intermedio. Per ulteriori informazioni sui tipi di oggetti personalizzati, vedere [Aggiunta di campi di collegamento oggetto personalizzato a Marketo](add-marketo-custom-object-link-fields.md) e [Informazioni sugli oggetti personalizzati a Marketo](understanding-marketo-custom-objects.md).

>[!MORELIKETHIS]
>
>* [Aggiungi campi collegamento oggetto personalizzato marketing](add-marketo-custom-object-link-fields.md)
>* [Modifica ed eliminazione di un oggetto personalizzato Marketo](edit-and-delete-a-marketo-custom-object.md)
>* [Informazioni sugli oggetti personalizzati Marketo](understanding-marketo-custom-objects.md)
>* [Modifica ed eliminazione dei campi oggetto personalizzati Marketo](edit-and-delete-marketo-custom-object-fields.md)

>



