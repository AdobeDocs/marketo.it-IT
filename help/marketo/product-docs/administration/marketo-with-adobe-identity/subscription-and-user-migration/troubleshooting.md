---
description: Guida alla risoluzione dei problemi di migrazione utente di Adobe IMS - Documentazione di Marketo - Documentazione del prodotto
title: Guida alla risoluzione dei problemi di migrazione utente di Adobe IMS
feature: Marketo with Adobe Identity
exl-id: 921d9d45-c5c2-405c-bd3b-be8aa6d11e2f
source-git-commit: b3bc6a7ec14a513e4b294852d066f9e3d0f74ef8
workflow-type: tm+mt
source-wordcount: '796'
ht-degree: 0%

---

# Guida alla risoluzione dei problemi di migrazione utente di Adobe IMS {#adobe-ims-user-migration-troubleshooting-guide}

Durante il processo di migrazione degli utenti IMS, viene creato un utente di Adobe per ogni utente Marketo Engage migrato (a meno che non esista già con lo stesso indirizzo e-mail). A volte non viene creato, il che può essere attribuito al record dell’utente in Active Directory o a problemi con l’indirizzo e-mail.

In questo articolo, per gli utenti che eseguono la migrazione automatica, vengono elencati tutti i messaggi di errore che possono essere visualizzati nel campo dello stato della console di migrazione automatica.

>[!NOTE]
>
>Gli errori relativi alla directory o al dominio possono essere attivati da un’altra organizzazione o Admin Console in cui è configurato un trust tra directory o il dominio è stato richiesto.

## Messaggi di errore {#error-messages}

Innanzitutto, stabilisci se l’utente deve essere migrato o meno, in quanto questo influenzerà i passaggi di risoluzione da seguire.

Utilizza la sezione &quot;Su questa pagina&quot; a destra per passare direttamente a un errore specifico.

### Carattere Gmail non valido {#gmail-invalid-character}

**Causa principale**: in base ai criteri di sicurezza di Adobe, i caratteri `.` e `+` non sono consentiti in un indirizzo e-mail Gmail. Entrambi i caratteri sono consentiti negli indirizzi e-mail non Gmail.

**Risoluzione**:

_Se è necessario eseguire la migrazione dell&#39;utente_ - L&#39;indirizzo e-mail deve essere aggiornato in Marketo Engage per essere conforme ai criteri di sicurezza di Adobe e sottoposto a nuova verifica. L’amministratore di Marketo dovrà quindi eseguire nuovamente la migrazione degli utenti per questo utente dalla console di migrazione.

_Se l&#39;utente **non**&#x200B;deve essere migrato_ - l&#39;amministratore di Marketo Engage salta l&#39;utente nella console di migrazione. Il pulsante &quot;Migrazione completata&quot; viene visualizzato quando tutti gli utenti vengono considerati tramite la migrazione o il salto. Fai clic sul pulsante per terminare il processo di migrazione utente.

### Utente non presente nella directory {#user-not-in-directory}

**Causa principale**: l&#39;utente non esiste in Active Directory. Per tutte le organizzazioni con SSO per le quali è abilitata la sincronizzazione di Active Directory, la creazione degli utenti è consentita solo tramite il provider di identità (IdP). Di conseguenza, non è stato possibile aggiungere l’utente tramite Admin Console durante la migrazione.

**Risoluzione**:

_Se è necessario eseguire la migrazione dell&#39;utente_ - L&#39;utente deve essere aggiunto ad Active Directory con le autorizzazioni appropriate da un amministratore di sistema. L’amministratore di Marketo Engage dovrà quindi eseguire nuovamente la migrazione degli utenti per questo utente dalla console di migrazione.

_Se l&#39;utente **non**&#x200B;deve essere migrato_ - l&#39;amministratore di Marketo Engage salta l&#39;utente nella console di migrazione. Il pulsante &quot;Migrazione completata&quot; viene visualizzato quando tutti gli utenti vengono considerati tramite la migrazione o il salto. Fai clic sul pulsante per terminare il processo di migrazione utente.

### Utente inattivo {#inactive-user}

