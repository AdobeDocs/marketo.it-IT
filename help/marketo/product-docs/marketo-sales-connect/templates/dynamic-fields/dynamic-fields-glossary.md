---
unique-page-id: 14352509
description: Glossario dei campi dinamici - Documentazione di Marketo - Documentazione del prodotto
title: Glossario dei campi dinamici
exl-id: 28351ba9-53da-4408-9526-918200d9bd29
feature: Marketo Sales Connect
source-git-commit: 7c8703059d7d28afbf57f4f285ac972fb9d8fbef
workflow-type: tm+mt
source-wordcount: '208'
ht-degree: 0%

---

# Glossario dei campi dinamici {#dynamic-fields-glossary}

Durante la creazione di un modello in Sales Connect, è sempre consigliabile integrare i campi dinamici utilizzando **Campi dinamici MSE** pulsante.

Questo strumento viene utilizzato per `auto-personalize your email` e risparmia tonnellate di tempo per `pulling information from the People page`.

| Campo dinamico | Esempio di cosa viene visualizzato nell’e-mail |
|---|---|
| `{{company}}` | Adobe |
| `{{company_friendly}}` | Adobe |
| `{{first_name}}` | Keith |
| `{{team_unsubscribe}}` | Se non desideri più ricevere e-mail da noi, fai clic qui |
| `{{friendly_unsubscribe}}` | Stanco di tutte le email? Per favore, fammelo sapere qui |
| `{{my_name}}` | Keith Flynn |
| `{{my_signature}}` | Keith Flynn, Senior Technical Writer - Adobe |
| `{{personal_email}}` | keith@pickyouremail.com |
| `{{title}}` | Scrittore tecnico senior |
| `{{work_website}}` | https://www.adobe.com |

**Aspetti da considerare**:

* Se le informazioni di un contatto non vengono immesse correttamente o non sono presenti nella pagina Persone, non verranno inserite correttamente nel modello.
* La differenza tra `{{company}}` e `{{company_friendly}}` è questo `{{company_friendly}}` rimuoverà qualsiasi titolo formale, come Inc., LLC., ecc., dal nome della società del contatto.
* Quando si utilizza `{{company_friendly}}`, assicurati di separare Inc. o Co. con una virgola nei dettagli di contatto. In questo modo Sales Connect sa cosa rimuovere quando si richiama il valore.
* Se si utilizza `{{my_signature}}` dinamico, il sistema non aggiunge automaticamente la firma dell&#39;utente per evitare duplicati.

>[!TIP]
>
>Puoi crearne uno tuo [campo dinamico personalizzato](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/create-custom-dynamic-fields.md) per tutto ciò che desideri inserire automaticamente nelle e-mail
