---
unique-page-id: 4720232
description: Creare un nuovo elenco di account - Documentazione Marketo - Documentazione del prodotto
title: Creare un nuovo elenco account
exl-id: 644c5b3b-852a-4dd9-8e55-b434505504ea
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 0%

---

# Creare un nuovo elenco account {#create-a-new-account-list}

Crea e carica un elenco di nomi di organizzazione e dominio per eseguire il targeting di questi account chiave con campagne personalizzate.

>[!NOTE]
>
>Questo articolo applica solo i clienti web ABM legacy. Se hai acquisito Web ABM dopo settembre 2016, segui i passaggi descritti in [articolo](https://docs.marketo.com/display/DOCS/Account+Lists#AccountLists-CreateaNewAccountList) invece.

## Creare un nuovo elenco account {#create-a-new-account-list-1}

1. Vai a **Elenchi account**.

   ![](assets/dropdown-account-lists-hand.jpg)

1. Seleziona **Crea nuovo**.

   ![](assets/create-new-account-list-hand.jpg)

1. Seleziona **Sfoglia** e carica il file CSV (assicurati che il file csv soddisfi i criteri). Aggiungi un **Nome** e **Descrizione**. Fai clic su **Salva**.

   ![](assets/create-account-list-hands.jpg)

   >[!NOTE]
   >
   >**Qual è il formato per il file CSV?**
   >
   >Assicurati che il file CSV dell&#39;account denominato soddisfi i seguenti requisiti:
   >
   >* Salvato come formato CSV
   >* Non supera 10 MB
   >* Solo 4 colonne con intestazione Colonna A: Nome, colonna B: Dominio, colonna C: Paese, colonna D: Stato americano.
   >* Il file caricato può richiedere fino a 2 giorni lavorativi prima dell’approvazione.
   >* Riceverai una notifica e-mail di approvazione o controllerai lo stato del file nella pagina Account denominati .
   >* Il numero totale di record/righe accumulati per tutti i tuoi elenchi caricati inizia a 10K, con il pacchetto più grande per un totale di 100K.


   >[!NOTE]
   >
   >**Esempio di file CSV**
   >
   >* Riga 1 Colonna A valore = Organizzazione
   >* Valore della colonna B riga 1 = dominio
   >* Riga 1 Colonna C valore = Paese
   >* Riga 1 Valore della colonna D = Stato USA
   >* Uno dei valori della colonna è obbligatorio. Tuttavia, fornendo sia i nomi dell’organizzazione che quelli del dominio si migliorano le percentuali di corrispondenza dell’elenco account.
   >* Paese e stato sono valori facoltativi.
      >
      >   * Per il nome del paese, utilizzare il nome del paese completo o il codice abbreviato. Esempio Stati Uniti o Stati Uniti.
      >   * Per uno Stato degli Stati Uniti, utilizzare il codice abbreviato di 2 lettere, ad esempio CA. Solo gli Stati Uniti sono riconosciuti.

   >
   >![](assets/image2015-2-25-12-3a19-3a10.png)

## Modificare un elenco account {#edit-an-account-list}

Sulla **Elenchi account** fai clic su **Modifica** nell&#39;elenco.

![](assets/create-new-account-list-edit.jpg)

Seleziona **Sfoglia** e carica il nuovo file CSV. Questo file sostituirà il file originale. Fai clic su **Salva**. Il nuovo file caricato sarà in sospeso fino all’approvazione da parte del supporto Marketo, quando in uno stato in sospeso il file originale rimarrà attivo.

![](assets/set-account-list-edit-hands.jpg)

Il file CSV sostituirà il file esistente. L’elenco esistente rimarrà attivo fino al completamento dell’elaborazione del nuovo file.

## Eliminare un elenco account denominato {#delete-a-named-account-list}

1. Sulla **Elenchi account** fare clic sull’icona Elimina dell’elenco da eliminare.

   ![](assets/create-new-account-list-delete.jpg)

1. Viene visualizzato un messaggio per confermare l’eliminazione dell’elenco. Fai clic su **OK**.

   ![](assets/delete-notification-hand.jpg)

>[!MORELIKETHIS]
>
>[Creare un segmento utilizzando un elenco account](/help/marketo/product-docs/web-personalization/account-based-web-marketing/create-a-segment-using-an-account-list.md)
