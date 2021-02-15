---
unique-page-id: 14352602
description: I miei campi dinamici non stanno riempiendo - Documenti Marketo - Documentazione prodotto
title: I miei campi dinamici non si stanno compilando
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 0%

---


# I campi dinamici non vengono compilati {#my-dynamic-fields-arent-filling-out}

I campi dinamici funzionano solo se si utilizza un modello. Le singole e-mail una tantum che scrivete non le compileranno.

## Cosa controllare {#what-to-check}

In Sales Connect sono disponibili tre tipi di campi dinamici: Base, Personalizzato e Salesforce. Base e Personalizzato entrambi aspetto per ottenere informazioni dall&#39;applicazione Web [](https://toutapp.com/login). Se le informazioni non esistono nell&#39;applicazione Web, i campi saranno vuoti. I campi Salesforce richiamano informazioni da [Salesforce.com](https://salesforce.com).

**Risoluzione dei problemi dei campi Salesforce**

Campi Salesforce: ad esempio `{{sfdc_account_name}}`

* Assicurati che sia collegato correttamente a Sales Connect. Andate alla pagina [Settings](https://toutapp.com/login) e fate clic su **Manage** accanto al CRM.

**Risoluzione dei problemi relativi ai campi di base e personalizzati**

Campi di base Tout: ad esempio `{{company}}`

Campi personalizzati Tout: ad esempio `{{custom_field_favorite_movie}}`

* Per fare riferimento al campo dinamico, è necessario salvare il campo corrispondente per il contatto nella [Pagina Persone](https://toutapp.com/next#relationships). Ad esempio, se invii un&#39;e-mail a Mary e utilizzi il campo `{{company}}`, ma il suo record di contatto non elenca una società, non saremo in grado di compilarlo.

## Perché La Mia E-Mail È Stata Inviata Senza Compilare Tutti I Campi Dinamici? {#why-did-my-email-send-without-populating-all-dynamic-fields}

Se non riusciamo a compilare tutti i campi dinamici dell&#39;e-mail, i messaggi e-mail verranno interrotti. **Tuttavia**, ci sono alcune eccezioni a questa regola. Alcuni campi invieranno vuoti o compileranno automaticamente un valore se ne troverà uno. Questi campi e come reagiranno se non saranno in grado di compilare il campo sono elencati di seguito.

`{{first_name}}` = VUOTO

`{{last_name}}` =VUOTO

`{{title}}` = VUOTO

`{{company}}` = &quot;azienda&quot;

`{{friendly_company}}` = &quot;azienda&quot;

>[!NOTE]
>
>Il campo `{{first_name}}` sarà visualizzato sia in Sales Connect che in Salesforce per tentare di richiamare le informazioni. Tutti gli altri campi di questo elenco sono visualizzati solo in Sales Connect per compilare il campo.
