---
unique-page-id: 10097613
description: Aggiungere campi di collegamento oggetto personalizzato Marketo - Documenti Marketo - Documentazione del prodotto
title: Aggiungi campi di collegamento a oggetti personalizzati Marketo
exl-id: e7537d79-9fca-4966-881a-9d7d312008e2
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '601'
ht-degree: 0%

---

# Aggiungi campi di collegamento a oggetti personalizzati Marketo {#add-marketo-custom-object-link-fields}

Quando si creano oggetti personalizzati, è necessario fornire campi di collegamento per collegare il record di oggetti personalizzati al record padre corretto.

* Per una struttura personalizzata uno-a-molti, utilizzare il campo di collegamento nell’oggetto personalizzato per collegarlo a una persona o a una società.
* Per una struttura molti-a-molti, è possibile utilizzare due campi di collegamento, collegati da un oggetto intermedio creato separatamente (che è anche un tipo di oggetto personalizzato). Un collegamento si connette alle persone o alle aziende nel database e l’altro all’oggetto personalizzato. In questo caso, il campo di collegamento non si trova nell’oggetto personalizzato stesso.

## Creare un campo di collegamento per una struttura uno-a-molti {#create-a-link-field-for-a-one-to-many-structure}

Ecco come creare un campo di collegamento in un oggetto personalizzato per una struttura uno-a-molti.

1. Fai clic su **Amministratore** e in **Gestione database**, seleziona **Oggetti personalizzati Marketo**.

   ![](assets/image2016-1-18-13-3a25-3a11.png)

1. Selezionare l’oggetto personalizzato nell’elenco.

   ![](assets/image2016-1-14-15-3a6-3a2.png)

1. In **Campi** scheda , fai clic su **Nuovo campo**.

   ![](assets/image2015-9-17-14-3a9-3a19.png)

1. Denomina il campo del collegamento e aggiungi una descrizione facoltativa. Assicurati di selezionare il tipo di dati Collegamento .

   ![](assets/image2015-10-5-13-3a24-3a57.png)

   >[!CAUTION]
   >
   >Non potrai tornare indietro e creare, modificare o eliminare un collegamento o un campo di deduplicazione dopo l’approvazione dell’oggetto personalizzato.

1. Seleziona se l’oggetto collegamento è per un lead (persona) o per un’azienda.

   ![](assets/image2015-10-5-13-3a28-3a1.png)

   >[!NOTE]
   >
   >Se scegli il lead, vedrai ID, indirizzo e-mail e tutti i campi personalizzati nell’elenco.
   >
   >Se scegli l’azienda, vedrai l’ID e tutti i campi personalizzati nell’elenco.

1. Selezionare il campo di collegamento a cui si desidera connettersi come elemento padre del nuovo campo.

   ![](assets/image2015-10-5-13-3a30-3a6.png)

   >[!NOTE]
   >
   >Nel campo di collegamento sono supportati solo i tipi di campo stringa.

1. Fai clic su **Salva.**

   ![](assets/image2015-10-5-13-3a34-3a0.png)

## Creare un campo di collegamento per una struttura Molti-a-Molti {#create-a-link-field-for-a-many-to-many-structure}

Ecco come creare un campo di collegamento in un oggetto intermedio da utilizzare in una struttura molti-a-molti.

>[!PREREQUISITES]
>
>È necessario aver già creato l’oggetto intermedio ed eventuali oggetti personalizzati a cui si desidera collegarlo.

1. Fai clic su **Amministratore** e in **Gestione database**, seleziona **Oggetti personalizzati Marketo**.

   ![](assets/image2016-1-18-9-3a8-3a14.png)

1. Selezionare l’oggetto intermedio a cui si desidera aggiungere il campo.

   ![](assets/image2016-1-18-9-3a10-3a29.png)

1. In **Campi** scheda , fai clic su **Nuovo campo**.

   ![](assets/image2016-1-18-9-3a31-3a43.png)

1. È necessario creare due campi di collegamento. Crea uno alla volta. Innanzitutto, denominare il campo relativo ai membri dell’elenco di database (ad esempio, leadID). Aggiungi una descrizione facoltativa. Assicurati di selezionare il tipo di dati del collegamento.

   ![](assets/image2016-1-18-9-3a38-3a59.png)

   >[!CAUTION]
   >
   >Non potrai tornare indietro e creare, modificare o eliminare un collegamento o un campo di deduplicazione dopo l’approvazione dell’oggetto personalizzato.

1. Selezionare l&#39;oggetto collegamento dal database, in questo caso Lead.

   ![](assets/image2016-1-18-9-3a50-3a48.png)

1. Seleziona il campo di collegamento a cui desideri connetterti, in questo caso, ID.

   ![](assets/image2016-1-18-9-3a53-3a54.png)

   >[!NOTE]
   >
   >Nel campo di collegamento sono supportati solo i tipi di campo stringa.

1. Fai clic su **Salva.**

   ![](assets/image2016-1-18-9-3a55-3a18.png)

1. Ripeti questo processo per il secondo collegamento all’oggetto personalizzato, in questo esempio, courseID. Il campo Nome oggetto collegamento sarà naturalmente e il campo collegamento sarà naturalmente ID. Poiché hai già creato e approvato l’oggetto personalizzato del corso, queste selezioni sono disponibili nei menu a discesa.

   ![](assets/image2016-1-18-9-3a57-3a46.png)

1. Creare tutti gli altri campi che si desidera utilizzare nell&#39;oggetto intermedio, ad esempio enRegistrationID o grade.

## Utilizzo di oggetti personalizzati {#using-custom-objects}

Il passaggio successivo consiste nell’utilizzare questi oggetti personalizzati nei filtri nelle campagne avanzate. Con una relazione molti-a-molti, è possibile selezionare più persone/aziende e più oggetti personalizzati. Nell’esempio seguente, verranno elencati tutti gli utenti del database che soddisfano questi criteri. Il campo del nome del corso viene dall&#39;oggetto personalizzato del corso e il livello di iscrizione viene dall&#39;oggetto intermedio.

![](assets/image2016-1-14-15-3a57-3a59.png)

>[!MORELIKETHIS]
>
>* [Aggiungi campi oggetto personalizzati Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md)
>* [Modificare ed eliminare un oggetto personalizzato Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-a-marketo-custom-object.md)
>* [Informazioni sugli oggetti personalizzati Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
>* [Modificare ed eliminare i campi oggetto personalizzati Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-marketo-custom-object-fields.md)

