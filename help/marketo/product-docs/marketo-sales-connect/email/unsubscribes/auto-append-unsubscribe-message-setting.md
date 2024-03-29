---
description: Aggiungi automaticamente l’impostazione dei messaggi di annullamento dell’abbonamento - Documentazione di Marketo - Documentazione del prodotto
title: Aggiungi automaticamente l’impostazione del messaggio di annullamento dell’iscrizione
feature: Marketo Sales Connect
exl-id: 8aa75123-f6b5-4dfe-8fa7-f764620c04e8
source-git-commit: 7c8703059d7d28afbf57f4f285ac972fb9d8fbef
workflow-type: tm+mt
source-wordcount: '198'
ht-degree: 0%

---

# Aggiungi automaticamente l’impostazione del messaggio di annullamento dell’iscrizione {#auto-append-unsubscribe-message-setting}

Assicurati che ogni e-mail inviata includa un messaggio per annullare l’iscrizione in modo che i destinatari abbiano una facile opzione per rinunciare alle comunicazioni. Quando è abilitato il messaggio di annullamento dell’iscrizione accodamento, tutte le comunicazioni inviate dal team da Marketo Sales includeranno un messaggio di annullamento dell’iscrizione, incluse le e-mail inviate dall’applicazione web, Salesforce, il plug-in Gmail e il plug-in di Outlook.

## Aspetti da considerare {#things-to-note}

* Per le e-mail inviate dai plug-in, l’annullamento dell’abbonamento verrà aggiunto solo quando viene utilizzato un modello.

* Se si utilizza `{{team_unsubscribe}}` campo dinamico in un modello e-mail e l’impostazione di aggiunta del messaggio di annullamento dell’iscrizione è abilitata, il campo dinamico di annullamento dell’iscrizione del team popolerà il messaggio di annullamento dell’iscrizione _invece di_ aggiunta del messaggio per annullare l’abbonamento.

## Abilita/Disabilita annulla iscrizione accodamento {#enable-disable-unsubscribe-append}

1. Fai clic sull’icona a forma di ingranaggio e seleziona **Impostazioni**.

   ![](assets/auto-append-unsubscribe-message-setting-1.png)

1. In Impostazioni Amministratore, Fai Clic Su **Annulla iscrizione**.

   ![](assets/auto-append-unsubscribe-message-setting-2.png)

1. Nella scheda Messaggistica, in Aggiungi messaggio di annullamento iscrizione, sposta il dispositivo di scorrimento sullo stato desiderato.

   ![](assets/auto-append-unsubscribe-message-setting-3.png)

>[!TIP]
>
>Se disattivi l’impostazione di aggiunta del messaggio di annullamento dell’iscrizione, ti consigliamo di aggiungere ai modelli un piè di pagina di annullamento dell’iscrizione per garantire che la comunicazione disponga di un’opzione di rinuncia. A tale scopo, puoi aggiungere un messaggio personalizzato a ciascun modello oppure utilizzare `{{team_unsubscribe}}` [campo dinamico](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/dynamic-fields-glossary.md){target="_blank"}.
