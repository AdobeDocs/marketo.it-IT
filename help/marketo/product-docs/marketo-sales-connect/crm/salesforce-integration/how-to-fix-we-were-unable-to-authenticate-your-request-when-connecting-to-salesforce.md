---
unique-page-id: 14352484
description: Come risolvere il problema "Impossibile autenticare la richiesta" quando si collega a Salesforce - Marketo Docs - Documentazione del prodotto
title: Come risolvere "Impossibile autenticare la richiesta" durante la connessione a Salesforce
exl-id: ddd49064-f584-4490-8d45-29cf61ed3ebe
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 0%

---

# Come risolvere &quot;Impossibile autenticare la richiesta&quot; durante la connessione a Salesforce {#how-to-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

Se ricevi il messaggio di errore &quot;Impossibile autenticare la richiesta&quot; durante il tentativo di collegare Sales Connect a Salesforce, potrebbe esserci una restrizione all&#39;accesso all&#39;API di Salesforce. Controlla con il tuo amministratore Salesforce per assicurarti che siano presenti le seguenti funzioni.

## Abilitare API nelle autorizzazioni utente {#enable-api-in-user-permissions}

1. Avere un accesso amministratore Salesforce in SFDC.
1. Seleziona **Configurazione**.
1. Seleziona **Gestione utenti**.
1. Seleziona **Profili**.
1. Trova il profilo in cui si trovano gli utenti di ToutApp e fai clic su **Modifica**.
1. Scorri verso il basso fino a **Autorizzazioni amministrative** e assicurati **API abilitata** è controllata.

## Controlla se Salesforce sta bloccando la connessione delle vendite {#check-if-salesforce-is-blocking-sales-connect-from-connecting}

1. Disporre di un accesso Admin Salesforce a SFDC.
1. Seleziona **Configurazione**.
1. Seleziona **Gestione app**.
1. Seleziona **Utilizzo OAuth delle app collegate**.
1. Assicurati che Sales Connect mostri &quot;Block&quot; accanto ad esso. Se vedi &quot;Sblocca&quot;, fai clic sul pulsante per sbloccare l&#39;accesso di Sales Connect a Salesforce.
