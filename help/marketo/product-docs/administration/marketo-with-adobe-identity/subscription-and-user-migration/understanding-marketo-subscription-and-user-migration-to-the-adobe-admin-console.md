---
description: Cosa cambia quando gli abbonamenti e gli utenti migrano a Adobe Admin Console, inclusi i ruoli Amministratore di sistema e Amministratore di prodotto, accesso con Adobe Identity, URL e timeline di migrazione.
title: Informazioni sull’abbonamento a Marketo e sulla migrazione degli utenti ad Adobe Admin Console
exl-id: 91e7b56b-2563-4986-a55c-f9760ea88b05
feature: Marketo with Adobe Identity
source-git-commit: e894ece3a643113fd3e1d8df9f8addefea5553f5
workflow-type: tm+mt
source-wordcount: '1584'
ht-degree: 98%

---

# Informazioni sull’abbonamento a Marketo e sulla migrazione degli utenti ad Adobe Admin Console {#understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console}

Adobe sta migliorando il modo di gestire gli abbonamenti e gli utenti Adobe Marketo Engage, aumentando la produttività per te e per la tua organizzazione. Come parte di questa modifica, Adobe sta migrando gli abbonamenti e gli utenti Marketo Engage ad Adobe Admin Console. Si tratta di una migrazione necessaria che non avrà alcun impatto su flussi di lavoro, contenuti, integrazioni o risorse di marketing.

