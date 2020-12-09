---
unique-page-id: 10099680
description: Importa dati oggetto personalizzati - Documenti Marketo - Documentazione prodotto
title: Importa dati oggetto personalizzati
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---


# Importa dati oggetto personalizzati {#import-custom-object-data}

È facile importare dati oggetto personalizzati nel database. Se si utilizzano oggetti personalizzati con le società, per ulteriori informazioni vedere [Uso di oggetti personalizzati con le società](http://docs.marketo.com/display/DOCS/Understanding+Marketo+Custom+Objects#UnderstandingMarketoCustomObjects-customcompanyUsingCustomObjectswithCompanies) .

1. In My Marketo, andate a **Database**.

   ![](assets/db-1.png)

1. Fare clic su **Nuovo** e selezionare **Importa dati** oggetto personalizzati.

   ![](assets/image2016-4-7-10-6-54.png)

1. Fare clic su **Sfoglia** per individuare il file di dati. Selezionare il formato del file (in questo esempio, Valori separati da virgole).

   ![](assets/image2016-4-13-14-3a21-3a53.png)

1. Selezionare l&#39;oggetto personalizzato.

   ![](assets/image2016-4-13-14-3a24-3a54.png)

1. Selezionate la modalità Deduplica dal menu a discesa. Fate clic su **Avanti**.

   ![](assets/image2016-4-13-14-3a28-3a7.png)

   >[!NOTE]
   >
   >Utilizzare i campi dedicati come identificatori univoci quando si creano o aggiornano record di oggetti personalizzati. In questo esempio viene utilizzato il campo Dedupe dell&#39;oggetto personalizzato **car** - vin (numero ID veicolo). Se si aggiornano solo i record di oggetti personalizzati, è possibile selezionare Marketo Guid come modalità dedicata.

1. Mappatura di ciascuna colonna su un campo Marketo, selezionandolo dall’elenco a discesa.

   ![](assets/image2016-4-13-14-3a36-3a57.png)

   >[!NOTE]
   >
   >Assicuratevi che i valori nel file corrispondano al tipo di campo a cui si sta confrontando (ad es. testo, numero intero, ecc.), in caso contrario il file verrà rifiutato.

1. Fate clic su **Avanti**.

   ![](assets/image2016-4-13-14-3a38-3a41.png)

1. Fate clic su **Importa**.

   ![](assets/image2016-4-7-13-3a15-3a9.png)

   >[!NOTE]
   >
   >Il limite di dimensione per gli oggetti personalizzati è di 100 MB.

   >[!TIP]
   >
   >Inserisci il tuo indirizzo e-mail in **Invia avviso a:** field e Marketo ti invieranno un&#39;e-mail al termine dell&#39;importazione!

1. Nell’angolo in alto a destra della schermata, viene visualizzata una notifica mentre è in esecuzione l’importazione e i risultati finali al termine dell’operazione.

   ![](assets/image2016-4-13-14-3a41-3a1.png)

   Sì!

>[!MORELIKETHIS]
>
>* [Informazioni sugli oggetti personalizzati Marketo](understanding-marketo-custom-objects.md)

>



