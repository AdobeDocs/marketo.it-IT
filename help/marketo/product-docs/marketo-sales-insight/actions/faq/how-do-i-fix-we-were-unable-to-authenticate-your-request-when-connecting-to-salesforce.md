---
description: Come posso risolvere il problema "Impossibile autenticare la richiesta" durante la connessione a Salesforce - Documentazione di Marketo - Documentazione del prodotto
title: Come posso risolvere il problema "Impossibile autenticare la richiesta" durante la connessione a Salesforce?
exl-id: ef876f0f-bd76-4ba5-bf48-885ee048ceae
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 0%

---

# Come posso risolvere il problema &quot;Impossibile autenticare la richiesta&quot; durante la connessione a Salesforce? {#how-do-i-fix-we-were-unable-to-authenticate-your-request-when-connecting-to-salesforce}

Se ricevi il messaggio di errore &quot;Impossibile autenticare la richiesta&quot; quando tenti di collegare le azioni di approfondimento sulle vendite a Salesforce, potresti riscontrare una restrizione nell’accesso all’API di Salesforce. Rivolgiti all’amministratore di Salesforce per verificare che siano presenti i seguenti elementi.

## Abilitare l’API nelle autorizzazioni utente {#enable-api-in-user-permissions}

1. Chiedi a un amministratore di Salesforce di accedere a SFDC.
1. Seleziona **Configurazione**.
1. Seleziona **Gestisci utenti**.
1. Seleziona **Profili**.
1. Trova il profilo in cui si trovano gli utenti ToutApp e fai clic su **Modifica**.
1. Scorri verso il basso fino a **Autorizzazioni amministrative** e assicurati che **API abilitata** è selezionato.

## Controlla se Salesforce sta bloccando la connessione delle azioni di approfondimento sulle vendite {#check-if-salesforce-is-blocking-sales-insight-actions-from-connecting}

1. Chiedi a un amministratore di Salesforce di accedere a SFDC.
1. Seleziona **Configurazione**.
1. Seleziona **Gestione app**.
1. Seleziona **Utilizzo OAuth delle app collegate**.
1. Accertati che Azioni approfondimento vendite sia visualizzato accanto a esso il messaggio &quot;Blocca&quot;. Se viene visualizzato &quot;Sblocca&quot;, fare clic sul pulsante per sbloccare l&#39;accesso a Salesforce da parte delle azioni di approfondimento sulle vendite.
