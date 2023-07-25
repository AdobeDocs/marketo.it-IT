---
unique-page-id: 14352509
description: Glossario dei campi dinamici - Documentazione di Marketo - Documentazione del prodotto
title: Glossario dei campi dinamici
exl-id: 28351ba9-53da-4408-9526-918200d9bd29
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---

# Glossario dei campi dinamici {#dynamic-fields-glossary}

Durante la creazione di un modello in Sales Connect, è sempre consigliabile integrare i campi dinamici utilizzando **Campi dinamici MSE** pulsante.

Questo strumento viene utilizzato per `auto-personalize your email` e risparmia tonnellate di tempo per `pulling information from the People page`.

| Campo dinamico | Esempio di cosa viene visualizzato nell’e-mail |
|---|---|
| `{{company}}` | Marketo |
| `{{company_friendly}}` | Marketo |
| `{{first_name}}` | Keith |
| `{{friendly_unsubscribe}}` | Se non vuoi più sentirmi dire qualcosa, fammelo sapere |
| `{{my_name}}` | Alan Bradley |
| `{{personal_email}}` | keith@pickyouremail.com |
| `{{title}}` | Scrittore tecnico senior |
| `{{work_website}}` | https://www.marketo.com |

**Aspetti da considerare**:

* Se le informazioni di un contatto non vengono immesse correttamente o non sono presenti nella pagina Persone, non verranno inserite correttamente nel modello.
* La differenza tra `{{company}}` e `{{company_friendly}}` è questo `{{company_friendly}}` rimuoverà qualsiasi titolo formale, come Inc., LLC., ecc., dal nome della società del contatto.
* Quando si utilizza `{{company_friendly}}`, assicurati di separare Inc. o Co. con una virgola nei dettagli di contatto. In questo modo Sales Connect sa cosa rimuovere quando si richiama il valore.

>[!TIP]
>
>Puoi crearne uno tuo [campo dinamico personalizzato](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/create-custom-dynamic-fields.md) per tutto ciò che desideri inserire automaticamente nelle e-mail
