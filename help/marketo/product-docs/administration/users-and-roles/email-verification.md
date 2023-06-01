---
description: Verifica e-mail - Documentazione di Marketo - Documentazione del prodotto
title: Verifica e-mail
exl-id: 976e46a7-8c85-45ed-86c1-0c5cdb2d5c3e
source-git-commit: 44cca5ebad831cc39babac87ac9ebbf53df6c795
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 0%

---

# Verifica e-mail {#email-verification}

Gli abbonamenti Adobe Marketo Engage richiedono a tutti gli utenti non API, inclusi gli amministratori di Marketo Engage, di verificare il proprio indirizzo e-mail. Gli utenti Single Sign-on (SSO) a cui non è assegnato un ruolo di amministratore o a cui è assegnato un ruolo con l’autorizzazione &quot;Ignora SSO&quot; avranno automaticamente la verifica della propria e-mail quando la sottoscrizione viene abilitata con la funzione di verifica e-mail.

## Invito utente {#user-invite}

Quando un amministratore invita un utente, quest’ultimo viene verificato automaticamente dopo aver fatto clic sul collegamento di invito. Gli utenti SSO a cui non è assegnato il ruolo di amministratore vengono verificati automaticamente.

## Modifica di un indirizzo e-mail {#changing-an-email-address}

Quando l’indirizzo e-mail di un utente viene modificato, non viene verificato. Verrà inviata loro un’e-mail che consentirà di eseguire nuovamente la verifica. Gli utenti possono inviare nuovamente tale e-mail facendo clic su **Invia di nuovo la verifica**.

![](assets/email-verification-1.png)

![](assets/email-verification-2.png)

## Utenti e ruoli {#users-and-roles}

In entrata **Amministratore** > **Utenti e ruoli**, la colonna Stato e-mail mostra lo stato di verifica di ogni utente.

![](assets/email-verification-3.png)

## ID di accesso per più utenti {#multiple-user-login-ids}

A un singolo indirizzo e-mail può essere associato un solo account utente. Se a un singolo indirizzo e-mail sono associati più account utente, il Marketo Engage richiederà la risoluzione del conflitto e la visualizzazione di tutti gli accessi utente associati all&#39;indirizzo e-mail, oltre a tre opzioni di risoluzione:<p>
`1` Utilizza l&#39;e-mail corrente per l&#39;ID accesso utente corrente<p>
`2` Utilizza una nuova e-mail per l&#39;ID di accesso utente corrente<p>
`3` Posticipa la decisione al prossimo accesso

![](assets/email-verification-4.png)

## E-mail di verifica {#verification-email}

Gli utenti invitati riceveranno la seguente e-mail:

![](assets/email-verification-5.png)

>[!NOTE]
>
>Per inviare di nuovo un messaggio e-mail di verifica a un utente non verificato, selezionane il record e fai clic su **Verifica e-mail** pulsante.
