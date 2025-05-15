---
description: Abbonamento a Marketo e migrazione degli utenti al Adobe Admin Console - Documentazione di Marketo - Documentazione del prodotto
title: Abbonamento a Marketo e migrazione degli utenti a Adobe Admin Console
exl-id: 91e7b56b-2563-4986-a55c-f9760ea88b05
feature: Marketo with Adobe Identity
source-git-commit: 8b44c3b2ccabeb796a3a8f7775848a5063279076
workflow-type: tm+mt
source-wordcount: '1571'
ht-degree: 0%

---

# Abbonamento a Marketo e migrazione degli utenti a Adobe Admin Console {#understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console}

Adobe migliora il modo in cui gestisci gli abbonamenti e gli utenti Adobe Marketo Engage, aumentando la produttività per te e la tua organizzazione. Come parte di questa modifica, Adobe sta eseguendo la migrazione delle sottoscrizioni e degli utenti Marketo Engage al Adobe Admin Console. Si tratta di una migrazione necessaria e non influirà su flussi di lavoro, contenuti, integrazioni o risorse di marketing.

>[!TIP]
>
>Scopri come utilizzare Adobe Admin Console per gestire i diritti Adobe in tutta l&#39;organizzazione con la [Guida per l&#39;amministratore di Enterprise e Team](https://helpx.adobe.com/it/enterprise/admin-guide.html){target="_blank"}.

## Cosa sta cambiando? {#what-is-changing}

Come parte della migrazione, la gestione dell’abbonamento e degli utenti passerà dall’applicazione Marketo a Adobe Admin Console.

* **Gli amministratori di sistema gestiranno gli abbonamenti in Adobe Admin Console**. Visualizza tutti i prodotti Adobe in un’unica console.

* **Gli amministratori di prodotto gestiranno gli utenti e il loro accesso in Adobe Admin Console**. Aggiungi e rimuovi utenti per tutti gli abbonamenti Adobe. Adobe Admin Console non supporta la scadenza dell’accesso basata sull’utente. Gli utenti che dispongono di un accesso a Marketo Engage la cui scadenza è pianificata per il periodo successivo alla migrazione continueranno a ricevere la migrazione e l’accesso non scadrà. Dopo la migrazione, devono essere rimossi manualmente il (o prima) della data di scadenza desiderata.

* **Gli utenti accederanno con Adobe Identity**. Adobe eseguirà la migrazione degli utenti esistenti a Adobe Admin Console. Gli utenti effettueranno l’accesso ai propri abbonamenti Marketo utilizzando la nuova identità Adobe, un Adobe ID o un Federated ID Adobe (SSO).

