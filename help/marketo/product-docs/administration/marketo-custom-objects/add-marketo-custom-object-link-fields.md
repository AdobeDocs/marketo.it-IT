---
unique-page-id: 10097613
description: Aggiungi Marketo Custom Object Link Fields - Marketo Docs - Documentazione prodotto
title: Aggiungi campi collegamento oggetto personalizzato marketing
translation-type: tm+mt
source-git-commit: f865630638e7c0fe6ac2a449e196a7de4fbfeea1
workflow-type: tm+mt
source-wordcount: '601'
ht-degree: 0%

---


# Aggiungi campi collegamento oggetto personalizzato Marketo {#add-marketo-custom-object-link-fields}

Quando si creano oggetti personalizzati, è necessario fornire campi di collegamento per collegare il record oggetto personalizzato al record padre corretto.

* Per una struttura personalizzata uno-molti, utilizzare il campo di collegamento nell&#39;oggetto personalizzato per collegarlo a una persona o una società.
* Per una struttura molti-molti, si utilizzano due campi di collegamento, collegati da un oggetto intermedio creato separatamente (anch&#39;esso un tipo di oggetto personalizzato). Un collegamento si collega alle persone o alle società presenti nel database e l&#39;altro all&#39;oggetto personalizzato. In questo caso, il campo del collegamento non si trova nello stesso oggetto personalizzato.

## Creare un campo collegamento per una struttura uno-molti {#create-a-link-field-for-a-one-to-many-structure}

Come creare un campo di collegamento in un oggetto personalizzato per una struttura uno-molti.

1. Fare clic su **Admin** e in **Database Management** selezionare **Marketo Custom Objects**.

   ![](assets/image2016-1-18-13-3a25-3a11.png)

1. Selezionare l&#39;oggetto personalizzato nell&#39;elenco.

   ![](assets/image2016-1-14-15-3a6-3a2.png)

1. Nella scheda **Campi** fare clic su **Nuovo campo**.

   ![](assets/image2015-9-17-14-3a9-3a19.png)

1. Denominate il campo del collegamento e aggiungete una descrizione facoltativa. Accertatevi di selezionare il tipo di dati Collegamento.

   ![](assets/image2015-10-5-13-3a24-3a57.png)

   >[!CAUTION]
   >
   >Non potrai tornare indietro e creare, modificare o eliminare un collegamento o un campo dedicato dopo l&#39;approvazione dell&#39;oggetto personalizzato.

1. Selezionare se l&#39;oggetto collegamento è relativo a un lead (persona) o a una società.

   ![](assets/image2015-10-5-13-3a28-3a1.png)

   >[!NOTE]
   >
   >Se scegliete un lead, nell’elenco verranno visualizzati ID, indirizzo e-mail ed eventuali campi personalizzati.
   >
   >Se scegliete una società, nell&#39;elenco verranno visualizzati Id ed eventuali campi personalizzati.

1. Selezionare il campo di collegamento a cui si desidera connettersi come padre del nuovo campo.

   ![](assets/image2015-10-5-13-3a30-3a6.png)

   >[!NOTE]
   >
   >Nel campo del collegamento sono supportati solo i tipi di campo stringa.

1. Fare clic su **Salva.**

   ![](assets/image2015-10-5-13-3a34-3a0.png)

## Creare un campo collegamento per una struttura molti-molti {#create-a-link-field-for-a-many-to-many-structure}

Come creare un campo di collegamento in un oggetto intermediario da utilizzare in una struttura molti-a-molti.

>[!PREREQUISITES]
>
>È necessario aver già creato l&#39;oggetto intermediario ed eventuali oggetti personalizzati a cui si desidera collegarlo.

1. Fare clic su **Admin** e in **Database Management** selezionare **Marketo Custom Objects**.

   ![](assets/image2016-1-18-9-3a8-3a14.png)

1. Selezionare l&#39;oggetto intermedio a cui si desidera aggiungere il campo.

   ![](assets/image2016-1-18-9-3a10-3a29.png)

1. Nella scheda **Campi** fare clic su **Nuovo campo**.

   ![](assets/image2016-1-18-9-3a31-3a43.png)

1. È necessario creare due campi di collegamento. Create loro uno alla volta. Innanzitutto, assegnare un nome al campo per i membri dell’elenco del database (ad esempio, il codice leadID). Aggiungete una descrizione facoltativa. Assicurarsi di selezionare il tipo di dati del collegamento.

   ![](assets/image2016-1-18-9-3a38-3a59.png)

   >[!CAUTION]
   >
   >Non potrai tornare indietro e creare, modificare o eliminare un collegamento o un campo dedicato dopo l&#39;approvazione dell&#39;oggetto personalizzato.

1. Selezionare l&#39;oggetto collegamento dal database, in questo caso Lead.

   ![](assets/image2016-1-18-9-3a50-3a48.png)

1. Selezionate il campo di collegamento a cui desiderate connettervi, in questo caso, all&#39;ID.

   ![](assets/image2016-1-18-9-3a53-3a54.png)

   >[!NOTE]
   >
   >Nel campo del collegamento sono supportati solo i tipi di campo stringa.

1. Fare clic su **Salva.**

   ![](assets/image2016-1-18-9-3a55-3a18.png)

1. Ripetete questa procedura per il secondo collegamento all&#39;oggetto personalizzato, in questo esempio, courseID. Il Nome oggetto collegamento sarà naturalmente e il Campo collegamento sarà courseID. Poiché avete già creato e approvato l’oggetto personalizzato del corso, queste selezioni sono disponibili nei menu a discesa.

   ![](assets/image2016-1-18-9-3a57-3a46.png)

1. Creare qualsiasi altro campo da utilizzare nell&#39;oggetto intermedio, ad esempio enrollmentID o grade.

## Uso di oggetti personalizzati {#using-custom-objects}

Il passo successivo consiste nell&#39;utilizzare questi oggetti personalizzati nei filtri nelle campagne smart. Con una relazione molti-a-molti, potete selezionare più persone/società e più oggetti personalizzati. Nell&#39;esempio seguente, verranno elencati tutti gli utenti presenti nel database che soddisfano tali criteri. Il campo del nome del corso deriva dall’oggetto personalizzato del corso e il livello di iscrizione deriva dall’oggetto intermedio.

![](assets/image2016-1-14-15-3a57-3a59.png)

>[!MORELIKETHIS]
>
>* [Aggiungi campi oggetto personalizzati Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md)
>* [Modifica ed eliminazione di un oggetto personalizzato Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-a-marketo-custom-object.md)
>* [Informazioni sugli oggetti personalizzati Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
>* [Modifica ed eliminazione dei campi oggetto personalizzati Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-marketo-custom-object-fields.md)

