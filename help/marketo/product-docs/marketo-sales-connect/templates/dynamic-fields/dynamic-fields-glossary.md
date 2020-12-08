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

Quando si crea un modello in Sales Connect, è sempre consigliabile integrare i campi dinamici utilizzando il pulsante Campi **dinamici** MSE.

Questo strumento è utilizzato per `auto-personalize your email` risparmiare tonnellate di tempo `pulling information from the People page`.

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

* Se un contatto è `information is entered incorrectly` o è mancante nella pagina Persone, lo puoi `will not pull over correctly` inserire nel modello.

* La differenza tra `{{company}}` e `{{company_friendly}}` è che `{{company_friendly}}` sarà `remove any formal title`, come Inc., LLC, ecc., dal nome della società del contatto.
* Quando utilizzi `{{company_friendly}}`, accertati di separare Inc. o Co. con una virgola nei dettagli di contatto. Questo è il modo in cui Sales Connect sa cosa rimuovere quando estrae il valore.

>[!TIP]
>
>Puoi creare un campo [dinamico](http://docs.marketo.com/x/fADb) personalizzato per qualsiasi cosa desideri che sia stato inserito automaticamente nelle e-mail.

