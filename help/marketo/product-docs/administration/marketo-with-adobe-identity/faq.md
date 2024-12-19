---
description: Domande frequenti su Adobe Identity Management - Documentazione Marketo - Documentazione del prodotto
title: Domande frequenti su Adobe Identity Management
feature: Marketo with Adobe Identity
exl-id: 2401def7-1696-4d77-a8a3-96c490517121
source-git-commit: ec0fcba763a50348c3424a1ba33c5fc700093c68
workflow-type: tm+mt
source-wordcount: '1521'
ht-degree: 0%

---

# Domande frequenti su Adobe Identity Management {#adobe-identity-management-faq}

**Che cos&#39;è Adobe Identity?**

Adobe Identity Management System è costituito da tre componenti.

* [!DNL Adobe Identity Service]: gestisce l&#39;autenticazione e la convalida dell&#39;utente finale, inclusi la federazione e il Single Sign-On (SSO) di runtime.

* Adobe Admin Console: l’Admin Console fornisce una posizione centrale per la gestione dei diritti Adobe in tutta l’organizzazione. Gestisce la gestione degli utenti, il servizio cloud, il diritto alla licenza del desktop, la configurazione della federazione e fornisce funzioni di sicurezza per la prevenzione della perdita di dati.

* Adobe User Management API (UMAPI): consente alle organizzazioni di gestire gli utenti e le autorizzazioni Enterprise in Adobe Admin Console a livello di API.

**Quando verranno integrate con IMS le sottoscrizioni di Marketo Engage esistenti?**

Gli abbonamenti al Marketo Engage esistenti sono attualmente in fase di migrazione ad Adobe IMS per qualsiasi evento di vendita, che include rinnovi, eventi di riappalto e/o supplementi. Le migrazioni al di fuori di un evento di vendita sono ora supportate a ottobre 2024.

**Dopo la migrazione, gli URL di Marketo Engage rimarranno invariati?**

No. Gli URL avranno un aspetto diverso dopo la migrazione.

**C&#39;è qualcosa da fare per prepararci alla modifica dell&#39;URL?**

Sì.  Dopo la migrazione, il Marketo Engage passerà da experience.adobe.com a Adobe Experience Cloud. Per evitare interruzioni dell&#39;accesso al Marketo Engage, dovrai collaborare con il tuo team IT per inserire nell&#39;elenco Consentiti tutti i domini Adobe elencati [nella parte superiore di questo articolo](/help/marketo/getting-started/initial-setup/configure-protocols-for-marketo.md){target="_blank"}.

I collegamenti e i segnalibri precedenti per le risorse di Marketo Engage nel dominio engage-xx.marketo.com _funzioneranno_. Tuttavia, devi prima accedere all’istanza di Marketo Engage per l’URL a cui stai navigando. Ad esempio, per passare a un segnalibro per una campagna avanzata nell’istanza con Munchkin ID 123-ABC-456, devi prima accedere all’istanza di Marketo Engage con Munchkin ID 123-ABC-456.

**Qual è la differenza tra un amministratore di prodotto Adobe e un amministratore di Marketo Engage?**

* L’amministratore di prodotto Adobe è un nuovo ruolo nella piattaforma Marketo.
* Il ruolo di amministratore di prodotto di Adobe viene concesso agli utenti aggiunti come amministratore di prodotto in Adobe Admin Console
* L’amministratore del prodotto Adobe è un ruolo di sola lettura e non può essere modificato o eliminato dal Marketo Engage.
* L’amministratore di prodotto Adobe dispone degli stessi diritti e privilegi di un amministratore Marketo standard.
* Il ruolo di amministratore di Marketo Engage è ancora amministratore e viene concesso a un utente del Marketo Engage.

**Sono state apportate modifiche al supporto client API per la gestione utenti?**

