---
unique-page-id: 14352477
description: Push to Sales Connect - Documentazione Marketo - Documentazione del prodotto
title: Push to Sales Connect
exl-id: 8fb99d28-d6c6-47c3-b4d2-c416251aff47
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 0%

---

# Push to Sales Connect {#push-to-sales-connect}

Il nostro pulsante Push to Tout prenderà un elenco dei vostri lead/contatti in Salesforce e li spingerà in un gruppo in Sales Connect. Puoi quindi inviare rapidamente un’e-mail di gruppo personalizzabile con tracciamento Tout allegato.

## Requisiti {#requirements}

* Pacchetto Salesforce Sales Connect installato da Salesforce Admin

* Pulsante Push to Sales Connect installato nella visualizzazione elenco da Salesforce Admin

* Connessione Salesforce effettuata con Sales Connect per l&#39;utente che effettua il push

## Come fare per {#how-to}

1. Fai clic sul pulsante **Lead/Contatto** scheda in Salesforce.
1. Passa alla vista Elenco da premere per la connessione alle vendite accanto al pulsante Vai.
1. Fai clic su **Vai**.
1. Seleziona tutti i lead/contatti che desideri inviare al tout.
1. Seleziona **Invia a MSE**.
1. Viene visualizzata una nuova finestra che verifica il numero di lead/contatti da spingere. Seleziona **Procedi al gruppo**. Sales Connect non eseguirà il push di contatti contrassegnati come Rinuncia via e-mail in Salesforce o Annulla sottoscrizione in Sales Connect.

   >[!NOTE]
   >
   >Sales Connect aggiunge questo gruppo denominato &quot;SFDC-...&quot; alla pagina Relazioni della [applicazione web](https://toutapp.com/login).

1. Seleziona **Invia a tutto il gruppo e-mail** per inviare questa e-mail di gruppo.
