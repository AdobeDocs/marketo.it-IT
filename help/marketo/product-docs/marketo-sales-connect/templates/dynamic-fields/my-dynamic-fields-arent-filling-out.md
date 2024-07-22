---
unique-page-id: 14352602
description: I miei campi dinamici non vengono compilati - Documentazione di Marketo - Documentazione del prodotto
title: I miei campi dinamici non vengono compilati
exl-id: fb3e8b56-506a-41f8-a84f-41370381c058
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---

# I miei campi dinamici non vengono compilati {#my-dynamic-fields-arent-filling-out}

I campi dinamici funzionano solo quando si utilizza un modello. Le singole e-mail che scrivi non vengono compilate.

## Cosa verificare {#what-to-check}

In Sales Connect sono disponibili tre tipi di campi dinamici: Basic, Custom e Salesforce. Sia Basic che Custom cercano di richiamare informazioni dall&#39;[applicazione Web](https://toutapp.com/login). Se le informazioni non esistono nell’applicazione web, i campi saranno vuoti. I campi Salesforce richiamano informazioni da [Salesforce.com](https://salesforce.com).

**Risoluzione dei problemi dei campi Salesforce**

Campi Salesforce: esempio: `{{sfdc_account_name}}`

* Assicurati che sia collegato correttamente a Sales Connect. Vai alla pagina [Impostazioni](https://toutapp.com/login) e fai clic su **Gestione** accanto al tuo CRM.

**Risoluzione dei problemi dei campi di base e personalizzati**

Campi di base tout: ad esempio `{{company}}`

Campi personalizzati tout: ad esempio `{{custom_field_favorite_movie}}`

* Per fare riferimento al campo dinamico, è necessario salvare il campo corrispondente per il contatto nella [pagina Persone](https://toutapp.com/next#relationships). Ad esempio, se invii un&#39;e-mail a Mary e utilizzi il campo `{{company}}`, ma il suo record contatto non elenca una società, non saremo in grado di compilarlo.

## Perché La Mia E-Mail È Stata Inviata Senza Popolare Tutti I Campi Dinamici? {#why-did-my-email-send-without-populating-all-dynamic-fields}

Sales Connect impedirà l’invio delle e-mail se non è possibile compilare tutti i campi dinamici nell’e-mail. **Tuttavia**, esistono alcune eccezioni a questa regola. Alcuni campi inviano un valore vuoto oppure, se possibile, lo compilano automaticamente. Di seguito sono elencati questi campi e come reagiranno se non possono essere compilati.

`{{first_name}}` = VUOTO

`{{last_name}}` =VUOTO

`{{title}}` = VUOTO

`{{company}}` = &quot;la tua azienda&quot;

`{{friendly_company}}` = &quot;la tua azienda&quot;

>[!NOTE]
>
>Il campo `{{first_name}}` verrà visualizzato sia in Sales Connect che in Salesforce per tentare di richiamare informazioni. Tutti gli altri campi dell&#39;elenco vengono cercati solo in Sales Connect per compilare il campo.
