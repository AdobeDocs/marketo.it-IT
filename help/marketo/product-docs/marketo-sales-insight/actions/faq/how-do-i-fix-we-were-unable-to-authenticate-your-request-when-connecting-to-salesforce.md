---
description: Come posso correggere "Non siamo riusciti ad autenticare la tua richiesta" quando ci si connette a Salesforce - Marketo Docs - Documentazione del prodotto
title: Come posso correggere "Non siamo riusciti ad autenticare la tua richiesta" quando ci si connette a Salesforce
hide: true
hidefromtoc: true
source-git-commit: c398aff77e09f4a63db5d51af55178aa663ec98e
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 0%

---

# Come posso correggere &quot;Non siamo riusciti ad autenticare la tua richiesta&quot; quando ci si connette a Salesforce {#how-do-i-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

Se ricevi il messaggio di errore &quot;Impossibile autenticare la tua richiesta&quot; durante il tentativo di collegare le azioni Insight vendite a Salesforce, potrebbe esserci una restrizione all’accesso all’API di Salesforce. Controlla con il tuo amministratore Salesforce per assicurarti che siano presenti le seguenti funzioni.

## Abilitare API nelle autorizzazioni utente {#enable-api-in-user-permissions}

1. Avere un accesso amministratore Salesforce in SFDC.
1. Seleziona **Configurazione**.
1. Seleziona **Gestione utenti**.
1. Seleziona **Profili**.
1. Trova il profilo in cui si trovano gli utenti di ToutApp e fai clic su **Modifica**.
1. Scorri verso il basso fino a **Autorizzazioni amministrative** e assicurati **API abilitata** è controllata.

## Controlla se Salesforce sta bloccando le azioni di Insight sulle vendite dalla connessione {#check-if-salesforce-is-blocking-sales-insight-actions-from-connecting}

1. Disporre di un accesso Admin Salesforce a SFDC.
1. Seleziona **Configurazione**.
1. Seleziona **Gestione app**.
1. Seleziona **Utilizzo OAuth delle app collegate**.
1. Assicurati che le azioni Approfondimenti vendite mostrino il &quot;Blocco&quot; accanto ad esso. Se vedi &quot;Sblocca&quot;, fai clic sul pulsante per sbloccare l&#39;accesso a Salesforce delle azioni Insight vendite.
