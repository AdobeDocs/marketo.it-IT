---
description: Abbonamento a Marketo e migrazione degli utenti al Adobe Admin Console - Documentazione di Marketo - Documentazione del prodotto
title: Abbonamento a Marketo e migrazione degli utenti a Adobe Admin Console
exl-id: 91e7b56b-2563-4986-a55c-f9760ea88b05
feature: Marketo with Adobe Identity
source-git-commit: c871be92ce61c37e9a8d198c1b3bae6588f6a94f
workflow-type: tm+mt
source-wordcount: '1172'
ht-degree: 0%

---

# Abbonamento a Marketo e migrazione degli utenti a Adobe Admin Console {#understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console}

Adobe migliora il modo in cui gestisci gli abbonamenti e gli utenti Adobe Marketo Engage, aumentando la produttività per te e la tua organizzazione. Come parte di questa modifica, Adobe sta eseguendo la migrazione degli abbonamenti e degli utenti del Marketo Engage al Adobe Admin Console. Si tratta di una migrazione necessaria e non influirà su flussi di lavoro, contenuti, integrazioni o risorse di marketing.

Scopri come utilizzare Adobe Admin Console per gestire i diritti Adobi in tutta l’organizzazione con [Guida per l’amministratore di Enterprise e Teams](https://helpx.adobe.com/it/enterprise/admin-guide.html){target="_blank"}.

## Cosa sta cambiando? {#what-is-changing}

Come parte della migrazione, la gestione dell’abbonamento e degli utenti passerà dall’applicazione Marketo a Adobe Admin Console.

* **Gli amministratori di sistema gestiranno gli abbonamenti su Adobe Admin Console**. Visualizza tutti i tuoi prodotti di Adobe in un’unica console.

* **Gli amministratori di prodotto gestiranno gli utenti e il loro accesso su Adobe Admin Console**. Aggiungi e rimuovi utenti per tutte le sottoscrizioni di Adobi.

* **Gli utenti effettueranno l&#39;accesso con Adobe Identity**. Adobe eseguirà la migrazione degli utenti esistenti a Adobe Admin Console. Gli utenti accederanno alle sottoscrizioni Marketo utilizzando la nuova identità Adobe, un Adobe ID o un Federated ID Adobe (SSO).

* **Non cambia il modo in cui gestisci tutte le altre funzionalità** all&#39;interno dell&#39;applicazione di Marketo Engage stessa, inclusa la gestione di funzionalità, ruoli utente, aree di lavoro, funzionalità e comportamento.


## Timeline del Percorso di migrazione {#migration-journey-timeline}

Adobe eseguirà prima la migrazione degli abbonamenti di Marketo Engage a Adobe Admin Console, quindi eseguirà la migrazione di tutti gli utenti esistenti con indirizzi e-mail verificati. Se sei un amministratore di sistema o un amministratore di prodotto Marketo, riceverai e-mail che ti guidano attraverso il percorso di migrazione. Ecco una cronologia di ciò che puoi aspettarti:

### Migrazione abbonamento completata {#subscription-migration-complete}

Gli amministratori di sistema riceveranno un’e-mail al termine della migrazione dell’abbonamento a Adobe Admin Console.

Per ridurre al minimo l’impatto sugli utenti di Marketo, gli amministratori di sistema potrebbero dover completare alcuni passaggi obbligatori prima di avviare la migrazione degli utenti:

* Se gli utenti di Marketo al momento effettuano l&#39;accesso con SSO, ti verrà richiesto di impostare SSO su Adobe Admin Console in modo che gli utenti possano continuare ad accedere con SSO. Se gli utenti di Marketo al momento non utilizzano l’SSO, ma desideri configurarlo su Adobe Admin Console, puoi farlo a questo punto nel percorso di migrazione.

* Se gestisci già altri prodotti Adobe nel Adobe Admin Console, Adobe potrebbe richiedere il consenso per migrare automaticamente gli utenti alla console esistente. Per accedere alla pagina del consenso, fai clic sul pulsante &quot;Inizia&quot; nell’e-mail.

Al momento non vi sono modifiche alla gestione degli utenti. Gli amministratori di Marketo continueranno a gestire gli utenti nell’area di amministrazione di Marketo e gli utenti continueranno ad accedere con la loro identità Marketo fino a quando la migrazione degli utenti non sarà completata.

### Pianifica migrazione utenti {#schedule-user-migration}

Una volta che l’amministratore di sistema avrà soddisfatto i prerequisiti descritti nella sezione precedente, Adobe pianificherà automaticamente la migrazione utente con 30 giorni di anticipo e comunicherà con gli amministratori di prodotto Marketo per gestire la migrazione degli utenti.

Gli amministratori di prodotto Marketo:

* Ricevi un’e-mail con la data di inizio della migrazione utente pianificata, 30 giorni prima.

* Accedi a Marketo Migration Console, che si trova nell’area di amministrazione di Marketo, e consente di modificare la data di migrazione di un abbonamento.

>[!NOTE]
>
>A causa della complessità della migrazione, le modifiche della data sono limitate a non più di 30 giorni oltre la data pianificata. Se hai bisogno di una data successiva, invia un’e-mail a marketocares@marketo.com.

* Visualizza un banner in Il mio Marketo che mostra un conto alla rovescia per la data di inizio della migrazione utente.

* Ricevi un messaggio e-mail di promemoria il giorno precedente alla data di inizio della migrazione utente.

### Prepara utenti per il giorno della migrazione {#prepare-users-for-migration-day}

In qualità di amministratore di prodotto Marketo, sei invitato a garantire che tutti gli utenti siano preparati per la migrazione.

* Verifica [verifica e-mail](/help/marketo/product-docs/administration/users-and-roles/email-verification.md){target="_blank"} stato per tutti gli utenti nell’area di amministrazione di Marketo. Incoraggia gli utenti che non hanno verificato il proprio indirizzo e-mail a farlo e aiuta gli utenti a risolvere eventuali problemi durante il completamento del processo di verifica.

* Prepara tutti gli utenti per la prossima migrazione all’identità Adobe.

>[!NOTE]
>
>Durante la migrazione, gli utenti riceveranno un’e-mail da Adobe con la notifica della modifica del modo in cui accedono a Marketo. Gli utenti saranno invitati ad accettare un invito ad accedere utilizzando Adobe Identity per la prima volta, effettuando l’accesso con un Adobe ID esistente o configurandone uno nuovo utilizzando lo stesso indirizzo e-mail.

>[!IMPORTANT]
>
>Se un utente del Marketo Engage non verifica il proprio indirizzo e-mail, non eseguirà la migrazione a un Adobe ID e perderà l’accesso all’abbonamento a Marketo al termine della migrazione per l’abbonamento. Per recuperare l’accesso, un amministratore di prodotto Marketo deve aggiungerli come nuovo utente.

### Cosa aspettarsi il giorno della migrazione {#what-to-expect-on-migration-day}

La migrazione degli utenti inizierà alla mezzanotte del fuso orario impostato nell’abbonamento a Marketo.

**Adobe eseguirà automaticamente prima la migrazione degli amministratori di Marketo**. Quando gli amministratori di Marketo vengono migrati a Adobe Identity, ad essi verrà assegnato il ruolo di amministratore del prodotto di Adobe all’interno dell’applicazione Marketo insieme a tutti gli altri ruoli che avevano in precedenza.

**Se il tuo abbonamento a Marketo ha meno di 75 utenti**, Adobe eseguirà automaticamente la migrazione degli altri utenti. Questo flusso di lavoro mira a fornire il massimo livello di automazione per ridurre al minimo il sovraccarico per gli utenti di Marketo, ad Adobe. Non è richiesta alcuna azione da parte tua per eseguire la migrazione.

**Se il tuo abbonamento a Marketo ha più di 75 utenti**, gli amministratori di prodotto Marketo avranno accesso all’area Self-Service User Migration di Marketo Migration Console, che si trova nell’area di amministrazione di Marketo. Per coloro che necessitano di un maggiore controllo durante il processo di migrazione degli utenti, gli amministratori di prodotto Marketo potranno iniziare a selezionare gli utenti da migrare in batch o tutti in una sola volta. Una volta selezionati gli utenti, gli amministratori possono scegliere &quot;Migra ora&quot; o &quot;Pianifica migrazione&quot; per una data successiva, offrendo agli amministratori flessibilità e controllo massimi su quali utenti vengono migrati quando.

>[!NOTE]
>
>Non si verificherà alcuna perdita di accesso al prodotto durante la migrazione degli utenti. Se un utente ha eseguito l’accesso durante la migrazione, verrà disconnesso e gli verrà richiesto di eseguire nuovamente l’accesso in pochi minuti utilizzando Identità Adobe al termine della migrazione.

Durante la migrazione, gli utenti riceveranno un’e-mail da Adobe con la notifica della modifica del modo in cui accedono a Marketo. Gli utenti saranno invitati ad accettare un invito ad accedere utilizzando Adobe Identity per la prima volta, effettuando l’accesso con un Adobe ID esistente o configurando un nuovo Adobe ID utilizzando lo stesso indirizzo e-mail. Ulteriori informazioni sono disponibili nella [Accesso utente con Adobe](/help/marketo/product-docs/administration/marketo-with-adobe-identity/user-sign-in-with-adobe-id.md){target="_blank"} articolo.

## Migrazione utente completata {#user-migration-complete}

Adobe invierà una notifica a tutti gli amministratori di sistema e di prodotto tramite e-mail dopo la migrazione di tutti gli amministratori e gli utenti. Al momento, tutti gli utenti di Marketo per tale abbonamento accederanno a Marketo utilizzando Adobe Identity e gli amministratori di prodotto gestiranno gli utenti solo su Adobe Admin Console.

## Ottieni supporto {#get-support}

Per ulteriore supporto relativo all’abbonamento o alla migrazione degli utenti, invia un messaggio e-mail a marketocares@marketo.com.
