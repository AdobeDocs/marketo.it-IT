---
description: Guida alla risoluzione dei problemi di Adobe IMS - Documentazione di Marketo - Documentazione del prodotto
title: Guida alla risoluzione dei problemi di Adobe IMS
hide: true
hidefromtoc: true
feature: Marketo with Adobe Identity
exl-id: 921d9d45-c5c2-405c-bd3b-be8aa6d11e2f
source-git-commit: 2a01045abbc23bce9531c64e3494fb12a9adf1bd
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# Guida alla risoluzione dei problemi di Adobe IMS {#adobe-ims-troubleshooting-guide}

Durante il processo di migrazione degli utenti IMS, viene creato un utente Adobe per ogni utente Marketo Engage migrato. A volte non viene creata (per vari motivi, relativi al record dell’utente in Active Directory o a problemi con l’indirizzo e-mail). In questo caso, l’amministratore di Marketo Engage visualizzerà il motivo nel campo dello stato di migrazione dell’utente nella console di automigrazione.

## Messaggi di errore {#error-messages}

Utilizza la sezione &quot;Su questa pagina&quot; a destra per passare direttamente a un errore specifico e imparare a risolverlo.

### Non in directory {#not-in-directory}

_Causa principale_: l&#39;utente non esiste in Active Directory. Per tutte le organizzazioni con SSO per le quali è abilitata la sincronizzazione di Active Directory, la creazione degli utenti è consentita solo tramite il provider di identità (IdP). Di conseguenza, non è stato possibile aggiungere l’utente tramite Admin Console durante la migrazione.

_Risoluzione_:

Pre-migrazione: l’amministratore di Marketo Enage può saltare l’utente nella console di migrazione. Il pulsante &quot;Migrazione completata&quot; viene visualizzato quando tutti gli utenti vengono considerati tramite la migrazione o il salto. Fai clic sul pulsante per terminare il processo di migrazione utente.

Post-migrazione: l&#39;utente deve essere aggiunto ad Active Directory con le autorizzazioni appropriate. L’amministratore di Marketo Engage dovrà quindi eseguire nuovamente la migrazione degli utenti per questo utente dalla console di migrazione.

### Carattere Gmail non valido {#gmail-invalid-character}

_Causa principale_: in base ai criteri di sicurezza di Adobe, i caratteri `.` e `+` non sono consentiti in un indirizzo e-mail Gmail. Entrambi i caratteri sono consentiti negli indirizzi e-mail non Gmail.

_Risoluzione_:

Pre-migrazione: l’amministratore di Marketo Enage può saltare l’utente nella console di migrazione. Il pulsante &quot;Migrazione completata&quot; viene visualizzato quando tutti gli utenti vengono considerati tramite la migrazione o il salto. Fai clic sul pulsante per terminare il processo di migrazione utente.

Post-migrazione: l’indirizzo e-mail deve essere aggiornato in Marketo Engage per rispettare i criteri di sicurezza di Adobe. L’amministratore di Marketo deve eseguire nuovamente la migrazione degli utenti per questo utente dalla console di migrazione.

### Utente inattivo {#inactive-user}

_Causa principale_: la sincronizzazione Active Directory è abilitata e l&#39;account federato dell&#39;utente esiste ma è inattivo/disabilitato.

_Risoluzione_:

Pre-migrazione: l’amministratore di Marketo Enage può saltare l’utente nella console di migrazione. Il pulsante &quot;Migrazione completata&quot; viene visualizzato quando tutti gli utenti vengono considerati tramite la migrazione o il salto. Fai clic sul pulsante per terminare il processo di migrazione utente.

Post-migrazione: è necessario ripristinare lo stato e le autorizzazioni appropriate dell’utente. L’amministratore di Marketo Engage dovrà quindi eseguire nuovamente la migrazione degli utenti per questo utente dalla console di migrazione.

### Non nel dominio {#not-in-domain}

_Causa principale_: l&#39;imposizione del dominio è abilitata in Admin Console, ma il dominio dell&#39;indirizzo e-mail per l&#39;utente non è uno dei domini consentiti.

_Risoluzione_:

Pre-migrazione: l’amministratore di Marketo Enage può saltare l’utente nella console di migrazione. Il pulsante &quot;Migrazione completata&quot; viene visualizzato quando tutti gli utenti vengono considerati tramite la migrazione o il salto. Fai clic sul pulsante per terminare il processo di migrazione utente.

Post-migrazione: l’indirizzo e-mail deve essere aggiornato in Marketo Engage per rispettare i criteri di imposizione del dominio (DE). In alternativa, l&#39;amministratore di sistema può [spostare il dominio](https://helpx.adobe.com/enterprise/using/manage-domains-directories.html#move-domains-across-directories){target="_blank"} in un&#39;altra directory disabilitata di Domain Enforcement (DE) o [creare una nuova directory](https://helpx.adobe.com/it/enterprise/using/set-up-identity.html){target="_blank"} che non sia inclusa nei criteri DE. L’amministratore di Marketo Engage dovrà quindi eseguire nuovamente la migrazione degli utenti per questo utente dalla console di migrazione.

### Errore di creazione {#create-failure}

_Causa principale_: questo errore può essere causato da vari motivi nel back-end.

_Risoluzione_:

Pre-migrazione - Invia un caso di supporto per [non ancora migrati](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

Post-migrazione - Invia un caso di supporto per i [già migrati](https://experienceleague.adobe.com/home?support-tab=home#support){target="_blank"}.

### Errore utente Type2e {#type2e-user-failure}

_Causa principale_: questo errore può essere causato da vari motivi nel back-end.

_Risoluzione_:

Pre-migrazione - Invia un caso di supporto per [non ancora migrati](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

Post-migrazione - Invia un caso di supporto per i [già migrati](https://experienceleague.adobe.com/home?support-tab=home#support){target="_blank"}.