* **Gli URL avranno un aspetto diverso dopo la migrazione**. Marketo Engage passerà da experience.adobe.com a Adobe Experience Cloud e gli URL saranno nel seguente formato: `https://experience.adobe.com/#/@tenantID/so:XXX-XXX-XXX/marketo-engage/classic/` (gli XXX rappresentano l&#39;ID Munchkin e @tenantID proviene dall&#39;organizzazione Adobe). Per evitare interruzioni dell&#39;accesso a Marketo Engage, dovrai collaborare con il tuo team IT per inserire nell&#39;elenco Consentiti tutti i domini Adobe elencati [nella parte superiore di questo articolo](/help/marketo/getting-started/initial-setup/configure-protocols-for-marketo.md){target="_blank"}.

I numeri ID delle risorse rimangono invariati. I collegamenti e i segnalibri precedenti per le risorse Marketo Engage nel dominio engage-xx.marketo.com _continueranno a funzionare_. Tuttavia, devi prima accedere all’istanza di Marketo Engage per l’URL a cui stai navigando. Ad esempio, per passare a un segnalibro per una campagna avanzata nell’istanza con Munchkin ID 123-ABC-456, devi prima accedere all’istanza Marketo Engage con Munchkin ID 123-ABC-456.

Anche se non pianificato, il lavoro di sviluppo futuro può interrompere questa funzione di reindirizzamento. Per evitare interruzioni impreviste, si consiglia di aggiornare i segnalibri il prima possibile.

## Cosa non cambia? {#what-is-not-changing}

* **Non è stata modificata la modalità di gestione di tutte le altre funzionalità** all&#39;interno dell&#39;applicazione Marketo Engage stessa, inclusa la gestione di funzionalità, ruoli utente, aree di lavoro, funzionalità e comportamento. La gestione degli utenti locali (solo API) rimane nella scheda _Utenti e ruoli_ nell&#39;area di amministrazione di Marketo.

## Timeline del Percorso di migrazione {#migration-journey-timeline}

Adobe eseguirà prima la migrazione delle sottoscrizioni Marketo Engage a Adobe Admin Console, quindi eseguirà la migrazione di tutti gli utenti esistenti con indirizzi e-mail verificati. Se sei un amministratore di sistema o un amministratore di prodotto Marketo, riceverai e-mail che ti guidano attraverso il percorso di migrazione. Ecco una cronologia di ciò che puoi aspettarti:

![](assets/understanding-marketo-subscription-and-user-migration-1.png){width="800" zoomable="yes"}

### Migrazione abbonamento completata {#subscription-migration-complete}

Gli amministratori di sistema riceveranno un’e-mail al termine della migrazione dell’abbonamento a Adobe Admin Console.

Per ridurre al minimo l’impatto sugli utenti di Marketo, gli amministratori di sistema potrebbero dover completare alcuni passaggi obbligatori prima di avviare la migrazione degli utenti:

* Se gli utenti di Marketo al momento effettuano l&#39;accesso con SSO, ti verrà richiesto di impostare SSO su Adobe Admin Console in modo che gli utenti possano continuare ad accedere con SSO. Se gli utenti di Marketo al momento non utilizzano l’SSO, ma desideri configurarlo su Adobe Admin Console, puoi farlo a questo punto nel percorso di migrazione.

* Se gestisci già altri prodotti Adobe nel tuo Adobe Admin Console, Adobe potrebbe richiedere il consenso per eseguire automaticamente la migrazione degli utenti alla console esistente. Per accedere alla pagina del consenso, fai clic sul pulsante &quot;Inizia&quot; nell’e-mail.

Al momento non vi sono modifiche alla gestione degli utenti. Anche se i prodotti Marketo vengono visualizzati in Admin Console, gli amministratori di Marketo continueranno a gestire gli utenti nell’area di amministrazione di Marketo e gli utenti continueranno ad accedere con la propria identità Marketo fino a quando la migrazione degli utenti non sarà completata. Durante questo periodo, i prodotti Marketo non possono essere amministrati in Admin Console finché non inizia la migrazione degli utenti. Ciò include l’istanza Dynamic Chat associata all’abbonamento.

>[!NOTE]
>
>Se al momento non utilizzi l’SSO ma stai pensando di implementarlo, ti consigliamo di farlo prima che si verifichi la migrazione degli utenti. Se desideri implementare Single Sign On e il tuo abbonamento è stato effettuato a Adobe Identity senza SSO implementato nell&#39;organizzazione Adobe, invia un ticket al [Supporto Marketo](https://nation.marketo.com/){target="_blank"} e specifica l&#39;argomento come &quot;Marketo su Admin Console, implementazione di SSO&quot;.

### Pianifica migrazione utenti {#schedule-user-migration}

Una volta che l’amministratore di sistema avrà soddisfatto i prerequisiti descritti nella sezione precedente, Adobe pianificherà automaticamente la migrazione utente con 30 giorni di anticipo e comunicherà con gli amministratori di prodotto Marketo per gestire la migrazione degli utenti.

Gli amministratori di prodotto Marketo:

* Ricevi un’e-mail con la data di inizio della migrazione utente pianificata, 30 giorni prima.

* Accedi a Marketo Migration Console, che si trova nell’area di amministrazione di Marketo, e consente di modificare la data di migrazione di un abbonamento.

>[!NOTE]
>
>A causa della complessità della migrazione, le modifiche della data sono limitate a non più di 30 giorni oltre la data pianificata. Invia un&#39;e-mail a `marketocares@marketo.com` se hai bisogno di una data successiva.

* Visualizza un banner in Il mio Marketo che mostra un conto alla rovescia per la data di inizio della migrazione utente.

* Ricevi un messaggio e-mail di promemoria il giorno precedente alla data di inizio della migrazione utente.

### Prepara utenti per il giorno della migrazione {#prepare-users-for-migration-day}

In qualità di amministratore di prodotto Marketo, sei invitato a garantire che tutti gli utenti siano preparati per la migrazione.

* Controlla lo stato [verifica e-mail](/help/marketo/product-docs/administration/users-and-roles/email-verification.md){target="_blank"} per tutti gli utenti nell&#39;area di amministrazione di Marketo. Incoraggia gli utenti che non hanno verificato il proprio indirizzo e-mail a farlo e aiuta gli utenti a risolvere eventuali problemi durante il completamento del processo di verifica.

* Cerca nella tua casella di posta in arrivo le notifiche utente &quot;bloccate&quot;. Consiglia agli utenti che sono stati bloccati di reimpostare la password di ristabilire l’accesso a Marketo Engage prima del giorno della migrazione.

* Prepara tutti gli utenti per la prossima migrazione ad Adobe Identity.

>[!IMPORTANT]
>
>Se un utente di Marketo Engage non verifica il proprio indirizzo e-mail o è bloccato al momento della migrazione dell’utente, non verrà effettuata la migrazione a un Adobe ID e perderà l’accesso all’abbonamento a Marketo al termine della migrazione per l’abbonamento. Per recuperare l’accesso, un amministratore di prodotto Marketo deve aggiungerli come nuovo utente.

### Cosa aspettarsi il giorno della migrazione {#what-to-expect-on-migration-day}

Tutti gli abbonamenti Marketo con fuso orario negli Stati Uniti verranno migrati a partire dalla mezzanotte (ora standard del Pacifico) della data di inizio della migrazione. La migrazione degli utenti per tutti gli altri abbonamenti inizierà alla mezzanotte del fuso orario specificato per l’abbonamento.

**Adobe eseguirà automaticamente prima la migrazione degli amministratori di Marketo (con un ruolo di amministratore standard)**. Quando gli amministratori di Marketo vengono trasferiti ad Adobe Identity con il ruolo di amministratore di prodotto Admin Console, viene loro assegnato il ruolo di amministratore di prodotto Adobe all’interno dell’applicazione Marketo insieme a tutti gli altri ruoli che avevano in precedenza.

**Se la sottoscrizione a Marketo non dispone di SSO in Marketo e/o nell&#39;organizzazione Adobe**, Adobe eseguirà automaticamente la migrazione degli altri utenti. Questo flusso di lavoro mira a fornire il massimo livello di automazione per ridurre al minimo il sovraccarico per gli utenti di Adobe Marketo. Non è richiesta alcuna azione da parte tua per eseguire la migrazione.

**Se l&#39;abbonamento a Marketo dispone di SSO in Marketo e/o nell&#39;organizzazione Adobe**, gli amministratori di Marketo avranno accesso all&#39;area Self-Service User Migration della console di migrazione di Marketo, che si trova nell&#39;area di amministrazione di Marketo. Per coloro che necessitano di un maggiore controllo durante il processo di migrazione degli utenti, gli amministratori di Marketo potranno iniziare a selezionare gli utenti da migrare in batch o tutti in una sola volta. Una volta selezionati gli utenti, gli amministratori possono scegliere &quot;Migra ora&quot; o &quot;Pianifica migrazione&quot; per una data successiva, offrendo agli amministratori flessibilità e controllo massimi su quali utenti vengono migrati quando.

>[!NOTE]
>
>Non si verificherà alcuna perdita di accesso al prodotto durante la migrazione degli utenti. Se un utente ha eseguito l’accesso durante il periodo di migrazione, verrà disconnesso e gli verrà richiesto di eseguire di nuovo l’accesso in pochi minuti tramite Adobe Identity al termine della migrazione. L’utente deve accettare l’invito facendo clic sul collegamento nell’e-mail per la licenza inviata al termine di una migrazione utente eseguita correttamente.

Durante la migrazione, gli utenti riceveranno un’e-mail da Adobe per informarli della modifica del modo in cui accedono a Marketo. Gli utenti **devono** accettare un invito ad accedere con Adobe Identity per la prima volta, effettuando l&#39;accesso con un Adobe ID esistente o impostando un nuovo Adobe ID con lo stesso indirizzo e-mail.

Ulteriori informazioni sono disponibili in [Migrazione ad Adobe Identity](/help/marketo/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity.md){target="_blank"}, [Accesso utente con Adobe](/help/marketo/product-docs/administration/marketo-with-adobe-identity/user-sign-in-with-adobe-id.md){target="_blank"} e [Domande frequenti su Adobe Identity Management](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}.

## Migrazione utente completata {#user-migration-complete}

Una volta effettuata la migrazione, Adobe invierà una notifica a tutti gli amministratori di sistema e di prodotto tramite e-mail. Al momento, tutti gli utenti di Marketo per tale abbonamento accederanno a Marketo utilizzando Adobe Identity e gli amministratori di prodotto gestiranno gli utenti solo su Adobe Admin Console.

## Ottieni supporto {#get-support}

Per ulteriore supporto relativo all&#39;abbonamento o alla migrazione degli utenti, inviare un messaggio e-mail a `marketocares@marketo.com`.

>[!MORELIKETHIS]
>
>* [Migrazione alla panoramica di Adobe Identity](/help/marketo/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/migrating-to-adobe-identity.md){target="_blank"}
>* [Accesso utente con Adobe](/help/marketo/product-docs/administration/marketo-with-adobe-identity/user-sign-in-with-adobe-id.md){target="_blank"}
>* [Domande frequenti su Adobe Identity Management](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}
>* [Esercitazione sulla migrazione ad Adobe Identity Management](https://experienceleague.adobe.com/en/docs/marketo-learn/tutorials/fundamentals/migrating-to-adobe-identity-management){target="_blank"}
