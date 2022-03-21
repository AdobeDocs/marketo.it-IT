---
description: Campi dinamici - Documenti Marketo - Documentazione del prodotto
title: Campi dinamici
hide: true
hidefromtoc: true
source-git-commit: a0b10255513c13b7100b667513e3e61fc3788a15
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 0%

---

# Campi dinamici {#dynamic-fields}

Ti consente di personalizzare i modelli e-mail con attributi predefiniti, come `{{first_name}}` o `{{company}}`. Questi campi ti consentono di inviare e-mail a più contatti e completare automaticamente questi campi senza doverli digitare separatamente per ogni contatto.

>[!TIP]
>
>I campi &quot;first_name&quot; e &quot;company&quot; sono gli unici campi che verranno visualizzati sia nelle azioni Insight vendite che in Salesforce. Ciò significa che se un contatto non esiste nel [applicazione web](https://toutapp.com/login), in Salesforce verifichiamo se è possibile trovare un record contatto/lead con un indirizzo e-mail corrispondente. Quindi utilizziamo le informazioni di quel record per compilare il campo.

## Inserire un campo dinamico in un modello {#insert-a-dynamic-field-into-a-template}

1. In **Modelli e campagne**, trova il modello da modificare e fai clic su **Modifica modello**.

1. Fai clic su **Inserisci campo dinamico**.

   >[!NOTE]
   >
   >Quando invii tramite e-mail contatti esistenti in Azioni Approfondimenti vendite, puoi utilizzare i campi dinamici di base. Questi tireranno direttamente dal contatto.

Se invii tramite e-mail contatti esistenti in Salesforce, puoi sfruttare i campi dinamici Salesforce. Tutto inizia con &quot;sfdc&quot;. Se si dispone di una connessione a Salesforce, questi campi richiameranno direttamente al lead/contatto di Salesforce per compilare le informazioni nel modello.

## Inserire campi dinamici in una riga oggetto {#insert-dynamic-fields-in-a-subject-line}

È sufficiente copiarli e incollarli manualmente nel campo oggetto di un’e-mail, avendo cura di disporre della formattazione corretta.

## Glossario dei campi dinamici {#dynamic-fields-glossary}

Quando crei un modello in Azioni di Insight vendite, è sempre consigliabile integrare i campi dinamici utilizzando **Inserisci campo dinamico** pulsante .

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
* Quando utilizzi `{{company_friendly}}`, assicurati di separare Inc. o Co. con una virgola nei dettagli del contatto. Questo è il modo in cui le azioni Insight sulle vendite sanno cosa rimuovere quando si estrae il valore.
* Ti consente di personalizzare i modelli e-mail con attributi predefiniti, come `{{my_name}}` o `{{my_title}}`. Questi campi ti consentono di fare rapidamente riferimento a te stesso nei tuoi modelli e-mail.

>[!TIP]
>
>Se i campi dinamici non si popolano, estrarre [articolo](/help/marketo/product-docs/marketo-sales-insight/actions/faq/why-arent-my-dynamic-fields-filling-out.md).