Sì.  Gli utenti che hanno effettuato l’onboarding in Adobe IMS non possono utilizzare tutte le API di gestione utenti di Marketo esistenti. Per le azioni di invito, aggiornamento ed eliminazione degli utenti, è necessario utilizzare le [API IMS](https://www.adobe.io/apis/experienceplatform/umapi-new.html){target="_blank"} di Adobe. Per la gestione dei ruoli, si applicano ancora le API di gestione utenti di Marketo. Inoltre, non vi sono altre modifiche al supporto client API REST di Marketo.

**A chi rivolgerci per richiedere assistenza se siamo integrati con IMS?**

* Migrazione pre-utente: casi di supporto dei file in [Marketing Nation Community](https://nation.marketo.com/t5/support/ct-p/Support) o e-mail `customercare@marketo.com`.

* Migrazione post-utente: casi di supporto file in [Marketing Nation Community](https://nation.marketo.com/t5/support/ct-p/Support) o e-mail `customercare@marketo.com`.

* Completamento della migrazione post-supporto: gli amministratori del supporto del prodotto possono segnalare i casi tramite il portale di supporto Experience League.

Se hai successo con Ultimate, puoi accedere al servizio Admin Console Migration White Glove. Per assistenza, rivolgiti al team dell’account Adobe (il tuo Account Manager).

**Se si utilizza un&#39;identità Adobe per accedere ad altre applicazioni Adobe, è possibile utilizzarla per accedere a Marketo?**

Anche se disponi di altri prodotti Adobe, non puoi accedere a Marketo con Adobe Identity finché l’abbonamento non viene migrato a IMS.

**I ruoli utente di Marketo (all&#39;interno delle aree di lavoro) sono gestiti in Adobe Admin Console?**

No. La gestione dei ruoli utente (all’interno delle aree di lavoro) viene completata nel Marketo Engage.

**Sono un amministratore di Marketo in una sottoscrizione integrata IMS e non ho accesso all&#39;Admin Console. Come posso ottenere l&#39;accesso?**

Qualsiasi amministratore di prodotto o di Adobe che ha accesso all’Admin Console della tua organizzazione può concederti l’accesso. Se non sai chi dispone dei privilegi di amministratore nella console all&#39;interno della tua organizzazione, contatta l&#39;[Assistenza clienti Adobe](https://helpx.adobe.com/contact.html){target="_blank"}.

**In che modo un amministratore aggiungerebbe utenti a Marketo [!DNL Sales Connect]?**

A differenza della scheda prodotto disponibile in Admin Console per [!DNL Sales Connect], non utilizzare Admin Console per aggiungere/gestire gli utenti. Il seguente collegamento consentirà agli amministratori di gestire gli utenti tramite Marketo [!DNL Sales Connect]: [https://toutapp.com/next#settings/admin/user-management](https://toutapp.com/next#settings/admin/user-management){target="_blank"}.

**Dove posso trovare ulteriori informazioni su Adobe Admin Console?**

[https://helpx.adobe.com/enterprise/admin-guide.html](https://helpx.adobe.com/it/enterprise/admin-guide.html){target="_blank"}.

**Vado comunque alla sezione Amministratore in Marketo per apportare modifiche all&#39;account utente per il mio account?**

No, passare a [account.adobe.com](https://account.adobe.com){target="_blank"}.

**Come funziona con l&#39;ID universale di Marketo?**

Chi ha effettuato l’onboarding in Adobe identity può accedere senza problemi a tutti gli abbonamenti abilitati per IMS tramite il selettore di abbonamento nel prodotto.

**Funziona con SSO?**

Sì.  L’integrazione di Marketo con Adobe IMS supporta gli utenti Universal ID e SSO. L’SSO è ora gestito da Adobe IMS ed è configurato a livello di organizzazione in Adobe Admin Console. [Ulteriori informazioni](https://helpx.adobe.com/it/enterprise/using/set-up-identity.html){target="_blank"}.

**Ho già effettuato l&#39;onboarding in Adobe Identity e ora voglio implementare il SSO. Cosa posso fare?**

Se desideri implementare Single Sign-On e il tuo abbonamento è stato effettuato all&#39;onboarding in Adobe Identity senza l&#39;SSO implementato nell&#39;organizzazione Adobe, invia un ticket al [Supporto Marketo](https://nation.marketo.com/){target="_blank"} e specifica l&#39;argomento come &quot;Marketo su Admin Console, implementazione dell&#39;SSO&quot;.

**Come funziona l&#39;autorizzazione del dispositivo?**

Adobe IMS al momento non supporta nulla come la funzione di autorizzazione dei dispositivi di Marketo.

**È ancora possibile utilizzare la funzione &quot;Accedi alla finestra di dialogo Invita utente&quot; per rendere univoco l&#39;accesso di un utente dall&#39;e-mail?**

No. Il flusso di lavoro Invito utente non è più attivo quando una sottoscrizione è abilitata per IMS, pertanto la funzione non è più valida. Adobe L’identità di un utente è guidata dal suo indirizzo e-mail. L’identità di un utente è guidata dal suo indirizzo e-mail.

**Per Adobe IMS, è possibile utilizzare Adobe ID, Enterprise ID o Federated ID?**

Sì, è possibile determinare il tipo di identità per il supporto dell&#39;organizzazione. Ulteriori informazioni sono disponibili qui: [Panoramica identità](https://helpx.adobe.com/it/enterprise/using/identity.html) e qui: [Configura identità](https://helpx.adobe.com/it/enterprise/using/set-up-identity.html){target="_blank"}.

**Quali schede prodotto sono supportate in Adobe Admin Console?**

Le schede prodotto supportate sono: Marketo Engage, Marketo Measure, Marketo Dynamic Chat, Marketo Sales Connect e Marketo Sales Insight Actions.

**Cosa succede se l&#39;accesso utente non corrisponde all&#39;indirizzo e-mail quando viene eseguita la migrazione a un&#39;identità Adobe?**

Gli attuali utenti del Marketo Engage con accessi diversi dal proprio indirizzo e-mail non accederanno più con quella credenziale una volta migrati a un’identità Adobe. Le identità di Adobe si autenticano sempre con l’indirizzo e-mail di un utente. Adobe Puoi aggiornare un indirizzo e-mail di identità all&#39;indirizzo [account.adobe.com](https://account.adobe.com){target="_blank"}.

**Cosa succede dopo la migrazione di Adobe Identity se la sottoscrizione utilizza le impostazioni di restrizione IP?**

Quando si effettua l’onboarding delle sottoscrizioni in Adobe Identity, non viene effettuata la migrazione delle impostazioni di restrizione IP a Adobe Admin Console. Le impostazioni di restrizione IP di Marketo includono l’autorizzazione all’accesso solo da indirizzi IP specifici e il blocco dell’accesso da parte di indirizzi IP specifici. Al momento, Adobe Identity Management System non supporta le funzioni di restrizione IP.

A partire dai primi mesi del 2025, Adobe Identity Management System rilascerà una funzione per supportare solo indirizzi IP specifici, supportando una transizione per gli utenti di Marketo che attualmente utilizzano questa funzione. Gli utenti che attualmente utilizzano questa funzione non verranno sottoposti a migrazione fino al rilascio della funzione. Una volta distribuita la funzione, gli utenti riceveranno una notifica della pianificazione della migrazione. Se disponibili, verranno fornite ulteriori informazioni sulla funzione.

Gli utenti che attualmente utilizzano la restrizione IP, che blocca l’accesso a indirizzi specifici, non potranno più utilizzare questa funzione dopo la migrazione ad Adobe Identity, in quanto non supportata da Adobe Identity Management System.

**Cosa succede dopo la migrazione di Adobe Identity se dispongo di utenti con un ruolo con l&#39;opzione &#39;Ignora Single Sign-On&#39;?**

Quando si effettua l’onboarding degli abbonamenti in Adobe Adobe Identity, a livello di organizzazione viene impostato il Single Sign On (SSO) per tutti gli utenti. Quando è configurato, l’SSO viene applicato per tutti gli utenti Marketo e per tutte le istanze Marketo in tale organizzazione Adobe. In precedenza, Marketo supportava l’impostazione di un ruolo utente con l’opzione &quot;Bypass Single Sign On&quot; (Ignora accesso singolo). Questa funzione non è supportata da Adobe Identity Management System.

**Ho più di una sottoscrizione, ma non tutte hanno Single Sign-On abilitato. Cosa succede dopo la migrazione di Adobe Identity?**

Quando si effettua l’onboarding degli abbonamenti in Adobe Identity, viene impostato il Single Sign On (SSO) a livello di organizzazione Adobe. Ciò significa che l’SSO si applica a tutte le istanze di prodotto nell’organizzazione Adobe. Una volta configurato, l’SSO verrà applicato a tutte le istanze Marketo in tale organizzazione Adobe. In precedenza, Marketo supportava questa impostazione a livello di istanza. Non supportato da Adobe Identity Management System.

**Sono necessarie modifiche a CNAME, SPF o DKIM attualmente utilizzati per il Marketo Engage dopo la migrazione di Adobe Identity?**

No, non vi sono impatti su queste configurazioni.

**Come posso evitare il timeout delle sessioni?**

In [Impostazioni avanzate](https://helpx.adobe.com/enterprise/using/authentication-settings.html#advanced-settings), è possibile personalizzare la durata massima della sessione desiderata (sono necessarie le autorizzazioni di amministratore di sistema). Si consiglia di stabilire questa impostazione dopo la migrazione del prodotto, ma prima della migrazione degli utenti.

**Per accedere al Marketo Engage, ora devo passare a Experience Cloud. Esiste un modo per semplificare questo flusso?**

Sì.  Puoi creare un segnalibro del browser del collegamento che viene avviato dopo aver fatto clic sul pulsante **Avvia** nella pagina di ingresso dell&#39;istanza di Marketo Engage per ignorare la pagina in corso.

![](assets/faq-1.png)
