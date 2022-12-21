---
unique-page-id: 11378814
description: Elenchi account - Documenti Marketo - Documentazione del prodotto
title: Elenchi account
exl-id: 31bb4341-d012-4239-8f40-10a07cd4c51c
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---

# Elenchi account {#account-lists}

Un elenco di account è una raccolta di account denominati che possono essere targetizzati insieme. Gli elenchi di account ti consentono di eseguire il targeting degli account denominati in base al settore, alla posizione o alle dimensioni dell’azienda.

Oltre agli elenchi di account, puoi anche creare elenchi di account dinamici generati da visualizzazioni account CRM pubbliche. Una visualizzazione account CRM è un insieme di regole che funge da filtro durante la visualizzazione degli account. Ad esempio, puoi usarlo per trovare account in cui l&#39;Industria è Medicale *e* Le entrate superano i 100 milioni di dollari.

![](assets/one.png)

>[!NOTE]
>
>Gli elenchi di account creati in Gestione account di Marketo Target sono automaticamente disponibili quando si creano elenchi smart e campagne web in [Personalizzazione web](/help/marketo/product-docs/web-personalization/using-web-segments/web-segments.md).

## Creare un nuovo elenco account {#create-a-new-account-list}

1. Fai clic sul pulsante **Nuovo** a discesa e seleziona **Crea nuovo elenco account**.

   ![](assets/1a.png)

1. Assegna un nome all&#39;elenco e fai clic su **Crea**.

   ![](assets/three-0.png)

1. Dopo aver creato l&#39;elenco degli account, inizia a [aggiunta di account denominati](/help/marketo/product-docs/target-account-management/target/named-accounts/add-an-existing-named-account-to-an-account-list.md)!

   >[!NOTE]
   >
   >Marketo mostrerà solo informazioni per gli elenchi di account con un massimo di 2.000 account denominati.

## Creare un nuovo elenco account dinamico {#create-a-new-dynamic-account-list}

1. Fai clic sul pulsante **Nuovo** a discesa e seleziona **Crea nuovo elenco dinamico**.

   ![](assets/1.png)

1. Nella finestra di dialogo, seleziona un **Visualizzazione account CRM** dall’elenco a discesa, oppure digita il nome per cercarlo.

   ![](assets/image2017-7-18-9-48-23.png)

1. Fai clic su **Crea**.

   ![](assets/step4.jpg)

   >[!NOTE]
   >
   >In Salesforce, assicurati di fornire le autorizzazioni Oggetto vista elenco all’utente di sincronizzazione.

## Rinominare un elenco account {#rename-an-account-list}

>[!NOTE]
>
>Questi passaggi si applicano solo agli elenchi di account. _Dinamico_ Gli elenchi di account utilizzano il nome delle relative visualizzazioni account CRM associate.

1. Seleziona l’account da rinominare, fai clic sul pulsante **Azioni elenco account** a discesa e seleziona **Rinomina elenco account**.

   ![](assets/three.png)

1. Inserisci il nuovo nome e fai clic su **Rinomina**.

   ![](assets/four.png)

   >[!NOTE]
   >
   >La visualizzazione account CRM si sincronizza con l&#39;elenco degli account dinamici ogni 8 ore. Se non sono ancora sincronizzati, Marketo li sincronizzerà durante il ciclo successivo.

## Eliminare un elenco account {#delete-an-account-list}

>[!NOTE]
>
>Questi passaggi sono gli stessi sia per gli elenchi di account che per gli elenchi di account dinamici.

1. Seleziona l’account da eliminare, fai clic sul pulsante **Azioni elenco account** a discesa e seleziona **Elimina elenco account**.

   ![](assets/five.png)

1. Fai clic su **Elimina**.

   ![](assets/six.png)

>[!MORELIKETHIS]
>
>* [Aggiungi un account con nome esistente a un elenco account](/help/marketo/product-docs/target-account-management/target/named-accounts/add-an-existing-named-account-to-an-account-list.md)
>* [Approfondimenti elenco account](/help/marketo/product-docs/target-account-management/measure/account-list-insights.md)

