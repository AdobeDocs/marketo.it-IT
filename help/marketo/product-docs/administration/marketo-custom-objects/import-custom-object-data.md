---
unique-page-id: 10099680
description: Importare dati oggetto personalizzati - Documentazione di Marketo - Documentazione del prodotto
title: Importa dati oggetto personalizzati
exl-id: ee11199a-57ca-47ec-8f59-8384a93ea05e
feature: Custom Objects
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 0%

---

# Importa dati oggetto personalizzati {#import-custom-object-data}

È facile importare dati oggetto personalizzati nel database. Se utilizzi oggetti personalizzati con aziende, consulta [Utilizzo di oggetti personalizzati con aziende](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md#using-custom-objects-with-companies) per ulteriori informazioni.

1. In Il mio Marketo, passa a **[!UICONTROL Database]**.

   ![](assets/import-custom-object-data-1.png)

1. Fai clic su **[!UICONTROL Nuovo]** e seleziona **[!UICONTROL Importa dati oggetto personalizzati]**.

   ![](assets/import-custom-object-data-2.png)

1. Fare clic su **[!UICONTROL Sfoglia]** per individuare il file di dati. Selezionare il formato del file (valori separati da virgola in questo esempio).

   ![](assets/import-custom-object-data-3.png)

1. Seleziona il tuo [!UICONTROL oggetto personalizzato].

   ![](assets/import-custom-object-data-4.png)

1. Selezionare la [!UICONTROL Modalità di deduplicazione] dal menu a discesa. Fai clic su **[!UICONTROL Avanti]**.

   ![](assets/import-custom-object-data-5.png)

   >[!NOTE]
   >
   >Utilizzare i campi di deduplicazione come identificatori univoci quando si creano o si aggiornano record oggetto personalizzati. In questo esempio viene utilizzato il campo Dedupe dell&#39;oggetto personalizzato **car** - vin (numero ID veicolo). Se si aggiornano solo record oggetto personalizzati, è possibile selezionare il [!UICONTROL GUID Marketo] come [!UICONTROL Modalità di deduplicazione].

1. Mappa ciascuna colonna su un campo Marketo, selezionandola dall’elenco a discesa.

   ![](assets/import-custom-object-data-6.png)

   >[!NOTE]
   >
   >Assicurati che i valori nel file corrispondano al tipo di campo a cui stai corrispondendo (ad esempio, testo, numero intero, ecc.), altrimenti il file verrà rifiutato.

1. Fai clic su **[!UICONTROL Avanti]**.

   ![](assets/import-custom-object-data-7.png)

1. Fai clic su **[!UICONTROL Importa]**.

   ![](assets/import-custom-object-data-8.png)

   >[!NOTE]
   >
   >Il limite di dimensione per gli oggetti personalizzati è di 100 MB.

   >[!TIP]
   >
   >Immetti il tuo indirizzo e-mail nel campo **[!UICONTROL Invia avviso a]** e Marketo ti invierà un&#39;e-mail al termine dell&#39;importazione.

1. Nell’angolo in alto a destra dello schermo viene visualizzata una notifica mentre l’importazione è in esecuzione e al termine vengono visualizzati i risultati finali.

   ![](assets/import-custom-object-data-9.png)

   Yay!

>[!MORELIKETHIS]
>
>[Informazioni sugli oggetti personalizzati di Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
