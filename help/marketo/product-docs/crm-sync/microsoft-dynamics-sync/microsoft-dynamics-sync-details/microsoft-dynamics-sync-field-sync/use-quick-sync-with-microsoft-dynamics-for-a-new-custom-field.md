---
unique-page-id: 10098379
description: Utilizzare la sincronizzazione rapida con Microsoft Dynamics per un nuovo campo personalizzato - Documentazione di Marketo - Documentazione del prodotto
title: Utilizzare la sincronizzazione rapida con Microsoft Dynamics per un nuovo campo personalizzato
exl-id: c98f1443-c0dd-40e1-919b-f8110088b38a
feature: Microsoft Dynamics
source-git-commit: 2403ae0f1fdca3b8238f3f59e2a3b94129deb301
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 1%

---

# Utilizzare la sincronizzazione rapida con Microsoft Dynamics per un nuovo campo personalizzato {#use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field}

Il reparto Marketing o Vendite richiede un nuovo campo. O forse ne hai dimenticato uno nella selezione iniziale del campo. Oppure, le tue esigenze sono cambiate. In ogni caso, puoi utilizzare la sincronizzazione rapida per risincronizzare campi specifici.

Normalmente si utilizza la sincronizzazione rapida per aggiungere un nuovo campo e aggiornare i valori. Tuttavia, in alcuni casi potrebbe essere utile sincronizzare un campo esistente. Puoi limitare la sincronizzazione dei campi in base a un intervallo di date aggiornato o creato. Per ulteriori dettagli, consulta [Opzioni di sincronizzazione avanzate](#Advanced_Sync_Options) di seguito.

La sincronizzazione rapida può sincronizzare valori Null. Ad esempio, se utilizzi i valori A e B e modifichi un valore B in Dynamics in null, il valore null verrà sincronizzato con Marketo.

## Sincronizzazione rapida per tutti i record {#quick-sync-for-all-records}

Utilizzare la sincronizzazione rapida per risincronizzare i nuovi campi.

1. In Marketo Engage fare clic su **[!UICONTROL Amministratore]**.

   ![](assets/image2016-8-19-11-3a14-3a5.png)

1. Fare clic su **[!UICONTROL Microsoft Dynamics]**.

   ![](assets/image2016-8-19-11-3a15-3a8.png)

1. In Dettagli sincronizzazione campi fare clic su **[!UICONTROL Modifica]**.

   ![](assets/image2016-8-19-11-3a16-3a22.png)

1. Selezionare i campi da sincronizzare rapidamente e fare clic su **[!UICONTROL Salva]**.

   ![](assets/image2016-8-25-15-3a26-3a11.png)

   >[!NOTE]
   >
   >È possibile selezionare campi da più entità.

1. Riceverai una notifica al termine della sincronizzazione.

   ![](assets/field-sync-update-notification.png)

   >[!CAUTION]
   >
   >La sincronizzazione viene eseguita affiancata ad altre sincronizzazioni e, a seconda delle dimensioni del database, può richiedere molto tempo. Quando un campo si trova in una coda per la sincronizzazione, non è possibile deselezionarlo.

## Opzioni di sincronizzazione avanzate {#advanced-sync-options}

Cosa succede se desideri sincronizzare un campo esistente, ma solo per un set limitato di dati? Ecco come.

1. Deselezionare la casella di controllo per un campo esistente. Fai clic su **[!UICONTROL Salva]**.

   ![](assets/image2016-8-25-16-3a16-3a32.png)

1. Apri nuovamente la finestra a comparsa e riseleziona il campo.

   ![](assets/select-field-reselect-hand.png)

1. Fare clic su **[!UICONTROL Sincronizzazione avanzata]**.

   ![](assets/image2016-8-25-15-3a52-3a9.png)

1. Scegli **[!UICONTROL Aggiornato]** e seleziona un intervallo di date utilizzando i selettori di date. Fai clic su **[!UICONTROL Salva]**.

   ![](assets/image2016-8-25-16-3a0-3a3.png)

   Solo i record aggiornati tra il 8/19/16 e il 9/19/16 verranno sincronizzati rapidamente per il campo.

## Correzione dei campi non sincronizzati {#fixing-out-of-sync-fields}

Nel raro caso in cui un campo Dynamics e Marketo non siano sincronizzati, esiste un modo rapido e semplice per risincronizzarli.

1. Deseleziona il campo e fai clic su **[!UICONTROL Salva]**.

   ![](assets/image2016-8-25-16-3a16-3a32-1.png)

1. Riselezionare il campo e fare clic su **[!UICONTROL Salva]**.

   ![](assets/image2016-8-25-16-3a20-3a45.png)

   Questo dovrebbe aggiustarlo!
