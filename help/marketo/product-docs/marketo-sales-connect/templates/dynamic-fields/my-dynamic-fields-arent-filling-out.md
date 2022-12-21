---
unique-page-id: 14352602
description: I miei campi dinamici non si stanno compilando - Documenti Marketo - Documentazione del prodotto
title: I miei campi dinamici non si stanno compilando
exl-id: fb3e8b56-506a-41f8-a84f-41370381c058
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 0%

---

# I miei campi dinamici non si stanno compilando {#my-dynamic-fields-arent-filling-out}

I campi dinamici funzionano solo quando utilizzi un modello. Le singole e-mail una tantum che scrivi non vengono compilate.

## Cosa controllare {#what-to-check}

In Sales Connect sono disponibili tre tipi di campi dinamici: Base, Personalizzato e Salesforce. Base e Personalizzato entrambi cercano di estrarre le informazioni dal [applicazione web](https://toutapp.com/login). Se le informazioni non esistono nell’applicazione Web, i campi saranno vuoti. I campi Salesforce richiamano informazioni da [Salesforce.com](https://salesforce.com).

**Risoluzione dei problemi dei campi Salesforce**

Campi Salesforce: ad esempio `{{sfdc_account_name}}`

* Assicurati che sia collegato correttamente a Sales Connect. Vai a [Impostazioni](https://toutapp.com/login) e fai clic su **Gestisci** accanto al tuo CRM.

**Risoluzione dei problemi relativi ai campi di base e personalizzati**

Campi di base del timeout: ad esempio `{{company}}`

Campi personalizzati del timeout: ad esempio `{{custom_field_favorite_movie}}`

* Il campo corrispondente deve essere salvato per il contatto nel [Pagina Persone](https://toutapp.com/next#relationships) per fare riferimento al nostro campo dinamico. Ad esempio, se invii un’e-mail a Mary e utilizzi il `{{company}}` ma il suo record di contatto non elenca un&#39;azienda, non saremo in grado di compilarlo.

## Perché Il Mio Messaggio E-Mail È Stato Inviato Senza Popolare Tutti I Campi Dinamici? {#why-did-my-email-send-without-populating-all-dynamic-fields}

Se non è possibile compilare tutti i campi dinamici dell&#39;e-mail, le e-mail verranno inviate automaticamente. **Tuttavia**, ci sono alcune eccezioni a questa regola. Alcuni campi invieranno un valore vuoto oppure compileranno automaticamente un valore se disponibile. Di seguito sono elencati questi campi e le relative reazioni se non sono in grado di compilare il campo.

`{{first_name}}` = VUOTO

`{{last_name}}` =VUOTO

`{{title}}` = VUOTO

`{{company}}` = &quot;azienda&quot;

`{{friendly_company}}` = &quot;azienda&quot;

>[!NOTE]
>
>La `{{first_name}}` Per cercare di estrarre informazioni, cerca sia Sales Connect che Salesforce. Tutti gli altri campi di questo elenco sono visualizzati solo in Connetti vendite per compilare il campo.
