---
unique-page-id: 14352509
description: Glossario Campi Dinamici - Documenti Marketo - Documentazione prodotto
title: Glossario campi dinamici
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '173'
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
| `{{personal_email}}` | [[email protected]](http://docs.marketo.com/cdn-cgi/l/email-protection) |
| `{{title}}` | Responsabile tecnico |
| `{{work_website}}` | https://www.marketo.com |

**Elementi da notare**:

* Se un contatto è `information is entered incorrectly` o è mancante nella pagina Persone, `will not pull over correctly` nel modello.

* La differenza tra `{{company}}` e `{{company_friendly}}` è che `{{company_friendly}}` `remove any formal title`, come Inc., LLC, ecc., dal nome della società del contatto.
* Quando si utilizza `{{company_friendly}}`, assicurarsi di separare Inc. o Co. con una virgola nei dettagli di contatto. Questo è il modo in cui Sales Connect sa cosa rimuovere quando estrae il valore.

>[!TIP]
>
>È possibile creare un proprio [campo dinamico personalizzato](http://docs.marketo.com/x/fADb) per qualsiasi elemento che si desidera inserire automaticamente nelle e-mail

