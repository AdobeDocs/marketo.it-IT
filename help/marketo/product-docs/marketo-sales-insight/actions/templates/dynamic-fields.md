---
description: Campi dinamici - Documentazione di Marketo - Documentazione del prodotto
title: Campi dinamici
exl-id: d9e52eae-d5bb-462f-8b7b-c28a560f6ea4
feature: Sales Insight Actions
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '527'
ht-degree: 0%

---

# Campi dinamici {#dynamic-fields}

È possibile personalizzare i modelli e-mail con attributi predefiniti come `{{first_name}}` o `{{company}}`. Questi campi ti consentono di inviare tramite e-mail più contatti e di completarli automaticamente senza doverli digitare separatamente per ciascun contatto.

>[!TIP]
>
>Il campo &quot;first_name&quot; e &quot;company&quot; sono gli unici campi che verranno cercati sia in [!DNL Sales Insight Actions] che in [!DNL Salesforce]. Ciò significa che se un contatto non esiste nell&#39;applicazione Web [](https://toutapp.com/login), verrà eseguita una ricerca in [!DNL Salesforce] per verificare se è possibile trovare un record contatto/lead con un indirizzo e-mail corrispondente. Quindi utilizziamo le informazioni di quel record per compilare il campo.

## Inserire un campo dinamico in un modello {#insert-a-dynamic-field-into-a-template}

1. In **[!UICONTROL Templates & Campaigns]**, trovare il modello da modificare e fare clic su **[!UICONTROL Edit Template]**.

1. Fai clic su **[!UICONTROL Insert Dynamic Field]**.

   >[!NOTE]
   >
   >Quando si inviano messaggi di posta elettronica a contatti esistenti in [!DNL Sales Insight Actions], è possibile utilizzare i campi dinamici di base. Questi richiameranno direttamente dal contatto.

Se invii messaggi di posta elettronica a contatti esistenti in [!DNL Salesforce], puoi sfruttare i campi dinamici [!DNL Salesforce]. Questi iniziano tutti con &quot;sfdc&quot;. Se si dispone di una connessione a [!DNL Salesforce], questi campi chiameranno direttamente il lead/contatto in [!DNL Salesforce] per compilare le informazioni nel modello.

## Inserire campi dinamici in un oggetto {#insert-dynamic-fields-in-a-subject-line}

È sufficiente copiarli e incollarli manualmente nel campo dell’oggetto di un’e-mail, assicurandosi di disporre della formattazione corretta.

## Valori predefiniti campo dinamico {#dynamic-field-default-values}

Quando aggiungi campi dinamici ai modelli e-mail, puoi aggiungere un valore predefinito che il campo dinamico risolverà se non è disponibile alcun altro valore.

A questo scopo, aggiungi &quot;|&quot; dopo l’etichetta del campo dinamico, quindi aggiungi &quot;default:&quot; (entrambi senza virgolette). Quindi, aggiungi il valore a cui vuoi risolvere il campo (racchiuso tra virgolette) se non è possibile trovare altri valori.

**Esempio:**

`{{first name | default: "loyal customer"}}`

`{{sfdc_contact_account_name | default: "your company"}}`

## Glossario dei campi dinamici {#dynamic-fields-glossary}

Durante la creazione di un modello in [!DNL Sales Insight Actions], si consiglia sempre di integrare i campi dinamici mediante il pulsante **[!UICONTROL Insert Dynamic Field]**.

Questo strumento viene utilizzato per `auto-personalize your email` e consente di risparmiare tonnellate di tempo entro `pulling information from the People page`.

| Campo dinamico | Esempio di cosa viene visualizzato nell’e-mail |
|---|---|
| `{{company}}` | Adobe |
| `{{company_friendly}}` | Adobe |
| `{{first_name}}` | Keith |
| `{{team_unsubscribe}}` | Se non desideri più ricevere e-mail da noi, fai clic qui |
| `{{friendly_unsubscribe}}` | Stanco di tutte le email? Per favore, fammelo sapere qui |
| `{{my_name}}` | Keith Flynn |
| `{{my_signature}}` | Keith Flynn, Senior Technical Writer di Adobe |
| `{{personal_email}}` | keith@pickyouremail.com |
| `{{title}}` | Scrittore tecnico senior |
| `{{work_website}}` | https://www.adobe.com |

**Aspetti da considerare**:

* Se le informazioni di un contatto non vengono immesse correttamente o non sono presenti nella pagina Persone, non verranno inserite correttamente nel modello.
* La differenza tra `{{company}}` e `{{company_friendly}}` è che `{{company_friendly}}` rimuoverà qualsiasi titolo formale, ad esempio Inc., LLC., ecc., dal nome della società del contatto.
* Quando utilizzi `{{company_friendly}}`, assicurati di separare Inc. o Co. con una virgola nei dettagli di contatto. [!DNL Sales Insight Actions] è in grado di sapere cosa rimuovere durante l&#39;estrazione del valore.
* È possibile personalizzare i modelli e-mail con attributi predefiniti come `{{my_name}}` o `{{my_title}}`. Questi campi ti consentono di fare rapidamente riferimento a te stesso nei tuoi modelli e-mail.
* Il sistema aggiunge automaticamente la firma dell&#39;utente a ogni e-mail inviata. Se l&#39;utente utilizza un modello con il campo dinamico `{{my_signature}}`, il sistema compilerà la firma in cui è stato inserito il campo dinamico `{{my_signature}}`. Viene aggiunto solo per evitare duplicazioni. Il sistema gestirà `{{team_unsubscribe}}` nello stesso modo quando è abilitata l&#39;impostazione globale per l&#39;annullamento dell&#39;abbonamento.

>[!TIP]
>
>Se i campi dinamici non vengono compilati, vedi [questo articolo](/help/marketo/product-docs/marketo-sales-insight/actions/faq/why-arent-my-dynamic-fields-filling-out.md).
