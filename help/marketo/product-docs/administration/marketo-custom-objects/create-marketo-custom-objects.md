---
unique-page-id: 10093192
description: Creare oggetti personalizzati Marketo - Documenti Marketo - Documentazione del prodotto
title: Creare oggetti personalizzati Marketo
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 0%

---


# Creare oggetti personalizzati Marketo {#create-marketo-custom-objects}

Utilizzare oggetti personalizzati in Marketo per tenere traccia delle metriche specifiche della tua attività. Potrebbe trattarsi di qualsiasi cosa, dalle auto ai corsi, qualunque cosa desideri fare per modellare a Marketo per eseguire le tue campagne.

>[!NOTE]
>
>È possibile impostare oggetti personalizzati per l&#39;utilizzo su base uno-a-molti o molti-a-molti. L&#39;oggetto iniziale viene creato allo stesso modo, ma i passaggi variano quando si iniziano ad aggiungere campi all&#39;oggetto. Per ulteriori informazioni, vedere [Informazioni sugli oggetti](understanding-marketo-custom-objects.md) personalizzati Marketo.

>[!NOTE]
>
>Non è possibile creare, modificare o eliminare un collegamento o un campo dedicato dopo l&#39;approvazione dell&#39;oggetto personalizzato.

## Creare un oggetto personalizzato per una struttura uno-a-molti {#create-a-custom-object-for-a-one-to-many-structure}

Questo esempio mostra un oggetto personalizzato Auto da utilizzare in una struttura uno-molti. Successivamente, creerete un oggetto personalizzato per il corso e un oggetto intermediario da utilizzare in una struttura multi-a-molti.

1. Fare clic su **Admin**, quindi in Gestione **** database selezionare **Marketo oggetti** personalizzati.

   ** ![](assets/image2016-1-18-13-3a12-3a19.png)

   **

1. Fare clic su **Nuovo oggetto** personalizzato.

   ![](assets/image2016-5-18-16-3a28-3a4.png)

   >[!NOTE]
   >
   >La scheda Oggetti personalizzati Marketo visualizza tutti gli oggetti personalizzati sulla destra e i dettagli per quelli approvati, incluso il numero di record e campi nell&#39;aggiornamento più recente.

1. Immettete un nome da visualizzare. Il nome API e il nome plurale vengono inseriti automaticamente. Inserite una descrizione (facoltativo).

   ![](assets/image2015-9-15-16-3a29-3a17.png)

   >[!NOTE]
   >
   >Potete modificare questi campi quando li create, ma dopo averli salvati, potete modificare solo il campo Nome plurale e il cursore **Mostra in dettaglio** lead.

1. Trascinare il cursore **Show in Lead Detail **per visualizzare **Show** se si desidera visualizzare i dati dell&#39;oggetto personalizzato nella pagina Lead Database. Fate clic su **Salva**.

   ![](assets/image2015-9-15-16-3a32-3a2.png)

1. Le informazioni sull&#39;oggetto personalizzato mostrano il contenuto immesso. Notate che si trova in stato Bozza.

   ![](assets/image2015-9-15-16-3a38-3a22.png)

   Il passaggio successivo consiste nell&#39;aggiungere campi per [creare l&#39;oggetto](add-marketo-custom-object-fields.md)personalizzato.

   >[!NOTE]
   >
   >È possibile compilare solo oggetti personalizzati Marketo tramite un&#39;importazione di elenco o l&#39; [API](http://developers.marketo.com/documentation/rest/).

## Creare un oggetto personalizzato per una struttura molti-molti {#create-a-custom-object-for-a-many-to-many-structure}

Questo esempio mostra un oggetto personalizzato del corso, che verrà utilizzato per creare una relazione molti-a-molti tra persone/società e corsi. Al termine, verrà creato un oggetto intermediario per collegarlo alle persone o alle società presenti nel database.

