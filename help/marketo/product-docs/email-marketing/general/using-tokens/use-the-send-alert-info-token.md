---
unique-page-id: 2952678
description: Utilizzare il token Invia informazioni avviso {{SP_Send_Alert_Info}} - Documenti Marketo - Documentazione prodotto
title: Utilizzare il token Invia informazioni avviso
translation-type: tm+mt
source-git-commit: 1a29614ec938074902af201b2ffc11cfaa625f7a
workflow-type: tm+mt
source-wordcount: '316'
ht-degree: 0%

---


# Utilizzare il token Invia informazioni avviso {#use-the-send-alert-info-token-sp-send-alert-info}

Il `{{SP_Send_Alert_Info}}` token è un token speciale da utilizzare per la creazione di e-mail di avviso per il team di vendita.

>[!NOTE]
>
>**FYI**
>
>Marketo sta standardizzando la lingua tra tutte le iscrizioni, pertanto è possibile che nell&#39;abbonamento siano presenti lead/lead e persone in docs.marketo.com. Questi termini significano la stessa cosa; non influisce sulle istruzioni dell&#39;articolo. Ci sono anche altri cambiamenti. [Ulteriori](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)informazioni.

>[!TIP]
>
>Questo token funziona solo come previsto quando si invia l’e-mail che lo contiene con il passaggio del flusso di [invio avvisi](../../../../product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md) . Non funzionerà se utilizzato in un passaggio Invia flusso e-mail.

Esempio di avviso:   ![](assets/image2014-9-25-15-3a17-3a58.png)

>[!NOTE]
>
>Testa! Gli URL negli avvisi dispongono di date di scadenza, pertanto accertati che dispongano di cadenza tale da supportare questi tipi di messaggi. Le date di scadenza sono [configurate da un amministratore](../../../../product-docs/administration/settings/edit-link-expiration-in-reports-and-alerts.md).

Le seguenti informazioni sono incluse nell&#39; `{{SP_Send_Alert_Info}}`:

* Nome e cognome come collegamento al dettaglio della persona in Marketo
* Un collegamento alla persona nel CRM
* Nome della campagna in Marketo che ha inviato l’avviso
* Data e ora di invio dell’avviso

>[!NOTE]
>
>Il collegamento a CRM verrà visualizzato solo se la persona è nel sistema CRM (attualmente non disponibile con Dynamics CRM). Il collegamento è accessibile sia agli utenti di Marketo che a quelli non di Marketo.

## Aggiungere il token SP_Send_Alert_Info a un messaggio e-mail {#add-the-sp-send-alert-info-token-to-an-email}

1. Selezionate l’e-mail e fate clic su **Modifica bozza**.

   ![](assets/one-3.png)

1. Fare doppio clic sull&#39;area modificabile a cui si desidera aggiungere il token.

   ![](assets/two-3.png)

1. Posizionare il cursore nel punto in cui si desidera inserire il token, quindi fare clic sul pulsante **Inserisci token** .

   ![](assets/three-3.png)

1. Individuate e selezionate il **`{{SP_Send_Alert_Info}}`** token e fate clic su **Inserisci**.

   ![](assets/image2014-9-25-15-3a19-3a11.png)

1. Fate clic su **Salva**.

   ![](assets/image2014-9-25-15-3a19-3a24.png)

>[!NOTE]
>
>**Promemoria**
>
>Non dimenticare di approvare la tua e-mail.

Buona roba! Questo token è molto utile e dovrebbe essere utilizzato in tutti gli avvisi creati per il team di vendita.