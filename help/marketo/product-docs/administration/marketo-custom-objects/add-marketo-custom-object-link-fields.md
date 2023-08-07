---
unique-page-id: 10097613
description: Aggiungere campi di collegamento oggetti personalizzati di Marketo - Documentazione di Marketo - Documentazione del prodotto
title: Aggiungi campi collegamento oggetto personalizzato Marketo
exl-id: e7537d79-9fca-4966-881a-9d7d312008e2
feature: Custom Objects
source-git-commit: 1dbe820e126f92ce5820e38414925605372a4b09
workflow-type: tm+mt
source-wordcount: '702'
ht-degree: 0%

---

# Aggiungi campi collegamento oggetto personalizzato Marketo {#add-marketo-custom-object-link-fields}

Quando si creano oggetti personalizzati, è necessario fornire campi di collegamento per collegare il record oggetto personalizzato al record padre corretto.

* Per una struttura personalizzata uno-a-molti, utilizza il campo collegamento nell’oggetto personalizzato per connetterlo a una persona o a un’azienda.
* Per una struttura molti-a-molti, si utilizzano due campi di collegamento, connessi da un oggetto intermedio creato separatamente (che è anche un tipo di oggetto personalizzato). Un collegamento si connette a persone o società nel database e l&#39;altro all&#39;oggetto personalizzato. In questo caso, il campo del collegamento non si trova nell’oggetto personalizzato stesso.

>[!IMPORTANT]
>
>Il Marketo Engage supporta un solo oggetto edge per ogni oggetto bridge nella relazione Many to Many (Da molti a molti). Nell’esempio fornito di seguito, ogni iscrizione può essere collegata solo a un singolo corso. Tuttavia, possono esserci molti oggetti ponte per ogni oggetto perimetrale, così come ci sono molte iscrizioni degli studenti a ogni corso (relazione molti-a-uno). Se i dati oggetto personalizzati sono strutturati in modo che esistano più record oggetto Edge per ogni record oggetto Bridge (uno-a-molti o molti-a-molti), è possibile creare più record oggetto Bridge che fanno riferimento a ogni singolo record oggetto Edge per rappresentare tali dati in Marketo.

## Creare un campo collegamento per una struttura uno-a-molti {#create-a-link-field-for-a-one-to-many-structure}

Di seguito viene illustrato come creare un campo collegamento in un oggetto personalizzato per una struttura uno-a-molti.

1. Vai a **[!UICONTROL Amministratore]** area.

   ![](assets/add-marketo-custom-object-link-fields-1.png)

1. Clic **[!UICONTROL Oggetti personalizzati Marketo]**.

   ![](assets/add-marketo-custom-object-link-fields-2.png)

1. Selezionare l&#39;oggetto personalizzato nell&#39;elenco.

   ![](assets/add-marketo-custom-object-link-fields-3.png)

1. In **[!UICONTROL Campi]** , fare clic su **[!UICONTROL Nuovo campo]**.

   ![](assets/add-marketo-custom-object-link-fields-4.png)

1. Denomina il campo del collegamento e aggiungi un elemento facoltativo [!UICONTROL Descrizione]. Accertati di selezionare [!UICONTROL Collegamento] tipo di dati.

   ![](assets/add-marketo-custom-object-link-fields-5.png)

   >[!CAUTION]
   >
   >Non potrai tornare indietro e creare, modificare o eliminare una [!UICONTROL Collegamento] o [!UICONTROL Deduplica campo] dopo l&#39;approvazione dell&#39;oggetto personalizzato.

1. Seleziona se [!UICONTROL Collega oggetto] è per un [!UICONTROL lead] (persona) o un [!UICONTROL azienda].

   ![](assets/add-marketo-custom-object-link-fields-6.png)

   >[!NOTE]
   >
   >Se si sceglie [!UICONTROL lead], nell&#39;elenco sono visualizzati ID, indirizzo e-mail ed eventuali campi personalizzati.
   >
   >Se si sceglie [!UICONTROL azienda], nell&#39;elenco sono visualizzati l&#39;ID ed eventuali campi personalizzati.

