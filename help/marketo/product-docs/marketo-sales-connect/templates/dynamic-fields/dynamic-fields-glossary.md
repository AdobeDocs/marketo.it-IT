---
unique-page-id: 14352509
description: Glossario dei campi dinamici - Documentazione di Marketo - Documentazione del prodotto
title: Glossario dei campi dinamici
exl-id: 28351ba9-53da-4408-9526-918200d9bd29
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '240'
ht-degree: 3%

---

# Glossario dei campi dinamici {#dynamic-fields-glossary}

Durante la creazione di un modello in [!DNL Sales Connect], si consiglia sempre di integrare i campi dinamici mediante il pulsante **[!UICONTROL MSE Dynamic Fields]**.

Questo strumento viene utilizzato per `auto-personalize your email` e consente di risparmiare tonnellate di tempo entro `pulling information from the [!UICONTROL People] page`.

| Campo dinamico | Esempio di cosa viene visualizzato nell’e-mail |
|---|---|
| `{{company}}` | Adobe |
| `{{company_friendly}}` | Adobe |
| `{{first_name}}` | Keith |
| `{{team_unsubscribe}}` | Se non desideri più ricevere e-mail da noi, fai clic qui |
| `{{friendly_unsubscribe}}` | Stanco di tutte le email? Per favore, fammelo sapere qui |
| `{{my_name}}` | Keith Flynn |
| `{{my_signature}}` | Keith Flynn, Senior Technical Writer di Adobe |
| `{{personal_email}}` | <keith@pickyouremail.com> |
| `{{title}}` | Scrittore tecnico senior |
| `{{work_website}}` | <https://www.adobe.com> |

**Aspetti da considerare**:

* Se le informazioni di un contatto non vengono immesse correttamente o non sono presenti nella pagina Persone, non verranno inserite correttamente nel modello.
* La differenza tra `{{company}}` e `{{company_friendly}}` è che `{{company_friendly}}` rimuoverà qualsiasi titolo formale, ad esempio Inc., LLC., ecc., dal nome della società del contatto.
* Quando utilizzi `{{company_friendly}}`, assicurati di separare Inc. o Co. con una virgola nei dettagli di contatto. In questo modo Sales Connect sa cosa rimuovere quando si richiama il valore.
* Il sistema aggiunge automaticamente la firma dell&#39;utente a ogni e-mail inviata. Se l&#39;utente utilizza un modello con il campo dinamico `{{my_signature}}`, il sistema compilerà la firma in cui è stato inserito il campo dinamico `{{my_signature}}`. Viene aggiunto solo per evitare duplicazioni. Il sistema gestirà `{{team_unsubscribe}}` nello stesso modo quando è abilitata l&#39;impostazione globale per l&#39;annullamento dell&#39;abbonamento.

>[!TIP]
>
>Puoi creare il tuo [campo dinamico personalizzato](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/create-custom-dynamic-fields.md) per tutto ciò che desideri inserire automaticamente nelle e-mail
