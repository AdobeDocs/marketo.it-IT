---
unique-page-id: 10099680
description: Importare dati oggetto personalizzati - Documentazione di Marketo - Documentazione del prodotto
title: Importare i dati dell’oggetto personalizzato
exl-id: ee11199a-57ca-47ec-8f59-8384a93ea05e
feature: Custom Objects
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '212'
ht-degree: 5%

---

# Importare i dati dell’oggetto personalizzato {#import-custom-object-data}

È facile importare dati oggetto personalizzati nel database. Se utilizzi oggetti personalizzati con aziende, consulta [Utilizzo di oggetti personalizzati con aziende](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md#using-custom-objects-with-companies) per ulteriori informazioni.

1. In Il mio Marketo, vai a **[!UICONTROL Database]**.

   ![](assets/import-custom-object-data-1.png)

1. Fare clic su **[!UICONTROL New]** e selezionare **[!UICONTROL Import Custom Object Data]**.

   ![](assets/import-custom-object-data-2.png)

1. Fare clic su **[!UICONTROL Browse]** per individuare il file di dati. Selezionare il formato del file (valori separati da virgola in questo esempio).

   ![](assets/import-custom-object-data-3.png)

1. Seleziona [!UICONTROL custom object].

   ![](assets/import-custom-object-data-4.png)

1. Selezionare [!UICONTROL Dedupe Mode] dal menu a discesa. Fai clic su **[!UICONTROL Next]**.

   ![](assets/import-custom-object-data-5.png)

   >[!NOTE]
   >
   >Utilizzare i campi di deduplicazione come identificatori univoci quando si creano o si aggiornano record oggetto personalizzati. In questo esempio viene utilizzato il campo Dedupe dell&#39;oggetto personalizzato **car** - vin (numero ID veicolo). Se si aggiornano solo record oggetto personalizzati, è possibile selezionare [!UICONTROL Marketo Guid] come [!UICONTROL Dedupe Mode].

1. Mappa ciascuna colonna su un campo Marketo, selezionandola dall’elenco a discesa.

   ![](assets/import-custom-object-data-6.png)

   >[!NOTE]
   >
   >Assicurati che i valori nel file corrispondano al tipo di campo a cui stai corrispondendo (ad esempio, testo, numero intero, ecc.), altrimenti il file verrà rifiutato.

1. Fai clic su **[!UICONTROL Next]**.

   ![](assets/import-custom-object-data-7.png)

1. Fai clic su **[!UICONTROL Import]**.

   ![](assets/import-custom-object-data-8.png)

   >[!NOTE]
   >
   >Il limite di dimensione per gli oggetti personalizzati è di 100 MB.

   >[!TIP]
   >
   >Immetti il tuo indirizzo e-mail nel campo **[!UICONTROL Send Alert To]** e Marketo ti invierà un&#39;e-mail al termine dell&#39;importazione.

1. Nell’angolo in alto a destra dello schermo viene visualizzata una notifica mentre l’importazione è in esecuzione e al termine vengono visualizzati i risultati finali.

   ![](assets/import-custom-object-data-9.png)

   Yay!

>[!MORELIKETHIS]
>
>[Informazioni sugli oggetti personalizzati di Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
