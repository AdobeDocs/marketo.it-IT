---
unique-page-id: 10093188
description: Informazioni sugli oggetti personalizzati di Marketo - Documentazione di Marketo - Documentazione del prodotto
title: Informazioni sugli oggetti personalizzati di Marketo
exl-id: f18b1689-c7bc-4da0-8326-7b29733d527d
feature: Custom Objects
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '689'
ht-degree: 2%

---

# Informazioni sugli oggetti personalizzati di Marketo {#understanding-marketo-custom-objects}

Utilizza oggetti personalizzati per tenere traccia delle metriche specifiche della tua azienda.

>[!AVAILABILITY]
>
>Non tutti gli utenti di Marketo Engage hanno acquistato questa funzionalità. Per informazioni, contatta il team dell’account di Adobe (il tuo Account Manager).

Utilizza oggetti personalizzati come filtri e attivatori nelle campagne intelligenti. Ad esempio:

* **Filtro**: invia e-mail solo ai proprietari di una marca di veicolo specifica
* **Trigger**: invia un&#39;e-mail quando un oggetto personalizzato viene aggiunto a una persona o a un&#39;azienda.

È possibile impostare oggetti personalizzati in una relazione uno-a-molti o molti-a-molti. Ad esempio:

* **Uno-a-molti**: una persona possiede più auto
* **Molti-a-molti**: più studenti sono iscritti a più corsi da un catalogo corsi

Una struttura uno-a-molti utilizza un singolo campo di collegamento per collegare l’oggetto personalizzato a una persona o a un’azienda.

Gli oggetti personalizzati &quot;da molti a molti&quot; utilizzano due campi di collegamento, parte di un oggetto intermedio. Un campo Collegamento è connesso alla persona o all’azienda, mentre un altro campo è connesso all’oggetto personalizzato, ad esempio il catalogo dei corsi. Questo oggetto intermedio può contenere campi personalizzati aggiuntivi, ad esempio un livello di corso o una data di partecipazione, che definiscono ulteriormente la natura della connessione.

>[!TIP]
>
>Importa oggetti personalizzati utilizzando valori delimitati da virgole (CSV) all’interno dell’interfaccia utente per testare e convalidare un esempio di dati. Quindi, carica tutti i file con un’API.

>[!CAUTION]
>
>Non è possibile ripristinare oggetti personalizzati, quindi assicurati di non averne più bisogno prima di eliminarli.

## Accesso agli oggetti personalizzati di Marketo {#accessing-marketo-custom-objects}

1. Passa alla schermata **[!UICONTROL Admin]**.

   ![](assets/understanding-marketo-custom-objects-1.png)

1. Fai clic su **[!UICONTROL Marketo Custom Objects]**.

   ![](assets/understanding-marketo-custom-objects-2.png)

1. Nella visualizzazione Oggetti personalizzati di Marketo sono elencati a destra tutti gli oggetti personalizzati, ma solo quelli approvati nella griglia principale.

   ![](assets/understanding-marketo-custom-objects-3.png)

   >[!NOTE]
   >
   >Nella griglia vengono visualizzati il nome dell&#39;oggetto, il numero di record, il numero di campi e la data dell&#39;aggiornamento più recente.

   >[!TIP]
   >
   >Marketo aggiorna questi campi automaticamente, ma puoi aggiornare la visualizzazione facendo clic sull’icona nella colonna Record.

1. Fare clic sul nome dell&#39;oggetto a destra per aprire la pagina dei dettagli.

   ![](assets/understanding-marketo-custom-objects-4.png)

## Visualizzare oggetti personalizzati associati a una persona {#view-custom-objects-associated-to-a-person}

Dopo aver creato la struttura oggetto personalizzata, quando si caricano dati oggetto personalizzati specifici, gli oggetti personalizzati vengono automaticamente associati agli utenti del database utilizzando il campo di collegamento nell&#39;oggetto personalizzato. È possibile visualizzare le informazioni dalla scheda [!UICONTROL Custom Objects] nella pagina dei dettagli della persona.

1. Vai a **[!UICONTROL Database]**.

   ![](assets/understanding-marketo-custom-objects-5.png)

1. Aprire il database e fare clic sulla scheda **[!UICONTROL People]**. Fare doppio clic sul record di una persona associata a un oggetto personalizzato.

   ![](assets/understanding-marketo-custom-objects-6.png)

1. Nella pagina dei dettagli della persona fare clic sulla scheda **[!UICONTROL Custom Objects]**. Seleziona l’oggetto dal menu a discesa.

   ![](assets/understanding-marketo-custom-objects-7.png)

1. Ora puoi visualizzare un elenco di tutti gli oggetti personalizzati di quel tipo associati a quella persona.

   ![](assets/understanding-marketo-custom-objects-8.png)

   >[!NOTE]
   >
   >In un record persona, nella scheda Oggetto personalizzato è possibile visualizzare un massimo di 100 record, ordinati in base all&#39;ID in ordine decrescente.

## Utilizzo di oggetti personalizzati con le aziende {#using-custom-objects-with-companies}

Un oggetto personalizzato collegato all’azienda funziona meglio se sincronizzi le aziende dal sistema di gestione delle relazioni con i clienti o se crei esplicitamente aziende utilizzando l’API. È inoltre consigliabile utilizzare l’ID azienda come campo di collegamento.

Se in Marketo sono presenti più persone che sono record nei record CRM o solo Marketo, un oggetto personalizzato collegato a un&#39;azienda non verrà associato a più di un singolo record. Questo perché una società con più persone al di sotto di essa è supportata solo quando le società vengono sincronizzate dal sistema di gestione delle relazioni con i clienti o se utilizzi un’API per creare esplicitamente le società.

Gli oggetti personalizzati possono essere collegati direttamente solo a un singolo record. Ciò significa che quando il tipo di oggetto personalizzato è collegato dal campo aziendale, devi assicurarti che i record delle persone siano associati a una società utilizzando la conversione dei contatti nel CRM oppure utilizzando il campo externalCompanyId, se gestisci aziende utilizzando le API REST di Marketo. Per i record persona che non sono collegati in modo esplicito ai record società, gli oggetti personalizzati collegati tramite azienda verranno collegati in modo casuale a un singolo record, anche se il valore del campo società è condiviso tra più persone.

Per ulteriori informazioni, vedere [Importa dati oggetto personalizzati](/help/marketo/product-docs/administration/marketo-custom-objects/import-custom-object-data.md).

>[!MORELIKETHIS]
>
>* [Crea oggetti personalizzati Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/create-marketo-custom-objects.md)
>* [Approva un oggetto personalizzato](/help/marketo/product-docs/administration/marketo-custom-objects/approve-a-custom-object.md)
>* [Modifica ed elimina un oggetto personalizzato di Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-a-marketo-custom-object.md)
>* [Aggiungi campi oggetto personalizzati Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/add-marketo-custom-object-fields.md)
>* [Modifica ed elimina campi oggetto personalizzati di Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/edit-and-delete-marketo-custom-object-fields.md)
>* [Importa dati oggetto personalizzati](/help/marketo/product-docs/administration/marketo-custom-objects/import-custom-object-data.md)
