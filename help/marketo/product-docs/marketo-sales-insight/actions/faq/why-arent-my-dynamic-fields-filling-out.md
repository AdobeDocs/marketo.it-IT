---
description: Perché i campi dinamici non vengono compilati? - Documentazione di Marketo - Documentazione del prodotto
title: Perché i campi dinamici non vengono compilati?
exl-id: 4e1d133f-8314-4e64-b50b-f3e824c3bef4
feature: Sales Insight Actions
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 0%

---

# Perché i campi dinamici non vengono compilati? {#why-arent-my-dynamic-fields-filling-out}

I campi dinamici funzionano solo quando si utilizza un modello. Le singole e-mail che scrivi non vengono compilate.

## Cosa verificare {#what-to-check}

Nelle azioni di Sales Insight sono disponibili tre tipi di campi dinamici: Base, Personalizzato e Salesforce. Sia Basic che Custom cercano di richiamare informazioni dall&#39;[applicazione Web](https://toutapp.com/login){target="_blank"}. Se le informazioni non esistono nell’applicazione web, i campi saranno vuoti. I campi Salesforce richiamano informazioni da [Salesforce.com](https://salesforce.com){target="_blank"}.

**Risoluzione dei problemi di [!DNL Salesforce] campi**

[!DNL Salesforce] campi: ad esempio `{{sfdc_account_name}}`

* Assicurati che sia collegato correttamente alle azioni di Insight per le vendite. Vai alla pagina [Impostazioni]&#x200B;(<https://toutapp.com/login{target="_blank"}> e fai clic su **Gestione** accanto al tuo CRM.

**Risoluzione dei problemi dei campi di base e personalizzati**

Campi di base delle azioni Insight per le vendite Marketo: ad esempio, `{{company}}`

Campi personalizzati azioni Insight vendite Marketo: ad esempio `{{custom_field_favorite_movie}}`

* Per fare riferimento al campo dinamico, è necessario salvare il campo corrispondente per il contatto nella [pagina Persone](https://toutapp.com/next#relationships){target="_blank"}. Ad esempio, se invii un&#39;e-mail a Mary e utilizzi il campo `{{company}}`, ma il suo record contatto non elenca una società, non saremo in grado di compilarlo.

## Perché La Mia E-Mail È Stata Inviata Senza Popolare Tutti I Campi Dinamici? {#why-did-my-email-send-without-populating-all-dynamic-fields}

[!DNL Sales Insight Actions] interromperà l&#39;invio delle e-mail se non è possibile compilare tutti i campi dinamici nell&#39;e-mail. **Tuttavia**, esistono alcune eccezioni a questa regola. Alcuni campi inviano un valore vuoto oppure, se possibile, lo compilano automaticamente. Di seguito sono elencati questi campi e come reagiranno se non possono essere compilati.

`{{first_name}}` = VUOTO

`{{last_name}}` =VUOTO

`{{title}}` = VUOTO

`{{company}}` = &quot;la tua azienda&quot;

`{{friendly_company}}` = &quot;la tua azienda&quot;

>[!NOTE]
>
>Il campo `{{first_name}}` verrà cercato sia in [!DNL Sales Insight Actions] che in [!DNL Salesforce] per tentare di estrarre informazioni. Tutti gli altri campi di questo elenco cercano solo in [!DNL Sales Insight Actions] per compilare il campo.
