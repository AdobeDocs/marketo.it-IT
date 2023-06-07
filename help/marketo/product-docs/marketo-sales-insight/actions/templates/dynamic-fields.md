---
description: Campi dinamici - Documentazione di Marketo - Documentazione del prodotto
title: Campi dinamici
exl-id: d9e52eae-d5bb-462f-8b7b-c28a560f6ea4
source-git-commit: 466df1fbd561860152f9fea02edb6eab5670c90a
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 0%

---

# Campi dinamici {#dynamic-fields}

Ti consentiamo di personalizzare i modelli e-mail con attributi predefiniti come `{{first_name}}` o `{{company}}`. Questi campi ti consentono di inviare tramite e-mail più contatti e di completarli automaticamente senza doverli digitare separatamente per ciascun contatto.

>[!TIP]
>
>Il campo &quot;first_name&quot; e &quot;company&quot; sono gli unici campi che verranno visualizzati sia in Sales Insight Actions che in Salesforce. Ciò significa che se un contatto non esiste in [applicazione web](https://toutapp.com/login), analizziamo Salesforce per verificare se è possibile trovare un record contatto/lead con un indirizzo e-mail corrispondente. Quindi utilizziamo le informazioni di quel record per compilare il campo.

## Inserire un campo dinamico in un modello {#insert-a-dynamic-field-into-a-template}

1. In entrata **Modelli e campagne**, individua il modello da modificare e fai clic su **Modifica modello**.

1. Clic **Inserisci campo dinamico**.

   >[!NOTE]
   >
   >Quando si inviano messaggi di posta elettronica a contatti esistenti in Azioni approfondimenti vendite, è possibile utilizzare i campi dinamici di base. Questi richiameranno direttamente dal contatto.

Se invii messaggi di posta elettronica a contatti esistenti in Salesforce, puoi sfruttare i campi dinamici di Salesforce. Questi iniziano tutti con &quot;sfdc&quot;. Se disponi di una connessione a Salesforce, questi campi richiameranno direttamente il lead/contatto in Salesforce per compilare le informazioni nel modello.

## Inserire campi dinamici in un oggetto {#insert-dynamic-fields-in-a-subject-line}

È sufficiente copiarli e incollarli manualmente nel campo dell’oggetto di un’e-mail, assicurandosi di disporre della formattazione corretta.

## Valori predefiniti campo dinamico {#dynamic-field-default-values}

Quando aggiungi campi dinamici ai modelli e-mail, puoi aggiungere un valore predefinito che il campo dinamico risolverà se non è disponibile alcun altro valore.

A questo scopo, aggiungi &quot;|&quot; dopo l’etichetta del campo dinamico, quindi aggiungi &quot;default:&quot;. Quindi, aggiungi il valore in cui vuoi risolvere il campo, se non è possibile trovare un altro valore.

**Esempio:**

`{{first name | default: loyal customer}}`

`{{sfdc_contact_account_name | default: your company}}`

## Glossario dei campi dinamici {#dynamic-fields-glossary}

Durante la creazione di un modello in Azioni approfondimento vendite, si consiglia sempre di integrare i campi dinamici utilizzando **Inserisci campo dinamico** pulsante.

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
* Quando si utilizza `{{company_friendly}}`, assicurati di separare Inc. o Co. con una virgola nei dettagli di contatto. In questo modo le azioni di approfondimento sulle vendite sanno cosa rimuovere quando si richiama il valore.
* Ti consentiamo di personalizzare i modelli e-mail con attributi predefiniti come `{{my_name}}` o `{{my_title}}`. Questi campi ti consentono di fare rapidamente riferimento a te stesso nei tuoi modelli e-mail.

>[!TIP]
>
>Se i campi dinamici non vengono compilati, estrarre [questo articolo](/help/marketo/product-docs/marketo-sales-insight/actions/faq/why-arent-my-dynamic-fields-filling-out.md).
