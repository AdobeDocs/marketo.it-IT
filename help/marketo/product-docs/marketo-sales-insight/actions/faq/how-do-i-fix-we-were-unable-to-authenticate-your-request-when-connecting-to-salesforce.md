---
description: Come posso risolvere il problema "Impossibile autenticare la richiesta" durante la connessione a Salesforce - Documentazione di Marketo - Documentazione del prodotto
title: Come posso risolvere il problema "Impossibile autenticare la richiesta" durante la connessione a Salesforce?
exl-id: ef876f0f-bd76-4ba5-bf48-885ee048ceae
feature: Sales Insight Actions
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 0%

---

# Come risolvere il problema relativo all&#39;impossibilità di autenticare la richiesta durante la connessione a [!DNL Salesforce] {#how-do-i-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

Se stai tentando di collegare la tua istanza di Marketo Sales a Salesforce e visualizzi l’errore &quot;Non siamo in grado di autenticare la tua richiesta&quot;, è probabile che ciò dipenda dalla configurazione dell’istanza di Salesforce.

La pagina di autenticazione non riuscita può essere generata da due tipi di errori.

* Errore di accesso Dominio con restrizioni
* App Oauth bloccata

Controlla l’URL per identificare il tipo che stai ricevendo.

![](assets/how-do-i-fix-we-were-unable-to-authenticate-1.png)

![](assets/how-do-i-fix-we-were-unable-to-authenticate-2.png)

## Risolvi dominio con restrizioni di errore di accesso {#resolve-login-error-restricted-domain}

Questo errore indica in genere che disponi di un dominio personalizzato a cui non è possibile indirizzare. Per risolvere l&#39;errore, provare ad accedere all&#39;istanza di Salesforce a cui si desidera connettersi per prima. Quindi, segui i passaggi per connetterti a Salesforce.

Se l’istanza a cui stai tentando di connetterti è un dominio Sandbox di Salesforce e ricevi un errore, dovrai eseguire ulteriori passaggi per aggiornare l’istanza in modo che sia compatibile con Salesforce Sandbox. [Ulteriori informazioni](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/set-up-a-sales-insight-actions-sandbox.md){target="_blank"}.

## Risolvi app OAuth bloccata {#resolve-oauth-app-blocked}

Se ricevi il messaggio di errore &quot;Impossibile autenticare la richiesta&quot; con il tipo di errore Oauth App Blocked (o di altro tipo) nell’URL, potrebbe esserci una restrizione nell’accesso all’API di Salesforce. Rivolgiti al tuo amministratore di Salesforce per verificare che i seguenti elementi siano corretti.

### Abilitare l’API nelle autorizzazioni utente {#enable-api-in-user-permissions}

1. Chiedi a un amministratore di Salesforce di accedere a Salesforce.
1. Selezionare **Configurazione**.
1. Selezionare **Gestisci utenti**.
1. Seleziona **Profili**.
1. Trova il profilo in cui si trovano gli utenti ToutApp e fai clic su **Modifica**.
1. Scorri verso il basso fino a **Autorizzazioni amministrative** e assicurati che **API abilitata** sia selezionato.

### Controlla se Salesforce sta bloccando la connessione delle azioni di Sales Insight {#check-if-salesforce-is-blocking-sales-insight-actions-from-connecting}

1. Chiedi a un amministratore di Salesforce di accedere a Salesforce.
1. Selezionare **Configurazione**.
1. Seleziona **Gestisci app**.
1. Seleziona **Utilizzo OAuth app collegate**.
1. Accertati che Azioni Insight vendite sia visualizzato accanto a esso il messaggio &quot;Blocca&quot;. Se viene visualizzato &quot;Sblocca&quot;, fare clic sul pulsante per sbloccare l&#39;accesso delle azioni di Insight Sales a Salesforce.
