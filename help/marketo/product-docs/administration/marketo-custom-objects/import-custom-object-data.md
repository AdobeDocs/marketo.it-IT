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

È facile importare dati oggetto personalizzati nel database. Se utilizzi oggetti personalizzati con le aziende, consulta [Utilizzo di oggetti personalizzati con le aziende](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md#using-custom-objects-with-companies) per ulteriori informazioni.

1. In Il mio Marketo, vai a **[!UICONTROL Database]**.

   ![](assets/import-custom-object-data-1.png)

1. Clic **[!UICONTROL Nuovo]** e seleziona **[!UICONTROL Importa dati oggetto personalizzati]**.

   ![](assets/import-custom-object-data-2.png)

1. Clic **[!UICONTROL Sfoglia]** per individuare il file di dati. Selezionare il formato del file (valori separati da virgola in questo esempio).

   ![](assets/import-custom-object-data-3.png)

1. Seleziona il [!UICONTROL oggetto personalizzato].

   ![](assets/import-custom-object-data-4.png)

1. Seleziona la [!UICONTROL Modalità di deduplicazione] dal menu a discesa. Clic **[!UICONTROL Successivo]**.

   ![](assets/import-custom-object-data-5.png)

   >[!NOTE]
   >
   >Utilizzare i campi di deduplicazione come identificatori univoci quando si creano o si aggiornano record oggetto personalizzati. In questo esempio viene utilizzato il campo Dedupe del **automobile** oggetto personalizzato - vin (numero ID veicolo). Se si aggiornano solo record oggetto personalizzati, è possibile selezionare [!UICONTROL GUID MARKETO] come [!UICONTROL Modalità di deduplicazione].

1. Mappa ciascuna colonna su un campo Marketo, selezionandola dall’elenco a discesa.

   ![](assets/import-custom-object-data-6.png)

   >[!NOTE]
   >
   >Assicurati che i valori nel file corrispondano al tipo di campo a cui stai corrispondendo (ad esempio, testo, numero intero, ecc.), altrimenti il file verrà rifiutato.

1. Clic **[!UICONTROL Successivo]**.

   ![](assets/import-custom-object-data-7.png)

1. Clic **[!UICONTROL Importa]**.

   ![](assets/import-custom-object-data-8.png)

   >[!NOTE]
   >
   >Il limite di dimensione per gli oggetti personalizzati è di 100 MB.

   >[!TIP]
   >
   >Inserisci il tuo indirizzo e-mail in **[!UICONTROL Invia avviso a]** e Marketo ti invierà un’e-mail al termine dell’importazione.

1. Nell’angolo in alto a destra dello schermo viene visualizzata una notifica mentre l’importazione è in esecuzione e al termine vengono visualizzati i risultati finali.

   ![](assets/import-custom-object-data-9.png)

   Yay!

>[!MORELIKETHIS]
>
>[Informazioni sugli oggetti personalizzati di Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
