---
description: Perché i campi dinamici non vengono compilati? - Documentazione di Marketo - Documentazione del prodotto
title: Perché i campi dinamici non vengono compilati?
exl-id: 4e1d133f-8314-4e64-b50b-f3e824c3bef4
feature: Sales Insight Actions
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---

# Perché i campi dinamici non vengono compilati? {#why-arent-my-dynamic-fields-filling-out}

I campi dinamici funzionano solo quando si utilizza un modello. Le singole e-mail che scrivi non vengono compilate.

## Cosa verificare {#what-to-check}

Nelle azioni Sales Insight sono disponibili tre tipi di campi dinamici: Base, Personalizzato e Salesforce. Sia Basic che Custom cercano di richiamare informazioni dall&#39;[applicazione Web](https://toutapp.com/login){target="_blank"}. Se le informazioni non esistono nell’applicazione web, i campi saranno vuoti. I campi Salesforce richiamano informazioni da [Salesforce.com](https://salesforce.com){target="_blank"}.

**Risoluzione dei problemi dei campi Salesforce**

Campi Salesforce: esempio: `{{sfdc_account_name}}`

* Assicurati che sia correttamente collegato alle Azioni di approfondimento sulle vendite. Vai alla pagina [Impostazioni](https://toutapp.com/login{target="_blank"}) e fai clic su **Gestisci** accanto al tuo CRM.

**Risoluzione dei problemi dei campi di base e personalizzati**

Campi di base delle azioni di Marketo Sales Insight: ad esempio, `{{company}}`

Campi personalizzati azioni approfondimento vendite Marketo: ad esempio `{{custom_field_favorite_movie}}`

* Per fare riferimento al campo dinamico, è necessario salvare il campo corrispondente per il contatto nella [pagina Persone](https://toutapp.com/next#relationships){target="_blank"}. Ad esempio, se invii un&#39;e-mail a Mary e utilizzi il campo `{{company}}`, ma il suo record contatto non elenca una società, non saremo in grado di compilarlo.

## Perché La Mia E-Mail È Stata Inviata Senza Popolare Tutti I Campi Dinamici? {#why-did-my-email-send-without-populating-all-dynamic-fields}

Le azioni di approfondimento sulle vendite impediscono l’invio delle e-mail se non è possibile compilare tutti i campi dinamici nell’e-mail. **Tuttavia**, esistono alcune eccezioni a questa regola. Alcuni campi inviano un valore vuoto oppure, se possibile, lo compilano automaticamente. Di seguito sono elencati questi campi e come reagiranno se non possono essere compilati.

`{{first_name}}` = VUOTO

`{{last_name}}` =VUOTO

`{{title}}` = VUOTO

`{{company}}` = &quot;la tua azienda&quot;

`{{friendly_company}}` = &quot;la tua azienda&quot;

>[!NOTE]
>
>Il campo `{{first_name}}` verrà cercato sia in Sales Insight Actions che in Salesforce per tentare di richiamare informazioni. Tutti gli altri campi di questo elenco vengono cercati solo in Azioni approfondimenti vendite per compilare il campo.
