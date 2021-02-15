---
unique-page-id: 14352509
description: Glossario Campi Dinamici - Documenti Marketo - Documentazione prodotto
title: Glossario campi dinamici
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---


# Glossario campi dinamici {#dynamic-fields-glossary}

Durante la creazione di un modello in Sales Connect, si consiglia sempre di integrare i campi dinamici utilizzando il pulsante **Campi dinamici MSE**.

Questo strumento è utilizzato per `auto-personalize your email` e risparmiare tonnellate di tempo per `pulling information from the People page`.

| Campo dinamico | Esempio di ciò che viene visualizzato nel messaggio e-mail |
|---|---|
| `{{company}}` | Marketo |
| `{{company_friendly}}` | Marketo |
| `{{first_name}}` | Keith |
| `{{friendly_unsubscribe}}` | Se non vuoi sentire di nuovo da me, per favore fatemelo sapere qui |
| `{{my_name}}` | Alan Bradley |
| `{{personal_email}}` | keith@pickyouremail.com |
| `{{title}}` | Responsabile tecnico |
| `{{work_website}}` | https://www.marketo.com |

**Elementi da notare**:

* Se le informazioni di un contatto sono inserite in modo errato o mancano nella pagina Persone, non verranno trascinate correttamente nel modello.
* La differenza tra `{{company}}` e `{{company_friendly}}` è che `{{company_friendly}}` rimuoverà dal nome della società del contatto qualsiasi titolo formale, come Inc., LLC, ecc.
* Quando si utilizza `{{company_friendly}}`, assicurarsi di separare Inc. o Co. con una virgola nei dettagli di contatto. Questo è il modo in cui Sales Connect sa cosa rimuovere quando estrae il valore.

>[!TIP]
>
>È possibile creare un proprio [campo dinamico personalizzato](/help/marketo/product-docs/marketo-sales-connect/templates/dynamic-fields/create-custom-dynamic-fields.md) per qualsiasi elemento che si desidera inserire automaticamente nelle e-mail
