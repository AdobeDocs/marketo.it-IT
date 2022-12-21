---
unique-page-id: 14352509
description: Glossario dei campi dinamici - Documenti Marketo - Documentazione del prodotto
title: Glossario dei campi dinamici
exl-id: 28351ba9-53da-4408-9526-918200d9bd29
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---

# Glossario dei campi dinamici {#dynamic-fields-glossary}

Durante la creazione di un modello in Sales Connect, si consiglia sempre di integrare i campi dinamici, utilizzando **Campi dinamici MSE** pulsante .

Questo strumento viene utilizzato per `auto-personalize your email` e risparmiare tonnellate di tempo `pulling information from the People page`.

| Campo dinamico | Esempio di ciò che viene visualizzato nel messaggio e-mail |
|---|---|
| `{{company}}` | Marketo |
| `{{company_friendly}}` | Marketo |
| `{{first_name}}` | Keith |
| `{{friendly_unsubscribe}}` | Se non vuoi più sentire la mia voce, fammelo sapere qui |
| `{{my_name}}` | Alan Bradley |
| `{{personal_email}}` | keith@pickyouremail.com |
| `{{title}}` | Redattore tecnico senior |
| `{{work_website}}` | https://www.marketo.com |

**Cose da notare**:

* Se le informazioni di un contatto vengono inserite in modo errato o sono mancanti dalla pagina Persone, non verranno trascinate correttamente nel modello.
* La differenza tra `{{company}}` e `{{company_friendly}}` è `{{company_friendly}}` rimuoverà qualsiasi titolo formale, come Inc., LLC, ecc., dal nome dell&#39;azienda del contatto.
* Quando utilizzi `{{company_friendly}}`, assicurati di separare Inc. o Co. con una virgola nei dettagli del contatto. Questo è il modo in cui Sales Connect sa cosa rimuovere quando si estrae il valore.

>[!TIP]
>
>Puoi crearne uno personalizzato [campo dinamico personalizzato](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/create-custom-dynamic-fields.md) per tutto ciò che vorresti fosse inserito automaticamente nelle tue e-mail