>[!TIP]
>
>Scopri come utilizzare Adobe Admin Console per gestire le autorizzazioni di utilizzo dei prodotti Adobe per l’intera organizzazione con la [Guida per l’amministratore Enterprise e Team](https://helpx.adobe.com/it/enterprise/admin-guide.html){target="_blank"}.

## Cosa cambia? {#what-is-changing}

Come parte della migrazione, la gestione dell’abbonamento e degli utenti passerà dall’applicazione Marketo ad Adobe Admin Console.

* **Gli amministratori di sistema gestiranno gli abbonamenti in Adobe Admin Console**. Tutti i tuoi prodotti Adobe si troveranno in un’unica console.

* **Gli amministratori di prodotto gestiranno gli utenti e le loro autorizzazioni di accesso in Adobe Admin Console**. Puoi aggiungere e rimuovere gli utenti per tutti i tuoi abbonamenti Adobe. Adobe Admin Console non supporta la scadenza dell’accesso basata sull’utente. Gli utenti con accesso a Marketo Engage, la cui scadenza è prevista dopo la migrazione, saranno comunque migrati e avranno accesso senza scadenza. Dopo la migrazione, dovranno essere rimossi manualmente entro la data di scadenza desiderata.

* **Gli utenti eseguiranno l’accesso con Adobe Identity**. Adobe eseguirà la migrazione degli utenti esistenti ad Adobe Admin Console. Gli utenti potranno accedere al proprio abbonamento Marketo utilizzando la nuova Adobe Identity: un Adobe ID o un Adobe Federated ID (SSO).

* **Gli URL avranno un aspetto diverso dopo la migrazione**. Marketo Engage passerà dall’essere fornito tramite experience.adobe.com ad Adobe Experience Cloud e gli URL saranno nel seguente formato: `https://experience.adobe.com/#/@tenantID/so:XXX-XXX-XXX/marketo-engage/classic/` (dove gli XXX rappresentano l’ID Munchkin e @tenantID proviene dalla tua organizzazione Adobe). Per evitare interruzioni all’accesso a Marketo Engage, dovrai collaborare con il tuo team IT per inserire nell’elenco Consentiti tutti i domini Adobe elencati [all’inizio di questo articolo](/help/marketo/getting-started/initial-setup/configure-protocols-for-marketo.md){target="_blank"}.

I numeri ID delle risorse rimangono invariati. I collegamenti e i segnalibri precedenti per le risorse Marketo Engage nel dominio engage-xx.marketo.com _continueranno_ a funzionare. Tuttavia, devi prima accedere all’istanza di Marketo Engage per l’URL di destinazione. Ad esempio, se usi un segnalibro per passare a una campagna avanzata nell’istanza con ID Munchkin 123-ABC-456, devi prima accedere all’istanza Marketo Engage con ID Munchkin 123-ABC-456.

Anche se non è previsto, è possibile che sviluppi futuri compromettano questa funzione di reindirizzamento. Per evitare interruzioni impreviste, si consiglia di aggiornare i segnalibri il prima possibile.

## Cosa non cambia? {#what-is-not-changing}

* All’interno dell’applicazione Marketo Engage stessa **non è stato cambiato il modo in cui si gestiscono tutte le altre funzionalità**, inclusa la gestione di funzioni, ruoli utente, aree di lavoro, funzionalità e comportamento. La gestione locale degli utenti (solo API) rimane nella scheda _Utenti e ruoli_ nell’area di amministrazione di Marketo.

## Timeline del percorso di migrazione {#migration-journey-timeline}

Adobe eseguirà prima la migrazione degli abbonamenti Marketo Engage ad Adobe Admin Console, quindi la migrazione di tutti gli utenti esistenti con indirizzi e-mail verificati. Se sei un amministratore di sistema o un amministratore del prodotto Marketo, riceverai e-mail che ti guidano nel percorso di migrazione. Ecco una timeline di ciò che puoi aspettarti:

![](assets/understanding-marketo-subscription-and-user-migration-1.png){width="800" zoomable="yes"}

### Migrazione abbonamento completata {#subscription-migration-complete}

Una volta completata la migrazione dell’abbonamento ad Adobe Admin Console, gli amministratori di sistema riceveranno un’e-mail.

Per ridurre al minimo l’impatto sugli utenti di Marketo, gli amministratori di sistema potrebbero dover completare alcuni passaggi obbligatori prima di avviare la migrazione degli utenti:

* Se gli utenti di Marketo al momento effettuano l’accesso tramite SSO, ti verrà richiesto di impostare SSO in Adobe Admin Console in modo che gli utenti possano continuare ad accedere con SSO. Se al momento gli utenti di Marketo non utilizzano l’SSO, ma desideri configurarlo in Adobe Admin Console, puoi farlo a questo punto del percorso di migrazione.

* Se gestisci già altri prodotti Adobe in Adobe Admin Console, Adobe potrebbe richiederti il consenso alla migrazione automatica degli utenti alla console esistente. Per accedere alla pagina del consenso, fai clic sul pulsante “Inizia” nell’e-mail.

Al momento la gestione degli utenti resta invariata. Anche se i prodotti Marketo vengono visualizzati in Admin Console, gli amministratori di Marketo continueranno a gestire gli utenti nell’area di amministrazione di Marketo e gli utenti continueranno ad accedere con la propria identità Marketo fino a quando la migrazione degli utenti non sarà stata completata. Durante questo periodo, i prodotti Marketo non possono essere amministrati in Admin Console finché non inizia la migrazione degli utenti. Questo vale anche per l’istanza di Dynamic Chat associata all’abbonamento.

>[!NOTE]
>
>Se non utilizzi ancora l’SSO ma stai pensando di implementarlo, ti consigliamo di farlo prima che si verifichi la migrazione degli utenti. Se desideri implementare il Single Sign On (SSO) e il tuo abbonamento è stato inserito in Adobe Identity senza che l’SSO sia stato implementato nell’organizzazione Adobe, invia un ticket all’[assistenza Marketo](https://nation.marketo.com/){target="_blank"} specificando l’argomento “Marketo in Admin Console, implementing SSO”.

### Pianificare la migrazione degli utenti {#schedule-user-migration}

Una volta che l’amministratore di sistema avrà completato i prerequisiti descritti nella sezione precedente, Adobe pianificherà automaticamente la migrazione degli utenti con 30 giorni di anticipo e comunicherà con gli amministratori di prodotto Marketo per gestire tale migrazione.

Gli amministratori di prodotto Marketo:

* Riceveranno un’e-mail con la data di inizio della migrazione degli utenti pianificata, con 30 giorni di anticipo.

* Potranno accedere alla console per la migrazione di Marketo, nell’area di amministrazione di Marketo, in cui potranno modificare la data di migrazione di un abbonamento.

>[!NOTE]
>
>A causa della complessità della migrazione, le modifiche alla data sono limitate a non più di 30 giorni oltre la data pianificata. Se hai bisogno di una data successiva, invia un’e-mail a `marketocares@marketo.com`.

* Visualizzeranno un banner in My Marketo con un conto alla rovescia per la data di inizio della migrazione degli utenti.

* Riceveranno un messaggio e-mail di promemoria il giorno precedente alla data di inizio della migrazione degli utenti.

### Preparare gli utenti al giorno della migrazione {#prepare-users-for-migration-day}

In qualità di amministratore di prodotto Marketo, dovrai assicurarti che tutti gli utenti siano preparati al giorno della migrazione.

* Controlla lo stato di [verifica e-mail](/help/marketo/product-docs/administration/users-and-roles/email-verification.md){target="_blank"} per tutti gli utenti nell’area di amministrazione di Marketo. Incoraggia gli utenti che non hanno verificato il proprio indirizzo e-mail a farlo, e aiutali a risolvere eventuali problemi riscontrati durante il processo di verifica.

* Cerca nella tua casella di posta in entrata eventuali notifiche relative agli utenti “bloccati”. Consiglia agli utenti che sono stati bloccati di ripristinare la password in modo da ristabilire l’accesso a Marketo Engage prima del giorno della migrazione.

* Prepara tutti gli utenti alla prossima migrazione ad Adobe Identity.

>[!IMPORTANT]
>
>Se un utente di Marketo Engage non verifica il proprio indirizzo e-mail o è bloccato al momento della migrazione degli utenti, non verrà migrato a un Adobe ID e, una volta completata la migrazione dell’abbonamento, non potrà accedere all’abbonamento Marketo. Per ottenere di nuovo l’accesso, dovrà essere aggiunto come nuovo utente da un amministratore di prodotto Marketo.

### Cosa aspettarsi il giorno della migrazione {#what-to-expect-on-migration-day}

Tutti gli abbonamenti Marketo con fuso orario degli Stati Uniti verranno migrati a partire dalla mezzanotte, ora standard del Pacifico, della data di inizio della migrazione. La migrazione degli utenti per tutti gli altri abbonamenti inizierà alla mezzanotte nel fuso orario specificato per l’abbonamento.

**Adobe eseguirà prima la migrazione automatica degli amministratori di Marketo (con un ruolo di amministratore standard)**. Quando gli amministratori di Marketo vengono trasferiti ad Adobe Identity con un ruolo di amministratore di prodotto Admin Console, viene loro assegnato il ruolo di amministratore di prodotto Adobe all’interno dell’applicazione Marketo, insieme a eventuali altri ruoli che avevano in precedenza.

**Se l’abbonamento a Marketo non dispone di SSO in Marketo e/o nell’organizzazione Adobe**, Adobe eseguirà automaticamente la migrazione degli altri utenti. Questo flusso di lavoro mira a fornire il massimo livello di automazione per ridurre al minimo il lavoro necessario per gli utenti di Adobe Marketo. Non è richiesta alcuna azione da parte tua per eseguire la migrazione.

**Se l’abbonamento a Marketo dispone di SSO in Marketo e/o nell’organizzazione Adobe**, gli amministratori di Marketo avranno accesso all’area Self-Service User Migration della console di migrazione di Marketo, nell’area di amministrazione di Marketo. Per coloro che necessitano di un maggiore controllo durante il processo di migrazione degli utenti, gli amministratori di Marketo potranno iniziare a selezionare gli utenti da migrare in batch o tutti insieme. Una volta selezionati gli utenti, gli amministratori possono scegliere tra due opzioni, per eseguire subito la migrazione o pianificarla per una data successiva. Queste offrono agli amministratori massima flessibilità e il pieno controllo su quali utenti migrare e quando eseguire la migrazione.

>[!NOTE]
>
>Durante la migrazione degli utenti, non si verificherà alcuna perdita di accesso al prodotto. Se un utente è attualmente connesso al momento in cui avviene la migrazione, verrà disconnesso e gli verrà richiesto di accedere nuovamente entro pochi minuti tramite Adobe Identity, una volta completata la migrazione. L’utente deve quindi accettare l’invito facendo clic sul collegamento nell’e-mail relativa alla licenza, inviata al termine di una migrazione di utenti completata correttamente.

Man mano che gli utenti vengono migrati, riceveranno un’e-mail da Adobe che li informerà della nuova modalità di accesso per Marketo. Gli utenti **devono** accettare un invito per accedere tramite Adobe Identity per la prima volta, effettuando l’accesso con un Adobe ID esistente oppure impostando un nuovo Adobe ID con lo stesso indirizzo e-mail.

Ulteriori informazioni sono disponibili in [Migrazione ad Adobe Identity](/help/marketo/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity.md){target="_blank"}, [Accesso degli utenti con Adobe](/help/marketo/product-docs/administration/marketo-with-adobe-identity/user-sign-in-with-adobe-id.md){target="_blank"} e [Domande frequenti sulla gestione di Adobe Identity](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}.

## Migrazione degli utenti completata {#user-migration-complete}

Una volta completata la migrazione di tutti gli amministratori e gli utenti, Adobe invierà una notifica e-mail a tutti gli amministratori di sistema e di prodotto. A questo punto, tutti gli utenti di Marketo per tale abbonamento potranno accedere a Marketo utilizzando Adobe Identity e gli amministratori di prodotto potranno gestire gli utenti solo in Adobe Admin Console.

## Ricevere assistenza {#get-support}

Per ulteriore assistenza in merito all’abbonamento o alla migrazione degli utenti, invia un messaggio e-mail a `marketocares@marketo.com`.

>[!MORELIKETHIS]
>
>* [Panoramica della migrazione ad Adobe Identity](/help/marketo/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity.md){target="_blank"}
>* [Accesso degli utenti con Adobe ID](/help/marketo/product-docs/administration/marketo-with-adobe-identity/user-sign-in-with-adobe-id.md){target="_blank"}
>* [Domande frequenti su Adobe Identity Management](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}
>* [Tutorial sulla migrazione ad Adobe Identity Management](https://experienceleague.adobe.com/it/docs/marketo-learn/tutorials/fundamentals/migrating-to-adobe-identity-management){target="_blank"}
