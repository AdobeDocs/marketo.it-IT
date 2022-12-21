---
description: Perché i miei campi dinamici non si riempiono - Marketo Docs - Documentazione del prodotto
title: Perché i miei campi dinamici non si riempiono
hide: true
hidefromtoc: true
exl-id: 4e1d133f-8314-4e64-b50b-f3e824c3bef4
source-git-commit: f77a076c243c25f3bff98a82751f51c464712795
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 0%

---

# Perché i miei campi dinamici non si riempiono {#why-arent-my-dynamic-fields-filling-out}

I campi dinamici funzionano solo quando utilizzi un modello. Le singole e-mail una tantum che scrivi non vengono compilate.

## Cosa controllare {#what-to-check}

Esistono tre tipi di campi dinamici nelle azioni Approfondimenti vendite: Base, Personalizzato e Salesforce. Base e Personalizzato entrambi cercano di estrarre le informazioni dal [applicazione web](https://toutapp.com/login). Se le informazioni non esistono nell’applicazione Web, i campi saranno vuoti. I campi Salesforce richiamano informazioni da [Salesforce.com](https://salesforce.com).

**Risoluzione dei problemi dei campi Salesforce**

Campi Salesforce: ad esempio `{{sfdc_account_name}}`

* Assicurati che sia collegato correttamente alle azioni di Insight sulle vendite. Vai a [Impostazioni](https://toutapp.com/login) e fai clic su **Gestisci** accanto al tuo CRM.

**Risoluzione dei problemi relativi ai campi di base e personalizzati**

Campi di base del timeout: ad esempio `{{company}}`

Campi personalizzati del timeout: ad esempio `{{custom_field_favorite_movie}}`

* Il campo corrispondente deve essere salvato per il contatto nel [Pagina Persone](https://toutapp.com/next#relationships) per fare riferimento al nostro campo dinamico. Ad esempio, se invii un’e-mail a Mary e utilizzi il `{{company}}` ma il suo record di contatto non elenca un&#39;azienda, non saremo in grado di compilarlo.

## Perché Il Mio Messaggio E-Mail È Stato Inviato Senza Popolare Tutti I Campi Dinamici? {#why-did-my-email-send-without-populating-all-dynamic-fields}

Se non riusciamo a compilare tutti i campi dinamici dell’e-mail, le azioni Approfondimenti vendite impediranno l’invio delle e-mail. **Tuttavia**, ci sono alcune eccezioni a questa regola. Alcuni campi invieranno un valore vuoto oppure compileranno automaticamente un valore se disponibile. Di seguito sono elencati questi campi e le relative reazioni se non sono in grado di compilare il campo.

`{{first_name}}` = VUOTO

`{{last_name}}` =VUOTO

`{{title}}` = VUOTO

`{{company}}` = &quot;azienda&quot;

`{{friendly_company}}` = &quot;azienda&quot;

>[!NOTE]
>
>La `{{first_name}}` Per cercare di estrarre informazioni, consulta le azioni Approfondimenti vendite e Salesforce . Tutti gli altri campi di questo elenco sono visualizzati solo in Azioni Approfondimenti vendite per compilare il campo.
