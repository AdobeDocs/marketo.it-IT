---
unique-page-id: 11375827
description: Campi obbligatori per la sincronizzazione di Marketo con Dynamics - Documentazione di Marketo - Documentazione del prodotto
title: Campi obbligatori per la sincronizzazione di Marketo con Dynamics
exl-id: c1b9d208-bdc0-4718-b3e5-e9e915b8ae0f
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 0%

---

# Campi obbligatori per la sincronizzazione di Marketo con Dynamics {#required-fields-for-syncing-marketo-with-dynamics}

Questi campi *deve* sincronizzarsi con Marketo per il funzionamento sia di Lead che di Contact for Sales Insight:

* Priorità
* Urgenza
* Punteggio relativo

Se manca uno di questi campi, in Marketo verrà visualizzato un messaggio di errore con il nome dei campi mancanti. Per risolvere questo problema, controlla nell’istanza per assicurarti che i campi siano sincronizzati per entrambi **Lead** e **Contatto**. In caso contrario, aggiungili.

Ecco come verificare e aggiungere campi di sincronizzazione.

1. Vai a Amministratore e fai clic su **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Clic **Modifica** in Dettagli sincronizzazione campi.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. In Lead selezionare la casella di controllo Priorità.

   ![](assets/image2016-6-8-13-3a33-3a50.png)

1. Ora, scorri verso il basso e seleziona la casella Urgenza...

   ![](assets/image2016-6-8-13-3a35-3a22.png)

1. e la casella di controllo Punteggio relativo.

   ![](assets/image2016-6-8-13-3a36-3a1.png)

1. Quindi, seleziona le caselle di controllo Priorità, Urgenza e Punteggio relativo per Contatto.

   ![](assets/image2016-6-8-13-3a36-3a36.png)

1. Clic **Salva**.

   ![](assets/image2016-6-8-13-3a41-3a27.png)

>[!NOTE]
>
>Prima di verificare di aver risolto il problema, attendi almeno 10 minuti per l’esecuzione di una sincronizzazione.

>[!MORELIKETHIS]
>
>[Impostazione di stelle e fiamme per record lead/contatti](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
