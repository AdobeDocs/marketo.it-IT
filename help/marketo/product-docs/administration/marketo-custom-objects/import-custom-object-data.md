---
unique-page-id: 10099680
description: Importare dati di oggetti personalizzati - Documenti Marketo - Documentazione del prodotto
title: Importa dati oggetto personalizzati
exl-id: ee11199a-57ca-47ec-8f59-8384a93ea05e
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 0%

---

# Importa dati oggetto personalizzati {#import-custom-object-data}

È facile importare dati di oggetti personalizzati nel database. Se utilizzi oggetti personalizzati con aziende, consulta [Utilizzo di oggetti personalizzati con le aziende](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md#using-custom-objects-with-companies) per ulteriori informazioni.

1. In My Marketo, vai a **Database**.

   ![](assets/db-1.png)

1. Fai clic su **Nuovo** e seleziona **Importa dati oggetto personalizzati**.

   ![](assets/image2016-4-7-10-6-54.png)

1. Fai clic su **Sfoglia** per individuare il file di dati. Selezionare il formato del file (Comma Separated Values in questo esempio).

   ![](assets/image2016-4-13-14-3a21-3a53.png)

1. Seleziona l’oggetto personalizzato.

   ![](assets/image2016-4-13-14-3a24-3a54.png)

1. Seleziona la Modalità di deduplicazione dal menu a discesa. Fai clic su **Successivo**.

   ![](assets/image2016-4-13-14-3a28-3a7.png)

   >[!NOTE]
   >
   >Utilizzare i campi Deduplice come identificatori univoci quando si creano o aggiornano record di oggetti personalizzati. In questo esempio viene utilizzato il campo Deduplice del **auto** oggetto personalizzato - vin (numero ID veicolo). Se si aggiornano solo i record di oggetti personalizzati, è possibile selezionare Marketo Guid come modalità dedicata.

1. Mappa ciascuna colonna su un campo Marketo, selezionandola dall’elenco a discesa.

   ![](assets/image2016-4-13-14-3a36-3a57.png)

   >[!NOTE]
   >
   >Assicurati che i valori nel file corrispondano al tipo di campo a cui stai confrontando (ad es. testo, numero intero, ecc.), altrimenti il file verrà rifiutato.

1. Fai clic su **Successivo**.

   ![](assets/image2016-4-13-14-3a38-3a41.png)

1. Fai clic su **Importa**.

   ![](assets/image2016-4-7-13-3a15-3a9.png)

   >[!NOTE]
   >
   >Il limite di dimensione per gli oggetti personalizzati è di 100 MB.

   >[!TIP]
   >
   >Inserisci il tuo indirizzo e-mail nel **Invia avviso a:** campo e Marketo ti invierà un&#39;e-mail al termine dell&#39;importazione!

1. Nell’angolo in alto a destra della schermata, viene visualizzata una notifica mentre l’importazione è in esecuzione e i risultati finali al termine dell’importazione.

   ![](assets/image2016-4-13-14-3a41-3a1.png)

   Yay!

>[!MORELIKETHIS]
>
>[Informazioni sugli oggetti personalizzati Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
