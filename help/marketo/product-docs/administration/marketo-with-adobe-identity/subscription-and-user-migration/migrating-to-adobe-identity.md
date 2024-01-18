---
description: Migrazione a Identità Adobe - Documentazione Marketo - Documentazione del prodotto
title: Migrazione all’identità Adobe
hide: true
hidefromtoc: true
feature: Marketo with Adobe Identity
exl-id: a7969204-0ec9-45aa-a206-eff2df8adcd0
source-git-commit: e99fa6d25bcf3c4a03234ce48dd17dd7c396c430
workflow-type: tm+mt
source-wordcount: '2329'
ht-degree: 0%

---

# Migrazione all’identità Adobe {#migrating-to-adobe-identity}

Quando Adobe pianifica la migrazione di un utente di un abbonamento, gli amministratori dei prodotti di Marketo Engage avranno accesso alla console di migrazione, a cui è possibile accedere dal menu di navigazione nell’area Amministratore nell’argomento Integrazione.

SCHERMATA

## Pre-migrazione {#pre-migration}

Prima dell’inizio della migrazione, un amministratore può modificare la data di inizio della migrazione degli utenti per il proprio abbonamento passando alla schermata Pre-migrazione nella console di migrazione. Per modificare la data, l’amministratore può fare clic sul pulsante **Modifica** pulsante.

SCHERMATA

L’amministratore può scegliere una data compresa tra 8 e 30 giorni nel futuro. Quando viene selezionata una data, l’amministratore deve fare clic su **Salva** per apportare la modifica.

SCHERMATA

>[!NOTE]
>
>Per richiedere una data prima degli 8 giorni o oltre i 30, o se devi modificare la data dopo il blocco della console di pre-migrazione, invia un’e-mail a `marketocares@marketo.com`.

## Migrazioni all’identità Adobe {#migrations-to-adobe-identity}

Tutti gli abbonamenti Marketo con fuso orario negli Stati Uniti verranno migrati a partire dalla mezzanotte (ora standard del Pacifico) della data di inizio della migrazione degli utenti. La migrazione degli utenti per tutti gli altri abbonamenti inizierà alla mezzanotte del fuso orario specificato per l’abbonamento. Quando inizia la migrazione degli utenti di un abbonamento, la gestione degli utenti non sarà più disponibile nell’area di amministrazione di Marketo e sarà ottenuta solo in Adobe Admin Console. La gestione dei ruoli rimane nella scheda Utenti e ruoli dell’area di amministrazione di Marketo, nonché nella gestione locale degli utenti (solo API).

Adobe eseguirà automaticamente la migrazione di tutti gli amministratori di Marketo con prima le e-mail verificate. Quando gli amministratori di Marketo vengono trasferiti ad Adobe Identity, vengono aggiunti a Adobe Admin Console come amministratore di prodotto per l’abbonamento a Marketo dell’abbonamento e ricevono il ruolo di amministratore del prodotto di Adobe all’interno dell’applicazione Marketo (insieme a tutti gli altri ruoli che avevano in precedenza) e dispongono del diritto Adobe ID all’abbonamento. Gli amministratori riceveranno due e-mail. Una indica che l’utente è assegnato come amministratore di prodotto Adobe, l’altra che indica che l’utente Adobe ID ha diritto al prodotto Marketo.

**E-mail per l&#39;amministratore del prodotto Marketo**

SCHERMATA

**E-mail di adesione Marketo**

SCHERMATA

**Se il tuo abbonamento a Marketo ha meno di 75 utenti**, Adobe eseguirà automaticamente la migrazione degli altri utenti. Questo flusso di lavoro mira a fornire il massimo livello di automazione e non è necessaria alcuna azione per eseguire la migrazione. Al termine della migrazione, Marketo Migration Console non verrà più visualizzato nell’area di navigazione di Marketo Admin e tutti gli utenti accederanno a Marketo utilizzando un Adobe ID.

**Se il tuo abbonamento a Marketo ha 75 o più utenti**, gli amministratori di prodotto Marketo avranno accesso allo strumento di migrazione self-service degli utenti della console di migrazione all’inizio della migrazione degli utenti e riceveranno un avviso tramite banner al momento dell’accesso alla pagina My Marketo. L&#39;amministratore sarà responsabile del completamento della migrazione degli utenti mediante lo strumento di migrazione self-service degli utenti.

SCHERMATA

## Migrazione degli utenti self-service di Marketo {#marketo-self-service-user-migration}

Lo strumento Marketo Self-Service User Migration Console è costituito da due schede.

* **Scheda Stato di migrazione**
* **Scheda Migrazione utenti**

### Scheda Stato di migrazione {#migration-status-tab}