1. Seleziona la [!UICONTROL Campo collegamento] desideri connetterti a come elemento principale del nuovo campo.

   ![](assets/add-marketo-custom-object-link-fields-7.png)

   >[!NOTE]
   >
   >Nel campo collegamento sono supportati solo i tipi di campo stringa.

1. Clic **[!UICONTROL Salva]**.

   ![](assets/add-marketo-custom-object-link-fields-8.png)

## Creare un campo di collegamento per una struttura Many-to-Many (Da molti-a-molti) {#create-a-link-field-for-a-many-to-many-structure}

Di seguito viene illustrato come creare un campo di collegamento in un oggetto intermedio da utilizzare in una struttura molti-a-molti.

>[!PREREQUISITES]
>
>È necessario avere già creato l&#39;oggetto intermedio e tutti gli oggetti personalizzati a cui si desidera collegarlo.

1. Vai a **[!UICONTROL Amministratore]** area.

   ![](assets/add-marketo-custom-object-link-fields-9.png)

1. Clic **[!UICONTROL Oggetti personalizzati Marketo]**.

   ![](assets/add-marketo-custom-object-link-fields-10.png)

1. Seleziona l’oggetto intermedio a cui aggiungere il campo.

   ![](assets/add-marketo-custom-object-link-fields-11.png)

1. In **[!UICONTROL Campi]** , fare clic su **[!UICONTROL Nuovo campo]**.

   ![](assets/add-marketo-custom-object-link-fields-12.png)

1. Devi creare due campi di collegamento. Creale una alla volta. Innanzitutto, assegna un nome al campo per i membri dell’elenco del database (ad esempio, leadID). Aggiungi un elemento [!UICONTROL Descrizione]. Accertati di selezionare [!UICONTROL link] [!UICONTROL Tipo di dati].

   ![](assets/add-marketo-custom-object-link-fields-13.png)

   >[!CAUTION]
   >
   >Non potrai tornare indietro e creare, modificare o eliminare una [!UICONTROL Collegamento] o [!UICONTROL Deduplica campo] dopo l&#39;approvazione dell&#39;oggetto personalizzato.

1. Seleziona la [!UICONTROL Collega oggetto] dal database; in questo caso, [!UICONTROL Lead].

   ![](assets/add-marketo-custom-object-link-fields-14.png)

1. Seleziona la [!UICONTROL Campo collegamento] a cui desideri connetterti, in questo caso, [!UICONTROL ID].

   ![](assets/add-marketo-custom-object-link-fields-15.png)

   >[!NOTE]
   >
   >Solo i tipi di campo stringa sono supportati nel [!UICONTROL Campo collegamento].

1. Clic **[!UICONTROL Salva]**.

   ![](assets/add-marketo-custom-object-link-fields-16.png)

1. Ripeti questa procedura per il secondo collegamento all’oggetto personalizzato, in questo esempio, courseID. Il [!UICONTROL Collega oggetto] il nome sarà corso e il [!UICONTROL Campo collegamento] sarà courseID. Poiché hai già creato e approvato l’oggetto personalizzato del corso, queste selezioni sono disponibili nei menu a discesa.

   ![](assets/add-marketo-custom-object-link-fields-17.png)

1. Creare qualsiasi altro campo che si desidera utilizzare nell&#39;oggetto intermedio, ad esempio enrollmentID o livello.

## Utilizzo di oggetti personalizzati {#using-custom-objects}

Il passaggio successivo consiste nell’utilizzare questi oggetti personalizzati nei filtri delle campagne intelligenti. Con una relazione molti-a-molti, puoi selezionare più persone/aziende e più oggetti personalizzati. Nell’esempio seguente, verranno elencati tutti gli utenti del database che soddisfano questi criteri. Il campo Nome corso proviene dall&#39;oggetto personalizzato del corso e il livello di iscrizione proviene dall&#39;oggetto intermedio.

![](assets/add-marketo-custom-object-link-fields-18.png)

>[!MORELIKETHIS]
>
>* [Aggiungi campi oggetto personalizzati Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md)
>* [Modificare ed eliminare un oggetto personalizzato di Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-a-marketo-custom-object.md)
>* [Informazioni sugli oggetti personalizzati di Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
>* [Modificare ed eliminare i campi oggetto personalizzati di Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-marketo-custom-object-fields.md)