**Causa principale**: la sincronizzazione Active Directory è abilitata e l&#39;account federato dell&#39;utente esiste ma è inattivo/disabilitato.

**Risoluzione**:

_Se è necessario eseguire la migrazione dell&#39;utente_ - Lo stato dell&#39;utente e le autorizzazioni appropriate devono essere ripristinati da un amministratore di sistema. L’amministratore di Marketo Engage dovrà quindi eseguire nuovamente la migrazione degli utenti per questo utente dalla console di migrazione.

_Se l&#39;utente **non**&#x200B;deve essere migrato_ - l&#39;amministratore di Marketo Engage salta l&#39;utente nella console di migrazione. Il pulsante &quot;Migrazione completata&quot; viene visualizzato quando tutti gli utenti vengono considerati tramite la migrazione o il salto. Fai clic sul pulsante per terminare il processo di migrazione utente.

### Dominio non valido {#invalid-domain}

**Causa principale**: l&#39;imposizione del dominio è abilitata in Admin Console. Tuttavia, il dominio dell’indirizzo e-mail per l’utente non è uno dei domini consentiti, oppure il dominio è stato registrato in un’altra organizzazione o Admin Console.

**Risoluzione**:

_Se è necessario eseguire la migrazione dell&#39;utente_ (e l&#39;imposizione del dominio è abilitata nell&#39;organizzazione di migrazione) - L&#39;indirizzo e-mail deve essere aggiornato in Marketo Engage per essere conforme al criterio di imposizione del dominio (DE). In alternativa, l&#39;amministratore di sistema può [spostare il dominio](https://helpx.adobe.com/enterprise/using/manage-domains-directories.html#move-domains-across-directories){target="_blank"} in un&#39;altra directory disabilitata di Domain Enforcement (DE) o [creare una nuova directory](https://helpx.adobe.com/it/enterprise/using/set-up-identity.html){target="_blank"} che non sia inclusa nei criteri DE. L’amministratore di Marketo Engage dovrà quindi eseguire nuovamente la migrazione degli utenti per questo utente dalla console di migrazione.

_Se è necessario eseguire la migrazione dell&#39;utente_ (e l&#39;imposizione del dominio è abilitata in un&#39;altra organizzazione), un amministratore di sistema dell&#39;organizzazione in cui il dominio è stato richiesto deve aggiungere l&#39;indirizzo e-mail dell&#39;utente all&#39;elenco di eccezioni. L’amministratore di Marketo Engage dovrà quindi eseguire nuovamente la migrazione degli utenti per questo utente dalla console di migrazione.

_Se l&#39;utente **non**&#x200B;deve essere migrato_ - l&#39;amministratore di Marketo Engage salta l&#39;utente nella console di migrazione. Il pulsante &quot;Migrazione completata&quot; viene visualizzato quando tutti gli utenti vengono considerati tramite la migrazione o il salto. Fai clic sul pulsante per terminare il processo di migrazione utente.

### Creazione utente non riuscita {#user-creation-failed}

[Vedi sotto](#failed)

### Errore Type2E {#type2e-failure}

[Vedi sotto](#failed)

### Adesione Marketo non riuscita {#marketo-entitlement-failed}

[Vedi sotto](#failed)

### Migrazione Pendo non riuscita {#pendo-migration-failed}

[Vedi sotto](#failed)

### Migrazione dei dati utente non riuscita {#user-data-migration-failed}

[Vedi sotto](#failed)

### Sincronizzazione dati prodotto non riuscita {#product-data-sync-failed}

[Vedi sotto](#failed)

### Adesione Adobe non riuscita {#adobe-entitlement-failed}

[Vedi sotto](#failed)

### Disconnessione utente non riuscita {#user-sign-out-failed}

[Vedi sotto](#failed)

### Creazione Adobe ID non riuscita {#adobe-id-creation-failed}

[Vedi sotto](#failed)

### Operazione non riuscita {#failed}

**Causa principale**: questi errori possono essere causati da vari motivi nel back-end.

**Risoluzione**:

Invia un caso di supporto con i dettagli rilevanti per [Supporto Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.
