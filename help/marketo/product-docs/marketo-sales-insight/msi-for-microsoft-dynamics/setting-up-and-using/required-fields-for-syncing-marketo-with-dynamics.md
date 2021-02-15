---
unique-page-id: 11375827
description: Campi obbligatori per la sincronizzazione del Marketo con Dynamics - Marketo Docs - Documentazione prodotto
title: Campi obbligatori per la sincronizzazione del marketing con Dynamics
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 0%

---


# Campi obbligatori per la sincronizzazione del marketing con Dynamics {#required-fields-for-syncing-marketo-with-dynamics}

Questi campi *devono essere sincronizzati con Marketo sia per il lead che per il funzionamento di Contatto per il reparto Vendite:*

* Priorità
* Urgenza
* Punteggio relativo

Se manca uno di questi campi, in Marketo verrà visualizzato un messaggio di errore con il nome dei campi mancanti. Per risolvere il problema, verificare che i campi siano sincronizzati sia per **Lead** che per **Contact**. In caso contrario, aggiungeteli.

Questo è il modo in cui verificare e aggiungere campi di sincronizzazione.

1. Vai ad Admin e fai clic su **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Fare clic su **Modifica** in Dettagli sincronizzazione campo.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. In Lead, seleziona la casella Priorità.

   ![](assets/image2016-6-8-13-3a33-3a50.png)

1. A questo punto, scorrete verso il basso e selezionate la casella di controllo Urgenza...

   ![](assets/image2016-6-8-13-3a35-3a22.png)

1. ...e la casella Valutazione relativa.

   ![](assets/image2016-6-8-13-3a36-3a1.png)

1. Quindi, selezionare le caselle di controllo relative a Priorità, Urgenza e Valutazione relativa per contatto.

   ![](assets/image2016-6-8-13-3a36-3a36.png)

1. Fare clic su **Salva**.

   ![](assets/image2016-6-8-13-3a41-3a27.png)

>[!NOTE]
>
>Prima di verificare di aver risolto il problema, attendete almeno 10 minuti prima di eseguire la sincronizzazione.

>[!MORELIKETHIS]
>
>[Impostazione di stelle e fiamme per i record lead/contatto](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
