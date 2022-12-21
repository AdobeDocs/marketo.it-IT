---
unique-page-id: 11375827
description: Campi obbligatori per la sincronizzazione di Marketo con Dynamics - Documenti Marketo - Documentazione del prodotto
title: Campi richiesti per la sincronizzazione di Marketo con Dynamics
exl-id: c1b9d208-bdc0-4718-b3e5-e9e915b8ae0f
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 0%

---

# Campi richiesti per la sincronizzazione di Marketo con Dynamics {#required-fields-for-syncing-marketo-with-dynamics}

Questi campi *deve* sincronizzato con Marketo sia per lead che per contatti per il funzionamento di Sales Insight:

* Priorità
* Urgenza
* Punteggio relativo

Se manca uno di questi campi, in Marketo verrà visualizzato un messaggio di errore con il nome dei campi mancanti. Per risolvere il problema, accedi all’istanza per assicurarti che i campi siano sincronizzati per entrambi **Lead** e **Contatto**. In caso contrario, aggiungili.

Ecco come verificare e aggiungere campi di sincronizzazione.

1. Vai ad Amministratore e fai clic su **Microsoft Dynamics**.

   ![](assets/image2015-10-9-9-3a50-3a9.png)

1. Fai clic su **Modifica** in Dettagli sincronizzazione campo.

   ![](assets/image2015-10-9-9-3a52-3a23.png)

1. In Lead, seleziona la casella di controllo Priorità .

   ![](assets/image2016-6-8-13-3a33-3a50.png)

1. Ora scorri verso il basso e seleziona la casella di controllo Urgenza .

   ![](assets/image2016-6-8-13-3a35-3a22.png)

1. ...e la casella di controllo Punteggio relativo.

   ![](assets/image2016-6-8-13-3a36-3a1.png)

1. Quindi, seleziona le caselle di controllo Priorità, Urgenza e Punteggio relativo per contatto.

   ![](assets/image2016-6-8-13-3a36-3a36.png)

1. Fai clic su **Salva**.

   ![](assets/image2016-6-8-13-3a41-3a27.png)

>[!NOTE]
>
>Assicurati di attendere almeno 10 minuti prima di eseguire una sincronizzazione prima di verificare di aver risolto il problema.

>[!MORELIKETHIS]
>
>[Impostazione di stelle e fiamme per i record lead/contatti](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/setting-up-and-using/setting-up-stars-and-flames-for-lead-contact-records.md)
