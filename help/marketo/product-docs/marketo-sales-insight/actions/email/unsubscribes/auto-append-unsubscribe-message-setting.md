---
description: Aggiungi automaticamente l’impostazione dei messaggi di annullamento dell’abbonamento - Documentazione di Marketo - Documentazione del prodotto
title: Aggiungi automaticamente l’impostazione del messaggio di annullamento dell’iscrizione
hide: true
hidefromtoc: true
feature: Sales Insight Actions
source-git-commit: 8b2eed5e28c46ea9c467fd25dd732c1654a09bed
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 0%

---

# Aggiungi automaticamente l’impostazione del messaggio di annullamento dell’iscrizione {#auto-append-unsubscribe-message-setting}

Assicurati che ogni e-mail di Sales Insight Actions (Azioni di approfondimento sulle vendite) inviata includa un messaggio di annullamento dell’iscrizione in modo che i destinatari abbiano una facile opzione per rifiutare la comunicazione. Quando è abilitato il messaggio di annullamento dell’abbonamento, tutte le comunicazioni inviate dal team da Marketo Sales includeranno un messaggio di annullamento dell’abbonamento, incluse le e-mail inviate dall’applicazione web e da Salesforce.

>[!NOTE]
>
>Se si utilizza `{{team_unsubscribe}}` campo dinamico in un modello e-mail e l’impostazione di aggiunta del messaggio di annullamento dell’iscrizione è abilitata, il campo dinamico di annullamento dell’iscrizione del team popolerà il messaggio di annullamento dell’iscrizione _invece di_ aggiunta del messaggio per annullare l’abbonamento.

## Abilita/Disabilita annulla iscrizione accodamento {#enable-disable-unsubscribe-append}

1. Fai clic sull’icona a forma di ingranaggio e seleziona **Impostazioni**.

   ![](assets/auto-append-unsubscribe-message-setting-1.png)

1. In Impostazioni Amministratore, Fai Clic Su **Annulla iscrizione**.

   ![](assets/auto-append-unsubscribe-message-setting-2.png)

1. Nella scheda Messaggistica, in Aggiungi messaggio di annullamento iscrizione, sposta il dispositivo di scorrimento sullo stato desiderato.

   ![](assets/auto-append-unsubscribe-message-setting-3.png)

>[!TIP]
>
>Se disattivi l’impostazione di aggiunta del messaggio di annullamento dell’iscrizione, ti consigliamo di aggiungere ai modelli un piè di pagina di annullamento dell’iscrizione per garantire che la comunicazione disponga di un’opzione di rinuncia. A tale scopo, puoi aggiungere un messaggio personalizzato a ciascun modello oppure utilizzare `{{team_unsubscribe}}` [campo dinamico](/help/marketo/product-docs/marketo-sales-insight/actions/templates/dynamic-fields.md){target="_blank"}.
