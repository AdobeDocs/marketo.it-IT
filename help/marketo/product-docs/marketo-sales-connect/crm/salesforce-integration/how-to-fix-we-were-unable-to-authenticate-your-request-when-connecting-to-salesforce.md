---
unique-page-id: 14352484
description: Come risolvere "Non siamo stati in grado di autenticare la tua richiesta" quando ci si collega a Salesforce - Marketo Docs - Documentazione del prodotto
title: Come risolvere "Impossibile autenticare la richiesta" durante la connessione a Salesforce
translation-type: tm+mt
source-git-commit: 1dd80b7de801df78ac7dde39002455063f9979b7
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 0%

---


# Come risolvere &quot;Impossibile autenticare la richiesta&quot; durante la connessione a Salesforce {#how-to-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

Se durante il tentativo di connettere Sales Connect a Salesforce ricevi il messaggio di errore &quot;Impossibile autenticare la richiesta&quot;, potrebbe verificarsi una limitazione all&#39;accesso all&#39;API di Salesforce. Consulta il tuo amministratore Salesforce per verificare che siano già stati installati i seguenti elementi.

## Abilita API nelle autorizzazioni utente {#enable-api-in-user-permissions}

1. Accedi a un amministratore Salesforce in SFDC.
1. Selezionare **Setup**.
1. Selezionare **Gestisci utenti**.
1. Selezionare **Profili**.
1. Individua il profilo in cui si trovano gli utenti ToutApp e fai clic su **Modifica**.
1. Scorrete verso il basso fino a **Autorizzazioni amministrative** e accertatevi che l&#39;opzione **API abilitata** sia selezionata.

## Verifica se Salesforce sta bloccando la connessione delle vendite {#check-if-salesforce-is-blocking-sales-connect-from-connecting}

1. Accedi a Salesforce Admin da SFDC.
1. Selezionare **Setup**.
1. Selezionare **Gestisci app**.
1. Selezionare **Applicazioni collegate OAuth Usage**.
1. Verificate che il Sales Connect mostri &quot;Blocca&quot; accanto ad esso. Se viene visualizzato &quot;Sblocca&quot;, fate clic sul pulsante per sbloccare l&#39;accesso di Sales Connect a Salesforce.
