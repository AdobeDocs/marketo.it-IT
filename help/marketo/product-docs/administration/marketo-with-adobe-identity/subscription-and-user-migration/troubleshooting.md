---
description: Guida alla risoluzione dei problemi di Adobe IMS - Documentazione di Marketo - Documentazione del prodotto
title: Guida alla risoluzione dei problemi di Adobe IMS
hide: true
hidefromtoc: true
feature: Marketo with Adobe Identity
source-git-commit: eccebb8352c56770dea5af9395c8bc83a08525dd
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 0%

---

# Guida alla risoluzione dei problemi di Adobe IMS {#adobe-ims-troubleshooting-guide}

Durante il processo di migrazione degli utenti IMS, viene creato un utente Adobe per ogni utente Marketo Engage migrato. A volte non viene creata (per vari motivi, relativi al record dell’utente in Active Directory o a problemi con l’indirizzo e-mail). In questo caso, l’amministratore di Marketo Engage visualizzerà i motivi nel campo dello stato di migrazione dell’utente nella console di automigrazione. Scopri come risolvere i vari problemi relativi alla creazione di utenti in Adobe, di seguito.

## Messaggi di errore {#error-messages}

* <a href="#not-in-directory">Non presente nella directory</a>
* <a href="#gmail-invalid-character">Carattere Non Valido Per Gmail</a>
* <a href="#inactive-user">Utente inattivo</a>
* <a href="#not-in-domain">Non nel dominio</a>
* <a href="#create-failure">Errore di creazione</a>
* <a href="#type2e-user-failure">Errore utente Type2e</a>



<table>
<thead>
  <tr>
    <th style="width:20%">Messaggio di errore</th>
    <th style="width:40%">Causa principale</th>
    <th style="width:40%">Risoluzioni</th>
  </tr>
  </thead>
<tbody>
  <tr>
    <td><i><a id="not-in-directory">Non in directory</a></i></td>
    <td>L'utente non esiste in Active Directory. Per tutte le organizzazioni con SSO per le quali è abilitata la sincronizzazione Active Directory, la creazione degli utenti è consentita solo tramite il provider di identità (IdP). Pertanto, non è stato possibile aggiungere l’utente tramite Admin Console durante la migrazione utente.</td>
    <td>Migra: l'utente deve essere aggiunto ad Active Directory con le autorizzazioni appropriate. L’amministratore di Marketo deve eseguire nuovamente la migrazione degli utenti per questo utente dalla console di migrazione. 
    <br>Non eseguire la migrazione - L'amministratore di Marketo salta l'utente nella console di migrazione. Il pulsante "Migration Complete" (Migrazione completata) viene visualizzato quando tutti gli utenti vengono considerati durante la migrazione o il salto. Fai clic su di esso per terminare il processo di migrazione utente.</td>
  </tr>
  <tr>
    <td><i><a id="gmail-invalid-character">Carattere Gmail non valido</a></i></td>
    <td>In base ai criteri di sicurezza di Adobe, '.' e il segno '+' non sono consentiti solo in un indirizzo e-mail di dominio Gmail  
    <br>Entrambi i caratteri speciali sono consentiti in un indirizzo e-mail di dominio non Gmail. </td>
    <td>Migra: per rispettare i criteri di sicurezza di Adobe, l’indirizzo e-mail deve essere aggiornato in Marketo Engage. L’amministratore di Marketo deve eseguire nuovamente la migrazione degli utenti per questo utente da Migration Console.<br>Non eseguire la migrazione - L'amministratore di Marketo salta l'utente nella console di migrazione. Il pulsante "Migration Complete" (Migrazione completata) viene visualizzato quando tutti gli utenti vengono considerati durante la migrazione o il salto. Fai clic su di esso per terminare il processo di migrazione utente.</td>
  </tr>
  <tr>
    <td><i><a id="inactive-user">Utente inattivo</a></i></td>
    <td>Sincronizzazione Active Directory è abilitata e l'account federato dell'utente esiste ma è inattivo/disabilitato.</td>
    <td>Migra: è necessario ripristinare lo stato dell’utente e le autorizzazioni appropriate. L’amministratore di Marketo deve eseguire nuovamente la migrazione degli utenti per questo utente dalla console di migrazione.
    <br>Non eseguire la migrazione - L'amministratore di Marketo salta l'utente nella console di migrazione. Il pulsante "Migration Complete" (Migrazione completata) viene visualizzato quando tutti gli utenti vengono considerati durante la migrazione o il salto. Fai clic su di esso per terminare il processo di migrazione utente.</td>
  </tr>
  <tr>
    <td><i><a id="not-in-domain">Non nel dominio</a></i></td>
    <td>L’imposizione del dominio è abilitata in Admin Console, ma il dominio dell’indirizzo e-mail per l’utente non è uno dei domini consentiti. 
    <br>I criteri di imposizione del dominio sono impostati a livello di directory.</td>
    <td>Migra - È necessario aggiornare l'indirizzo e-mail in Marketo Engage per rispettare i criteri di imposizione del dominio oppure l'amministratore di sistema può <a href="https://helpx.adobe.com/enterprise/using/manage-domains-directories.html#move-domains-across-directories"> 
    spostare il dominio in un'altra directory disabilitata di tipo Applicazione dominio </a>o <a href="https://helpx.adobe.com/it/enterprise/using/set-up-identity.html">creare una nuova directory</a>, che non si trova nel criterio DE. L’amministratore di Marketo deve eseguire nuovamente la migrazione degli utenti per questo utente da Migration Console. <br>Non eseguire la migrazione - L'amministratore di Marketo salta l'utente nella console di migrazione. Il pulsante "Migration Complete" (Migrazione completata) viene visualizzato quando tutti gli utenti vengono considerati durante la migrazione o il salto. Fai clic su di esso per terminare il processo di migrazione utente.</td>
  </tr>
  <tr>
    <td><i><a id="create-failure">Errore di creazione</a></i></td>
    <td>Vari motivi nel backend.</td>
    <td>Inviare un caso di supporto.</td>
  </tr>
  <tr>
    <td><i><a id="type2e-user-failure">Errore utente Type2e</a></i></td>
    <td>Vari motivi nel backend.</td>
    <td>Inviare un caso di supporto.</td>
  </tr>
</tbody>
</table>
