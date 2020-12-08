---
unique-page-id: 10098379
description: Utilizzare la sincronizzazione rapida con Microsoft Dynamics per un nuovo campo personalizzato - Documenti Marketo - Documentazione prodotto
title: Usa sincronizzazione rapida con Microsoft Dynamics per un nuovo campo personalizzato
translation-type: tm+mt
source-git-commit: 313266a67243f0c70c25010cb4825efb7f3db0ab
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 0%

---


# Usa sincronizzazione rapida con Microsoft Dynamics per un nuovo campo personalizzato {#use-quick-sync-with-microsoft-dynamics-for-a-new-custom-field}

Marketing o Vendite vuole un nuovo campo. Oppure, forse ne hai dimenticato uno nella selezione iniziale del campo. Oppure, le vostre esigenze sono cambiate. In ogni caso, potete utilizzare la sincronizzazione rapida per risincronizzare campi specifici.

In genere, per aggiungere un nuovo campo e aggiornare i valori si utilizza la sincronizzazione rapida. Tuttavia, in alcuni casi potrebbe essere utile sincronizzare un campo esistente. Puoi limitare la sincronizzazione dei campi in base a un intervallo di date aggiornato o creato. Consultate Opzioni [di sincronizzazione](#Advanced_Sync_Options) avanzate di seguito.

Sincronizzazione rapida può sincronizzare valori null. Ad esempio, se utilizzi i valori A e B e cambi il valore B in Dynamics su null, sincronizzerà il valore null su Marketo.

## Sincronizzazione rapida per tutti i record {#quick-sync-for-all-records}

Come utilizzare la sincronizzazione rapida per eseguire nuovamente la sincronizzazione per i nuovi campi.

1. In Marketo, fai clic su **Admin**.

   ![](assets/image2016-8-19-11-3a14-3a5.png)

1. Fare clic su** Microsoft Dynamics**.

   ![](assets/image2016-8-19-11-3a15-3a8.png)

1. In Dettagli sincronizzazione campo, fate clic su **Modifica**.

   ![](assets/image2016-8-19-11-3a16-3a22.png)

1. Selezionate i campi da sincronizzare rapidamente e fate clic su **Salva**.

   ![](assets/image2016-8-25-15-3a26-3a11.png)

   >[!NOTE]
   >
   >È possibile selezionare campi da più entità.

1. Al termine della sincronizzazione riceverete una notifica.

   ![](assets/field-sync-update-notification.png)

   >[!CAUTION]
   >
   >La sincronizzazione viene eseguita fianco a fianco con altre sincronizzazioni e, a seconda delle dimensioni del database, il completamento può richiedere molto tempo. Quando un campo è in coda per la sincronizzazione, non è possibile deselezionarlo.

## Opzioni di sincronizzazione avanzate {#advanced-sync-options}

Cosa succede se vuoi sincronizzare un campo esistente, ma solo per un set limitato di dati? Ecco come.

1. Deselezionare la casella di controllo per un campo esistente. Fate clic su **Salva**.

   ![](assets/image2016-8-25-16-3a16-3a32.png)

1. Aprite di nuovo la finestra a comparsa e selezionate nuovamente il campo.

   ![](assets/select-field-reselect-hand.png)

1. Fate clic su Sincronizzazione **** avanzata.

   ![](assets/image2016-8-25-15-3a52-3a9.png)

1. Scegliere **Aggiornato **e selezionare un intervallo di date utilizzando i selettori data. Fate clic su **Salva**.

   ![](assets/image2016-8-25-16-3a0-3a3.png)

   Solo i record aggiornati tra il 19/8/16 e il 19/9/16 verranno sincronizzati rapidamente per il campo.

## Correzione dei campi di sincronizzazione {#fixing-out-of-sync-fields}

Nel raro caso in cui un campo Dynamics e Marketo non siano sincronizzati, esiste un modo rapido e semplice per sincronizzarli.

1. Deselezionate il campo e fate clic su **Salva**.

   ![](assets/image2016-8-25-16-3a16-3a32-1.png)

1. Selezionate nuovamente il campo e fate clic su **Salva**. È tutto!

   ![](assets/image2016-8-25-16-3a20-3a45.png)

   Dovrebbe ripararlo!

