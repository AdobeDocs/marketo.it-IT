---
unique-page-id: 10093192
description: Creare oggetti personalizzati Marketo - Documentazione Marketo - Documentazione del prodotto
title: Creare oggetti personalizzati Marketo
exl-id: d68b41e1-a12b-436f-aad7-42c7264cd901
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 0%

---

# Creare oggetti personalizzati Marketo {#create-marketo-custom-objects}

Utilizza oggetti personalizzati in Marketo per tenere traccia delle metriche specifiche della tua azienda. Può trattarsi di qualsiasi cosa, dalle auto ai corsi, qualsiasi cosa desideri modellare in Marketo per eseguire le tue campagne.

>[!NOTE]
>
>È possibile impostare oggetti personalizzati che funzionino da uno a molti o da molti a molti. L’oggetto iniziale viene creato allo stesso modo, ma i passaggi variano quando si iniziano ad aggiungere campi all’oggetto. Vedi  [Informazioni sugli oggetti personalizzati Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md) per ulteriori informazioni.

>[!NOTE]
>
>Non è possibile creare, modificare o eliminare un collegamento o un campo di deduplicazione dopo l’approvazione dell’oggetto personalizzato.

## Creare un oggetto personalizzato per una struttura uno-a-molti {#create-a-custom-object-for-a-one-to-many-structure}

Questo esempio mostra un oggetto personalizzato Car da utilizzare in una struttura uno-a-molti. In seguito, creerai un oggetto personalizzato del corso e un oggetto intermediario da utilizzare in una struttura molti-a-molti.

1. Fai clic su **Amministratore** e in **Gestione database** select **Oggetti personalizzati Marketo**.

   ![](assets/image2016-1-18-13-3a12-3a19.png)

1. Fai clic su **Nuovo oggetto personalizzato**.

   ![](assets/image2016-5-18-16-3a28-3a4.png)

   >[!NOTE]
   >
   >Nella scheda Oggetti personalizzati di Marketo sono visualizzati tutti gli oggetti personalizzati sulla destra e i dettagli relativi a quelli approvati, compreso il numero di record e campi nell’aggiornamento più recente.

1. Immettere un nome visualizzato. Il nome API e il nome plurale vengono compilati automaticamente. Immetti una descrizione (facoltativa).

   ![](assets/image2015-9-15-16-3a29-3a17.png)

   >[!NOTE]
   >
   >È possibile modificare questi campi durante la creazione, ma dopo averli salvati, è possibile modificare solo il campo Nome plurale e il campo **Mostra in dettaglio lead** cursore.

1. Estrarre **Mostra in dettaglio lead** cursore sopra la visualizzazione **Mostra** se si desidera visualizzare i dati degli oggetti personalizzati nella pagina Database lead. Fai clic su **Salva**.

   ![](assets/image2015-9-15-16-3a32-3a2.png)

1. Le informazioni sull’oggetto personalizzato visualizzano il contenuto immesso. Notate che è in stato Bozza.

   ![](assets/image2015-9-15-16-3a38-3a22.png)

   Il passaggio successivo consiste nell’aggiungere campi a [creare l’oggetto personalizzato](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md).

   >[!NOTE]
   >
   >È possibile compilare solo oggetti personalizzati Marketo tramite un’importazione di elenchi oppure [API](https://developers.marketo.com/documentation/rest/).

## Creare un oggetto personalizzato per una struttura Many-to-Many {#create-a-custom-object-for-a-many-to-many-structure}

Questo esempio mostra un oggetto personalizzato del corso, che verrà utilizzato per creare una relazione molti-a-molti tra persone/aziende e corsi. Al termine, creerai un oggetto intermediario per collegarlo alle persone o alle aziende nel database.

>[!NOTE]
>
>Per una relazione molti-a-molti, non è necessario creare un collegamento nell’oggetto personalizzato. Al contrario, verranno aggiunti due collegamenti all’oggetto intermediario (vedi di seguito).

1. Fai clic su **Amministratore** e in **Gestione database** select **Oggetti personalizzati Marketo**.

   ![](assets/image2016-1-18-13-3a16-3a25.png)

1. Fai clic su **Nuovo oggetto personalizzato**.

   ![](assets/image2016-5-18-16-3a32-3a42.png)

1. Immettere un nome visualizzato. Il nome API e il nome plurale vengono compilati automaticamente. Immetti una descrizione (facoltativa).

   ![](assets/image2016-1-14-13-3a38-3a46.png)

   >[!NOTE]
   >
   >È possibile modificare questi campi durante la creazione, ma dopo averli salvati, è possibile modificare solo il campo Nome plurale e il campo **Mostra in dettaglio lead** cursore.

1. Estrarre **Mostra in dettaglio lead** cursore sopra la visualizzazione **Mostra** se si desidera visualizzare i dati degli oggetti personalizzati nella pagina Database lead. Fai clic su **Salva**.

   ![](assets/image2016-1-14-13-3a42-3a56.png)

1. Le informazioni sull’oggetto personalizzato visualizzano il contenuto immesso. Notate che è in stato Bozza.

   ![](assets/image2016-1-18-8-3a38-3a58.png)

   >[!NOTE]
   >
   >È possibile compilare solo oggetti personalizzati Marketo tramite un’importazione di elenchi oppure [API](https://developers.marketo.com/documentation/rest/).

Il passaggio successivo consiste nel creare l’oggetto intermedio (vedere di seguito). Ma prima di questo, devi creare un campo a cui collegarti.

## Creare un oggetto intermedio {#create-an-intermediary-object}

Utilizzare un oggetto intermedio per collegare un oggetto personalizzato a persone o aziende. In questo esempio, viene utilizzato per collegare i corsi nell&#39;oggetto personalizzato del corso a persone o aziende nel database.

>[!NOTE]
>
>Non è necessario creare un oggetto intermedio per una struttura di oggetti personalizzati uno-a-molti.

1. Fai clic su **Amministratore** e in **Gestione database**, seleziona **Oggetti personalizzati Marketo**.

   ![](assets/image2016-1-18-13-3a17-3a40.png)

1. Fai clic su **Nuovo oggetto personalizzato**.

   ![](assets/image2016-5-18-16-3a33-3a16.png)

1. Immettere un nome visualizzato. Il nome API e il nome plurale vengono compilati automaticamente. Immetti una descrizione (facoltativa).

   ![](assets/image2016-1-14-14-3a10-3a44.png)

   >[!NOTE]
   >
   >È possibile modificare questi campi durante la creazione, ma dopo averli salvati, è possibile modificare solo il campo Nome plurale e il cursore Mostra in dettaglio lead.

1. Estrarre **Mostra in dettaglio lead** cursore sopra la visualizzazione **Mostra** se si desidera visualizzare i dati degli oggetti personalizzati nella pagina Database lead. Fai clic su **Salva**.

   ![](assets/image2016-1-14-14-3a12-3a49.png)

1. Le informazioni sull’oggetto personalizzato visualizzano il contenuto immesso. Notate che è in stato Bozza.

   Il passo successivo è quello di [aggiungere campi di collegamento](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md) per collegare l’oggetto intermedio a una persona/società e a un oggetto personalizzato.

>[!MORELIKETHIS]
>
>* [Aggiungi campi oggetto personalizzati Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md)
>* [Aggiungi campi di collegamento a oggetti personalizzati Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-link-fields.md)
>* [Informazioni sugli oggetti personalizzati Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)

