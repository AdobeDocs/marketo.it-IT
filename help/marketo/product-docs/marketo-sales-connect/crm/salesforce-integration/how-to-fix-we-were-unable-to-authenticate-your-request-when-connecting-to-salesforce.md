---
unique-page-id: 14352484
description: Come risolvere il problema "Impossibile autenticare la richiesta" durante la connessione a Salesforce - Documentazione di Marketo - Documentazione del prodotto
title: Come risolvere il problema "Impossibile autenticare la richiesta" durante la connessione a Salesforce
exl-id: ddd49064-f584-4490-8d45-29cf61ed3ebe
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 0%

---

# Come risolvere il problema &quot;Impossibile autenticare la richiesta&quot; durante la connessione a Salesforce {#how-to-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

Se durante il tentativo di connessione di Sales Connect a Salesforce ricevi il messaggio di errore &quot;Impossibile autenticare la richiesta&quot;, l’accesso all’API di Salesforce potrebbe essere soggetto a restrizioni. Rivolgiti all’amministratore di Salesforce per verificare che siano presenti i seguenti elementi.

## Abilitare l’API nelle autorizzazioni utente {#enable-api-in-user-permissions}

1. Chiedi a un amministratore di Salesforce di accedere a SFDC.
1. Seleziona **Configurazione**.
1. Seleziona **Gestisci utenti**.
1. Seleziona **Profili**.
1. Trova il profilo in cui si trovano gli utenti ToutApp e fai clic su **Modifica**.
1. Scorri verso il basso fino a **Autorizzazioni amministrative** e assicurati che **API abilitata** è selezionato.

## Controlla se Salesforce sta bloccando la connessione delle vendite {#check-if-salesforce-is-blocking-sales-connect-from-connecting}

1. Chiedi a un amministratore di Salesforce di accedere a SFDC.
1. Seleziona **Configurazione**.
1. Seleziona **Gestione app**.
1. Seleziona **Utilizzo OAuth delle app collegate**.
1. Verificare che Sales Connect sia visualizzato accanto a esso il messaggio &quot;Blocca&quot;. Se viene visualizzato &quot;Sblocca&quot;, fare clic sul pulsante per sbloccare l&#39;accesso di Sales Connect a Salesforce.