La scheda Stato di migrazione fornisce metriche generali sull’avanzamento dei prerequisiti di verifica e-mail degli utenti, sulla migrazione e l’attivazione degli utenti e sul completamento della migrazione dell’abbonamento.

SCHERMATA

Nella parte superiore dello Stato di migrazione vengono visualizzati la scadenza della migrazione dell’abbonamento e il pulsante per estendere la scadenza. Ulteriori informazioni sulla scadenza della migrazione sono disponibili nella sezione [Sezione Scadenza migrazione utente](#user-migration-expiration).

Nella sezione successiva della scheda Stato di migrazione sono disponibili due barre di avanzamento. La prima barra di avanzamento mostra l’avanzamento del completamento della verifica e-mail dell’utente. La seconda barra di avanzamento mostra la progressione del completamento della migrazione degli utenti.

Successivamente, l’amministratore visualizzerà tre sezioni dello Stato.

La prima sezione riguarda lo stato di verifica e-mail degli utenti all’interno dell’abbonamento.

La seconda sezione riguarda lo stato di migrazione e attivazione degli utenti (ovvero migrazione e adesione al prodotto di Marketo Engage) all’interno dell’abbonamento.

La terza sezione riguarda lo stato di completamento della migrazione dell’abbonamento.

Verifica e-mail utente

Nella sezione Verifica e-mail utente, un amministratore può trovare lo stato corrente della verifica e-mail per gli utenti nell’abbonamento, prima della migrazione all’identità Adobe.

Un amministratore può visualizzare lo stato di verifica e-mail dell’abbonamento, la percentuale di utenti nell’abbonamento che hanno completato la verifica e-mail e il numero di utenti contrassegnati come ignorati. Lo stato viene segnalato in base allo stato della verifica e-mail di tutti gli utenti nell’abbonamento. L’amministratore può fare clic sul numero di utenti ignorati e passare alla scheda Migrazione utenti per visualizzarli.

L’e-mail di verifica può essere inviata nuovamente da un amministratore nelle schede Migrazione utenti della console di migrazione e Utente e ruoli dell’area Amministratore di Marketo, oppure dall’utente nelle Impostazioni account. Come le e-mail di invito dell’utente, il collegamento nell’e-mail di verifica scadrà tra 3 giorni. Ulteriori informazioni sulla verifica tramite e-mail sono disponibili nella community &lt;nation.marketo.com> e nella documentazione di verifica via e-mail &lt; https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/email-verification.html?lang=en>.

IMPORTANTE

Se un utente del Marketo Engage non verifica il proprio indirizzo e-mail, non può effettuare la migrazione a un Adobe ID e perderà l’accesso all’abbonamento a Marketo al termine della migrazione. Per recuperare l’accesso al termine della migrazione degli utenti, un amministratore di prodotto Marketo dovrà aggiungerli come nuovo utente.

Migrazione e attivazione degli utenti

Nella sezione Migrazione e attivazione utenti, un amministratore può trovare lo stato corrente della migrazione utente totale e l’adesione all’Adobe Identity Management System.

Un amministratore può visualizzare la percentuale di utenti nella sottoscrizione che sono stati trasferiti a un Adobe ID o contrassegnati come Ignorati. Lo stato viene segnalato sullo stato della migrazione di tutti gli utenti a un Adobe ID nell’abbonamento, oppure viene contrassegnato come Ignorato e non verrà migrato. Quando gli utenti vengono trasferiti e autorizzati al Marketo Engage, o saltati, questo stato viene aggiornato.

Conferma della migrazione

Nella sezione Conferma della migrazione, verrà richiesto a un amministratore di confermare il completamento della migrazione utente per l’abbonamento.

Una volta conteggiati tutti gli utenti della sottoscrizione (trasferiti o ignorati), verrà visualizzato il pulsante &quot;Completa migrazione&quot;.

SCHERMATA

L’amministratore che esegue la migrazione deve completare la conferma della migrazione facendo clic sul pulsante &quot;Completa migrazione&quot;. Verrà richiesto di confermare il completamento della migrazione.

SCHERMATA

Una volta confermato il completamento della migrazione utente, la console di migrazione verrà rimossa dal menu di navigazione Admin.

### Scadenza migrazione utenti {#user-migration-expiration}

Adobe richiede ai clienti di completare le migrazioni self-service entro 30 giorni. La migrazione degli utenti o il completamento della migrazione non verrà impedito agli amministratori se la data di scadenza è stata superata, ma potranno eseguire la migrazione solo su richiesta.  Se un amministratore ha bisogno di più tempo, può estendere la data di scadenza dell’abbonamento.

SCHERMATA

Facendo clic sul pulsante &quot;Estendi scadenza&quot;, la data verrà aggiornata a una settimana dopo. Un amministratore può estendere la scadenza fino a tre volte.

SCHERMATA

SCHERMATA

L’estensione per Adobe si verifica dopo che un cliente non completa la migrazione entro la data di scadenza.

### Scheda Migrazione utenti {#user-migration-tab}

La scheda Migrazione utenti fornisce agli amministratori gli strumenti necessari per avere il controllo completo della migrazione degli utenti.

Gli amministratori possono:

Attiva le e-mail di verifica per gli utenti non verificati tramite il pulsante &quot;Verifica e-mail&quot;

Salta la migrazione degli utenti se gli utenti sanno che l’amministratore non può/non deve verificare la loro e-mail o non deve essere migrata tramite il pulsante &quot;Salta migrazione&quot;

Eseguire la migrazione degli utenti selezionati su richiesta tramite il pulsante &quot;Esegui migrazione ora&quot;

Pianifica la migrazione degli utenti per gli utenti selezionati per una data specifica tramite il pulsante &quot;Pianifica migrazione&quot;

Esegui la migrazione di tutti gli utenti idonei su richiesta (non è necessaria alcuna selezione di utenti) tramite il pulsante &quot;Migra tutti gli utenti&quot;

SCHERMATA

Verifica e-mail

La verifica e-mail è necessaria per la migrazione di un utente a un Adobe ID. Se alcuni utenti non hanno verificato il proprio indirizzo e-mail e devono essere trasferiti, l’amministratore può attivare l’invio dell’e-mail di verifica all’utente. Selezionando un utente non verificato, si attiva il pulsante &quot;Verifica e-mail&quot;, a cui viene richiesto di inviare l’e-mail.

SCHERMATA

Quando l’amministratore fa clic sul pulsante &quot;Verifica e-mail&quot;, riceve una notifica dell’invio dell’e-mail.

SCHERMATA

Ignora e rimuovi migrazione utenti

Durante la migrazione degli utenti, è necessario eseguire o saltare la migrazione di tutti gli utenti. In base all&#39;Adobe, gli amministratori devono confermare che non verrà eseguita la migrazione di un utente e devono contrassegnare l&#39;utente come ignorato. In caso contrario, l’amministratore non sarà in grado di confermare il completamento della migrazione degli utenti. Al termine della migrazione, tutti gli utenti ignorati perderanno l’accesso a Marketo.

IMPORTANTE

Un amministratore deve ignorare tutti gli utenti con e-mail non verificate. Se alcuni utenti hanno verificato le e-mail, ma l’amministratore non desidera eseguirne la migrazione per alcun motivo, deve contrassegnarle come ignorate.

Per saltare un utente, l’amministratore può selezionare gli utenti desiderati. Il pulsante &quot;Ignora migrazione&quot; si attiva. Facendo clic sul pulsante &quot;Salta migrazione&quot;, la pagina si aggiorna e lo stato di verifica e migrazione dell’utente selezionato viene aggiornato a &quot;Ignorato&quot;.

SCHERMATA

Un amministratore può annullare il salto di un utente precedentemente ignorato, se è determinato che l’utente deve essere migrato.

Per non saltare un utente, l’amministratore può selezionare l’utente desiderato. Il pulsante &#39;Unskip Migration&#39; (Annulla migrazione) verrà attivato. Facendo clic sul pulsante &quot;Unskip Migration&quot; (Annulla migrazione), la pagina viene aggiornata.  Lo stato di verifica dell’utente selezionato verrà aggiornato al suo stato corrente, &quot;Verificato&quot; o &quot;Non verificato&quot;, e lo stato di migrazione dell’utente verrà aggiornato a &quot;Non avviato&quot;.

SCHERMATA

NOTA

Il pulsante &#39;Annulla migrazione&#39; sarà attivo solo se tutti gli utenti selezionati hanno uno stato di migrazione &#39;Ignorato&#39;.

Migrazione degli utenti Marketo agli ID Adobe

Per i clienti che desiderano un maggiore controllo durante il processo di migrazione, Marketo supporta un approccio self-service per gli abbonamenti con 75 o più utenti. Gli amministratori di prodotto Marketo potranno selezionare gli utenti da migrare in batch o tutti gli utenti idonei contemporaneamente. Una volta selezionati gli utenti, gli amministratori possono scegliere &quot;Migra ora&quot; o &quot;Pianifica migrazione&quot; per una data successiva, offrendo agli amministratori la massima flessibilità e il controllo su quali utenti vengono migrati e quando. Agli amministratori viene inoltre offerta l’opzione &quot;Migra tutti gli utenti&quot; in un abbonamento.

Ad esempio, un amministratore può selezionare un gruppo di utenti &quot;avanzati&quot; che desidera migrare per primi. Una volta completate correttamente le migrazioni degli utenti, è possibile selezionare gruppi diversi in base a elementi quali l’area di lavoro, la funzione aziendale o il ruolo per eseguire ulteriori migrazioni batch degli utenti in base a. In alternativa, potrebbe decidere di eseguire la migrazione di tutti gli altri utenti degli abbonamenti dopo il completamento del primo batch. L’obiettivo è fornire agli utenti la massima flessibilità nella distribuzione degli ID Adobi.

Tutte le migrazioni degli utenti avvengono contemporaneamente e dovrebbero essere completate correttamente entro sessanta secondi. Durante la migrazione di un utente specifico, l’utente potrebbe perdere l’accesso per un massimo di 1 minuto e ciò solo se ha effettuato l’accesso all’applicazione. Al termine della migrazione utente, l’utente riceverà un’e-mail su come accedere al Marketo Engage con un’identità Adobe. L’utente deve accettare l’invito tramite il collegamento del pulsante nell’e-mail. Dopo aver accettato l’invito, l’utente deve accedere con un Adobe ID. Le istruzioni su come accedere al Marketo Engage con un Adobe ID sono disponibili qui. &lt; https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/user-sign-in-with-adobe-id.html>

SCHERMATA

Le migrazioni degli utenti vengono elaborate in modo indipendente; pertanto, se una migrazione non riesce, Adobe continuerà a elaborare le migrazioni degli altri utenti. Se si verifica un errore di migrazione utente, non è richiesta alcuna azione da parte di un amministratore. Il team ingegneristico Adobe sarà al lavoro per risolvere il problema il prima possibile. L’amministratore riceverà una notifica e-mail relativa all’errore e verrà avvisato che l’Adobe è in grado di risolvere il problema immediatamente. Se la migrazione di un utente non riesce e l’utente è connesso al Marketo Engage, potrebbe perdere l’accesso per un massimo di 2 minuti, durante i nuovi tentativi di migrazione.  Se la migrazione di un utente non riesce, l’utente può continuare ad accedere al Marketo Engage con la propria identità Marketo fino a quando non riceve una notifica e-mail di avvenuta migrazione e viene invitato ad accedere con un Adobe ID.

SCHERMATA

Migra ora

Un amministratore può selezionare uno o più utenti per la migrazione su richiesta. Questo attiverà immediatamente la migrazione degli utenti. Per eseguire la migrazione di uno o più utenti, l&#39;amministratore seleziona gli utenti desiderati e viene attivato il pulsante &quot;Esegui migrazione ora&quot;.

SCHERMATA

NOTA

Il pulsante &quot;Esegui migrazione ora&quot; sarà attivo solo se tutti gli utenti selezionati dispongono di uno stato di verifica &quot;Verificato&quot;.

Facendo clic sul pulsante Migra ora, all&#39;amministratore verrà richiesto di confermare la migrazione degli utenti selezionati. Una volta confermata dall’amministratore, le migrazioni degli utenti inizieranno l’elaborazione il prima possibile.

SCHERMATA

Pianifica migrazione

Un amministratore può selezionare uno o più utenti per pianificare la migrazione in una data successiva. Per pianificare la migrazione per uno o più utenti, l’amministratore seleziona gli utenti desiderati e viene attivato il pulsante &quot;Pianifica migrazione&quot;.

SCHERMATA

NOTA

Il pulsante &quot;Pianifica migrazione&quot; sarà attivo solo se tutti gli utenti selezionati dispongono di uno stato di verifica &quot;Verificato&quot;.

Facendo clic sul pulsante &quot;Pianifica migrazione&quot;, all’amministratore viene richiesto di selezionare la data di migrazione desiderata per gli utenti selezionati. L’amministratore può selezionare solo date precedenti alla data di scadenza della migrazione della sottoscrizione. Una volta confermata la conferma da parte dell’amministratore, l’elaborazione delle migrazioni utente verrà pianificata per la data selezionata.

SCHERMATA

NOTA

Tutti gli abbonamenti Marketo con fuso orario negli Stati Uniti verranno migrati a partire dalla mezzanotte (ora standard del Pacifico) della data di inizio della migrazione. La migrazione degli utenti per tutti gli altri abbonamenti inizierà alla mezzanotte del fuso orario specificato per l’abbonamento.

Migra tutti gli utenti

Un amministratore può scegliere di eseguire la migrazione di tutti gli utenti idonei in un abbonamento in qualsiasi momento. Questo attiverà immediatamente la migrazione degli utenti idonei. Gli utenti idonei sono quelli con e-mail verificate, che non sono ancora stati trasferiti.

SCHERMATA

Facendo clic sul pulsante &quot;Migra tutti gli utenti&quot;, all’amministratore verrà richiesto di confermare la migrazione di tutti gli utenti idonei. Una volta confermata dall’amministratore, le migrazioni degli utenti inizieranno l’elaborazione il prima possibile.

SCHERMATA
