---
unique-page-id: 2952678
description: Utilizzare il token di invio delle informazioni di avviso {{SP_Send_Alert_Info}} - Documentazione Marketo - Documentazione del prodotto
title: Utilizzare il token di invio delle informazioni di avviso
exl-id: 950eb4d1-35d5-4e5c-9624-a38284bff987
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 0%

---

# Utilizzare il token di invio delle informazioni di avviso {#use-the-send-alert-info-token-sp-send-alert-info}

La `{{SP_Send_Alert_Info}}` token è un token speciale da utilizzare per la creazione di e-mail di avviso per il team di vendita.

>[!TIP]
>
>Questo token funziona solo come previsto quando si invia l’e-mail che lo contiene con il [Invia avviso](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md) passaggio di flusso. Non funzionerà se utilizzato in un passaggio di flusso Invia e-mail.

Esempio di avviso:

![](assets/image2014-9-25-15-3a17-3a58.png)

>[!NOTE]
>
>Alzati! Gli URL negli avvisi hanno date di scadenza, quindi assicurati che abbiano una frequenza che supporti questi tipi di messaggi. Le date di scadenza sono [configurato da un amministratore](/help/marketo/product-docs/administration/settings/edit-link-expiration-in-reports-and-alerts.md).

Le seguenti informazioni sono incluse nel `{{SP_Send_Alert_Info}}`:

* Nome e cognome come collegamento al dettaglio della persona in Marketo
* Un collegamento alla persona nel CRM
* Nome della campagna in Marketo che ha inviato l’avviso
* Data di invio dell&#39;avviso

>[!NOTE]
>
>Il collegamento al CRM verrà visualizzato solo se la persona si trova nel sistema CRM (attualmente non disponibile con Dynamics CRM). Il collegamento è accessibile sia agli utenti Marketo che a quelli non Marketo.

## Aggiungi il token SP_Send_Alert_Info a un messaggio e-mail {#add-the-sp-send-alert-info-token-to-an-email}

1. Seleziona l’e-mail e fai clic su **Modifica bozza**.

   ![](assets/one-3.png)

1. Fare doppio clic sull’area modificabile a cui si desidera aggiungere il token.

   ![](assets/two-3.png)

1. Posiziona il cursore nel punto in cui desideri che sia il token, quindi fai clic sul **Inserisci token** pulsante .

   ![](assets/three-3.png)

1. Trova e seleziona la **`{{SP_Send_Alert_Info}}`** token e fai clic su **Inserisci**.

   ![](assets/image2014-9-25-15-3a19-3a11.png)

1. Fai clic su **Salva**.

   ![](assets/image2014-9-25-15-3a19-3a24.png)

>[!NOTE]
>
>Non dimenticarti di approvare la tua e-mail.

Brava roba! Questo token è molto utile e dovrebbe essere utilizzato in tutti gli avvisi creati per il team di vendita.