>[!NOTE]
>
>Per una relazione molti-a-molti, non è necessario creare un collegamento nell&#39;oggetto personalizzato. Verranno invece aggiunti due collegamenti all&#39;oggetto intermediario (vedere di seguito).

1. Fare clic su **Admin**, quindi in Gestione **** database selezionare **Marketo oggetti** personalizzati.

   ![](assets/image2016-1-18-13-3a16-3a25.png)

1. Fare clic su **Nuovo oggetto** personalizzato.

   ![](assets/image2016-5-18-16-3a32-3a42.png)

1. Immettete un nome da visualizzare. Il nome API e il nome plurale vengono inseriti automaticamente. Inserite una descrizione (facoltativo).

   ![](assets/image2016-1-14-13-3a38-3a46.png)

   >[!NOTE]
   >
   >Potete modificare questi campi quando li create, ma dopo averli salvati, potete modificare solo il campo Nome plurale e il cursore **Mostra in dettaglio** lead.

1. Trascinare il cursore **Show in Lead Detail **per visualizzare Show (Mostra) se si desidera visualizzare i dati dell&#39;oggetto personalizzato nella pagina Lead Database. Fate clic su **Salva**.

   ![](assets/image2016-1-14-13-3a42-3a56.png)

1. Le informazioni sull&#39;oggetto personalizzato mostrano il contenuto immesso. Notate che si trova in stato Bozza.

   ![](assets/image2016-1-18-8-3a38-3a58.png)

   >[!NOTE]
   >
   >È possibile compilare solo oggetti personalizzati Marketo tramite un&#39;importazione di elenco o l&#39; [API](http://developers.marketo.com/documentation/rest/).

Il passaggio successivo prevede la creazione dell&#39;oggetto intermediario (vedere di seguito). Ma prima di questo, è necessario creare un campo a cui collegarsi.

## Creare un oggetto intermedio {#create-an-intermediary-object}

Utilizzare un oggetto intermediario per collegare un oggetto personalizzato a persone o società. In questo esempio, viene utilizzato per collegare i corsi nell&#39;oggetto personalizzato del corso alle persone o alle società presenti nel database.

>[!NOTE]
>
>Non è necessario creare un oggetto intermediario per una struttura di oggetti personalizzata uno-molti.

1. Fare clic su **Admin** e, in Gestione **** database, selezionare **Marketo oggetti** personalizzati.

   ![](assets/image2016-1-18-13-3a17-3a40.png)

1. Fare clic su **Nuovo oggetto** personalizzato.

   ![](assets/image2016-5-18-16-3a33-3a16.png)

1. Immettete un nome da visualizzare. Il nome API e il nome plurale vengono inseriti automaticamente. Inserite una descrizione (facoltativo).

   ![](assets/image2016-1-14-14-3a10-3a44.png)

   >[!NOTE]
   >
   >Potete modificare questi campi quando li create, ma dopo averli salvati, potete modificare solo il campo Nome plurale e il cursore Mostra in dettaglio lead.

1. Spostate il cursore **Mostra in Dettagli** lead per visualizzare Mostra per visualizzare i dati oggetto personalizzati nella pagina Database lead. Fate clic su **Salva**.

   ![](assets/image2016-1-14-14-3a12-3a49.png)

1. Le informazioni sull&#39;oggetto personalizzato mostrano il contenuto immesso. Notate che si trova in stato Bozza.

   Il passaggio successivo prevede l&#39; [aggiunta di campi](add-marketo-custom-object-link-fields.md) di collegamento per collegare l&#39;oggetto intermediario a una persona/società e a un oggetto personalizzato.

>[!MORELIKETHIS]
>
>* [Aggiungi campi oggetto personalizzati Marketo](add-marketo-custom-object-fields.md)
>* [Aggiungi campi collegamento oggetto personalizzato marketing](add-marketo-custom-object-link-fields.md)
>* [Informazioni sugli oggetti personalizzati Marketo](understanding-marketo-custom-objects.md)

>



