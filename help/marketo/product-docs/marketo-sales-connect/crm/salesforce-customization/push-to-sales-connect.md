---
unique-page-id: 14352477
description: Push to Sales Connect - Marketo Docs - Documentazione prodotto
title: Push to Sales Connect
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 0%

---


# Push to Sales Connect {#push-to-sales-connect}

Il nostro pulsante Premi a Tout fornirà un elenco dei lead/contatti in Salesforce e li invierà a un gruppo in Sales Connect. Potete quindi inviare rapidamente un&#39;e-mail di gruppo personalizzabile con tracciamento del Tout allegato.

## Requisiti {#requirements}

* Pacchetto Salesforce di Sales Connect installato dall&#39;amministratore Salesforce

* Pulsante Push to Sales Connect installato dall&#39;amministratore Salesforce per visualizzare l&#39;elenco

* Connessione Salesforce realizzata con Sales Connect per gli utenti che eseguono il push

## Come {#how-to}

1. Fare clic sulla scheda **Lead/Contact** in Salesforce.
1. Passate alla vista Elenco a cui desiderate aggiungere il pulsante Premi per il collegamento vendite accanto al pulsante Vai.
1. Fare clic su **Go**.
1. Seleziona tutti i lead/contatti che desideri inviare al tout.
1. Selezionare **Push to MSE**.
1. Viene visualizzata una nuova finestra per verificare il numero di lead/contatti da spostare. Selezionare **Procedi a Group**. I servizi di vendita Connect non eseguiranno il push dei contatti contrassegnati come Rifiuto e-mail in Salesforce o Annulla sottoscrizione in Sales Connect.

   >[!NOTE]
   >
   >In Sales Connect verrà aggiunto il gruppo denominato &quot;SFDC-...&quot; nella pagina Relazioni dell&#39; [applicazione Web](http://toutapp.com/login).

1. Selezionare **Email Entire Group** per inviare l&#39;e-mail del gruppo.
