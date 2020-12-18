---
unique-page-id: 14352477
description: Push to Sales Connect - Marketo Docs - Documentazione prodotto
title: Push to Sales Connect
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---


# Push to Sales Connect {#push-to-sales-connect}

Il nostro pulsante Premi a Tout fornirà un elenco dei lead/contatti in Salesforce e li invierà a un gruppo in Sales Connect. Potete quindi inviare rapidamente un&#39;e-mail di gruppo personalizzabile con tracciamento del Tout allegato.

## Requisiti {#requirements}

* Connect di vendita [Pacchetto Salesforce](http://docs.marketo.com/x/C4PS) installato da `Salesforce Admin`

* `Push to Sales Connect`pulsante installato nella visualizzazione elenco per  `Salesforce Admin`

* Connessione Salesforce realizzata con Sales Connect per gli utenti che eseguono il push

## Come {#how-to}

1. Fare clic sulla scheda **Lead/Contact** in Salesforce.
1. Passate alla vista Elenco a cui desiderate aggiungere il pulsante Premi per il collegamento vendite accanto al pulsante Vai.
1. Fare clic su **Go**.
1. Seleziona tutti i lead/contatti che desideri inviare al tout.
1. Selezionare **Push to MSE**.
1. Viene visualizzata una nuova finestra per verificare il numero di lead/contatti da spostare. Selezionare **Procedi a Group**. Connect vendite `will not push over` tutti i contatti contrassegnati come `Email Opt Out` in Salesforce o `Unsubscribed` in Sales Connect.

   >[!NOTE]
   >
   >In Sales Connect verrà aggiunto il gruppo denominato &quot;SFDC-...&quot; nella pagina Relazioni dell&#39; [applicazione Web](http://toutapp.com/login).

1. Selezionare **Email Entire Group** per inviare l&#39;e-mail del gruppo.

