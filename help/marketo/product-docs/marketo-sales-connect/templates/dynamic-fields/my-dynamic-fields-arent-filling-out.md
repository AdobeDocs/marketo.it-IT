---
unique-page-id: 14352602
description: I miei campi dinamici non stanno riempiendo - Documenti Marketo - Documentazione prodotto
title: I miei campi dinamici non si stanno compilando
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---


# I miei campi dinamici non si stanno compilando {#my-dynamic-fields-arent-filling-out}

I campi dinamici funzionano solo se si utilizza un modello. Le singole e-mail una tantum che scrivete non le compileranno.

## Cosa controllare {#what-to-check}

In Sales Connect sono disponibili tre tipi di campi dinamici: Base, Personalizzato e Salesforce. L&#39;aspetto di base e personalizzato consente di estrarre informazioni dall&#39;applicazione [](http://toutapp.com/login)Web. Se le informazioni non esistono nell&#39;applicazione Web, i campi saranno vuoti. I campi Salesforce richiamano informazioni da [Salesforce.com](http://salesforce.com).

`**Troubleshooting Salesforce Fields**`

Campi Salesforce: ad esempio `{{sfdc_account_name}}`

* Assicurati che sia collegato correttamente a Sales Connect. Vai alla pagina [Impostazioni](http://toutapp.com/next#settings) e fai clic su **Gestisci** accanto a CRM.

**Risoluzione dei problemi relativi ai campi di base e personalizzati**

Campi di base Tout: ad esempio `{{company}}`

Campi personalizzati Tout: ad esempio `{{custom_field_favorite_movie}}`

* Nella `he corresponding field needs to be saved for your contact` pagina [](http://toutapp.com/next#relationships) Persone fare riferimento al nostro campo dinamico. Ad esempio, se invii un&#39;e-mail a Mary e utilizzi il `{{company}}` campo, ma il suo record di contatto non elenca una società, non saremo in grado di compilarlo.

## Perché La Mia E-Mail È Stata Inviata Senza Compilare Tutti I Campi Dinamici? {#why-did-my-email-send-without-populating-all-dynamic-fields}

Se non riusciamo a compilare tutti i campi dinamici dell&#39;e-mail, i messaggi e-mail verranno interrotti. **Tuttavia**, ci sono alcune eccezioni a questa regola. Alcuni campi invieranno vuoti o compileranno automaticamente un valore se ne troverà uno. Questi campi e come reagiranno se non saranno in grado di compilare il campo sono elencati di seguito.

`{{first_name}}` = VUOTO

`{{last_name}}` =VUOTO

`{{title}}` = VUOTO

`{{company}}` = &quot;azienda&quot;

`{{friendly_company}}` = &quot;azienda&quot;

>[!NOTE]
>
>Il `{{first_name}}` campo verrà visualizzato sia in Sales Connect che in Salesforce per tentare di richiamare le informazioni. Tutti gli altri campi di questo elenco sono visualizzati solo in Sales Connect per compilare il campo.

