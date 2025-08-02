---
description: Aggiungi automaticamente l’impostazione dei messaggi di annullamento dell’abbonamento - Documentazione di Marketo - Documentazione del prodotto
title: Aggiungi automaticamente l’impostazione del messaggio di annullamento dell’iscrizione
feature: Sales Insight Actions
exl-id: 17734f62-74e6-4168-a9c8-7835e3daf5ff
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '175'
ht-degree: 0%

---

# Aggiungi automaticamente l’impostazione del messaggio di annullamento dell’iscrizione {#auto-append-unsubscribe-message-setting}

Assicurati che ogni e-mail Azioni di Sales Insight inviata includa un messaggio per annullare l’iscrizione in modo che i destinatari abbiano una facile opzione per rinunciare alla comunicazione. Quando è abilitato il messaggio di annullamento dell’iscrizione accodamento, tutte le comunicazioni inviate dal team da Marketo Sales includeranno un messaggio di annullamento dell’iscrizione, incluse le e-mail inviate dall’applicazione web e da Salesforce.

>[!NOTE]
>
>Se si utilizza il campo dinamico `{{team_unsubscribe}}` in un modello di messaggio di posta elettronica e l&#39;impostazione di accodamento del messaggio di annullamento dell&#39;iscrizione è abilitata, il campo dinamico di annullamento dell&#39;iscrizione del team popolerà il messaggio di annullamento dell&#39;iscrizione _anziché_ accodando il messaggio di annullamento dell&#39;iscrizione.

## Abilita/Disabilita annulla iscrizione accodamento {#enable-disable-unsubscribe-append}

1. Fai clic sull&#39;icona a forma di ingranaggio e seleziona **Impostazioni**.

   ![](assets/auto-append-unsubscribe-message-setting-1.png)

1. In Impostazioni Amministrazione Fare Clic Su **Annulla Sottoscrizione**.

   ![](assets/auto-append-unsubscribe-message-setting-2.png)

1. Nella scheda Messaggistica, in Aggiungi messaggio di annullamento iscrizione, sposta il dispositivo di scorrimento sullo stato desiderato.

   ![](assets/auto-append-unsubscribe-message-setting-3.png)

>[!TIP]
>
>Se disattivi l’impostazione di aggiunta del messaggio di annullamento dell’iscrizione, ti consigliamo di aggiungere ai modelli un piè di pagina di annullamento dell’iscrizione per garantire che la comunicazione disponga di un’opzione di rinuncia. Per eseguire questa operazione, aggiungere un messaggio personalizzato a ogni modello oppure utilizzare il `{{team_unsubscribe}}` [campo dinamico](/help/marketo/product-docs/marketo-sales-insight/actions/templates/dynamic-fields.md){target="_blank"}.
