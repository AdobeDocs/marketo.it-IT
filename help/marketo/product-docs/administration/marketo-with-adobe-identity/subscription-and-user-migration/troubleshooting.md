---
description: Guida alla risoluzione dei problemi di migrazione utente di Adobe IMS - Documentazione di Marketo - Documentazione del prodotto
title: Guida alla risoluzione dei problemi di migrazione utente di Adobe IMS
hide: true
hidefromtoc: true
feature: Marketo with Adobe Identity
exl-id: 921d9d45-c5c2-405c-bd3b-be8aa6d11e2f
source-git-commit: e96bc8676a73694ec60f46bb045f2a6ea5d8069c
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 0%

---

# Guida alla risoluzione dei problemi di migrazione utente di Adobe IMS {#adobe-ims-user-migration-troubleshooting-guide}

Durante il processo di migrazione degli utenti IMS, viene creato un utente di Adobe per ogni utente Marketo Engage migrato (a meno che non esista già con lo stesso indirizzo e-mail). A volte non viene creato, il che può essere attribuito al record dell’utente in Active Directory o a problemi con l’indirizzo e-mail. In questo caso, l’amministratore di Marketo Engage visualizzerà il motivo nel campo dello stato di migrazione dell’utente nella console di automigrazione.

## Messaggi di errore {#error-messages}

Innanzitutto, stabilisci se l’utente deve essere migrato o meno, in quanto questo influenzerà i passaggi di risoluzione da seguire.

Utilizza la sezione &quot;Su questa pagina&quot; a destra per passare direttamente a un errore specifico.

### Non in directory {#not-in-directory}

**Causa principale**: l&#39;utente non esiste in Active Directory. Per tutte le organizzazioni con SSO per le quali è abilitata la sincronizzazione di Active Directory, la creazione degli utenti è consentita solo tramite il provider di identità (IdP). Di conseguenza, non è stato possibile aggiungere l’utente tramite Admin Console durante la migrazione.

**Risoluzione**:

_Se non è necessario eseguire la migrazione dell&#39;utente_, l&#39;amministratore di Marketo Engage salterà l&#39;utente nella console di migrazione. Il pulsante &quot;Migrazione completata&quot; viene visualizzato quando tutti gli utenti vengono considerati tramite la migrazione o il salto. Fai clic sul pulsante per terminare il processo di migrazione utente.

_Se è necessario eseguire la migrazione dell&#39;utente_, è necessario che l&#39;utente venga aggiunto ad Active Directory con le autorizzazioni appropriate da parte di un amministratore di sistema. L’amministratore di Marketo Engage dovrà quindi eseguire nuovamente la migrazione degli utenti per questo utente dalla console di migrazione.

### Carattere Gmail non valido {#gmail-invalid-character}

**Causa principale**: in base ai criteri di sicurezza di Adobe, i caratteri `.` e `+` non sono consentiti in un indirizzo e-mail Gmail. Entrambi i caratteri sono consentiti negli indirizzi e-mail non Gmail.

**Risoluzione**:

_Se non è necessario eseguire la migrazione dell&#39;utente_, l&#39;amministratore di Marketo Engage salterà l&#39;utente nella console di migrazione. Il pulsante &quot;Migrazione completata&quot; viene visualizzato quando tutti gli utenti vengono considerati tramite la migrazione o il salto. Fai clic sul pulsante per terminare il processo di migrazione utente.

_Se è necessario eseguire la migrazione dell&#39;utente_ - L&#39;indirizzo e-mail deve essere aggiornato in Marketo Engage per rispettare i criteri di sicurezza di Adobe e ricontrollato. L’amministratore di Marketo dovrà quindi eseguire nuovamente la migrazione degli utenti per questo utente dalla console di migrazione.

### Utente inattivo {#inactive-user}

**Causa principale**: la sincronizzazione Active Directory è abilitata e l&#39;account federato dell&#39;utente esiste ma è inattivo/disabilitato.

**Risoluzione**:

_Se non è necessario eseguire la migrazione dell&#39;utente_, l&#39;amministratore di Marketo Engage salterà l&#39;utente nella console di migrazione. Il pulsante &quot;Migrazione completata&quot; viene visualizzato quando tutti gli utenti vengono considerati tramite la migrazione o il salto. Fai clic sul pulsante per terminare il processo di migrazione utente.

_Se non è necessario eseguire la migrazione dell&#39;utente_, è necessario ripristinare lo stato e le autorizzazioni appropriate dell&#39;utente. L’amministratore di Marketo Engage dovrà quindi eseguire nuovamente la migrazione degli utenti per questo utente dalla console di migrazione.

### Non nel dominio {#not-in-domain}

**Causa principale**: l&#39;imposizione del dominio è abilitata in Admin Console, ma il dominio dell&#39;indirizzo e-mail per l&#39;utente non è uno dei domini consentiti.

**Risoluzione**:

_Se non è necessario eseguire la migrazione dell&#39;utente_, l&#39;amministratore di Marketo Engage salterà l&#39;utente nella console di migrazione. Il pulsante &quot;Migrazione completata&quot; viene visualizzato quando tutti gli utenti vengono considerati tramite la migrazione o il salto. Fai clic sul pulsante per terminare il processo di migrazione utente.

_Se è necessario eseguire la migrazione dell&#39;utente_ - L&#39;indirizzo e-mail deve essere aggiornato in Marketo Engage per rispettare il criterio di imposizione del dominio (DE). In alternativa, l&#39;amministratore di sistema può [spostare il dominio](https://helpx.adobe.com/enterprise/using/manage-domains-directories.html#move-domains-across-directories){target="_blank"} in un&#39;altra directory disabilitata di Domain Enforcement (DE) o [creare una nuova directory](https://helpx.adobe.com/it/enterprise/using/set-up-identity.html){target="_blank"} che non sia inclusa nei criteri DE. L’amministratore di Marketo Engage dovrà quindi eseguire nuovamente la migrazione degli utenti per questo utente dalla console di migrazione.

### Errore di creazione {#create-failure}

**Causa principale**: questo errore può essere causato da vari motivi nel back-end.

**Risoluzione**:

Invia un caso di supporto con i dettagli rilevanti per [Supporto Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

### Errore utente Type2e {#type2e-user-failure}

**Causa principale**: questo errore può essere causato da vari motivi nel back-end.

**Risoluzione**:

Invia un caso di supporto con i dettagli rilevanti per [Supporto Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.
