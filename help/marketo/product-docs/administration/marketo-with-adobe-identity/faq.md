---
description: Domande frequenti su Adobe Identity Management - Documentazione su Marketo - Documentazione del prodotto
title: Domande frequenti su Adobe Identity Management
feature: Marketo with Adobe Identity
exl-id: 2401def7-1696-4d77-a8a3-96c490517121
source-git-commit: 95ed91736b7276dd7a5b9e09958c1f09832ae719
workflow-type: tm+mt
source-wordcount: '1579'
ht-degree: 1%

---

# Domande frequenti su Adobe Identity Management {#adobe-identity-management-faq}

**Cos&#39;è Adobe Identity?**

Adobe Identity Management System è costituito da tre componenti.

* [!DNL Adobe Identity Service]: gestisce l&#39;autenticazione e la convalida dell&#39;utente finale, inclusi la federazione e il Single Sign-On (SSO) di runtime.

* Adobe Admin Console: Admin Console fornisce una posizione centrale per la gestione delle adesioni Adobe in tutta l’organizzazione. Gestisce la gestione degli utenti, il servizio cloud, il diritto alla licenza del desktop, la configurazione della federazione e fornisce funzioni di sicurezza per la prevenzione della perdita di dati.

* Adobe User Management API (UMAPI): consente alle organizzazioni di gestire gli utenti e le autorizzazioni Enterprise in Adobe Admin Console a livello di API.

**Quando verranno integrati con IMS gli abbonamenti Marketo Engage esistenti?**

Gli abbonamenti Marketo Engage esistenti sono attualmente in fase di migrazione ad Adobe IMS su qualsiasi evento di vendita, che include rinnovi, eventi di riappalto e/o supplementi. Le migrazioni al di fuori di un evento di vendita sono supportate a ottobre 2024.

**Dopo la migrazione, gli URL di Marketo Engage rimarranno invariati?**

No. Dopo la migrazione, gli URL appariranno nel formato seguente: `https://experience.adobe.com/#/@tenantID/so:XXX-XXX-XXX/marketo-engage/classic/` (gli XXX rappresentano l&#39;ID Munchkin e @tenantID proviene dall&#39;organizzazione Adobe).

**C&#39;è qualcosa da fare per prepararci alla modifica dell&#39;URL?**

Sì.  Dopo la migrazione, Marketo Engage passerà da experience.adobe.com a Adobe Experience Cloud. Per evitare interruzioni dell&#39;accesso a Marketo Engage, dovrai collaborare con il tuo team IT per inserire nell&#39;elenco Consentiti tutti i domini Adobe elencati [nella parte superiore di questo articolo](/help/marketo/getting-started/initial-setup/configure-protocols-for-marketo.md){target="_blank"}.

I collegamenti e i segnalibri precedenti per le risorse Marketo Engage nel dominio engage-xx.marketo.com _funzioneranno_. Tuttavia, devi prima accedere all’istanza di Marketo Engage per l’URL a cui stai navigando. Ad esempio, per passare a un segnalibro per una campagna avanzata nell’istanza con Munchkin ID 123-ABC-456, devi prima accedere all’istanza Marketo Engage con Munchkin ID 123-ABC-456.

Anche se non pianificato, il lavoro di sviluppo futuro può interrompere questa funzione di reindirizzamento. Per evitare interruzioni impreviste, si consiglia di aggiornare i segnalibri il prima possibile.

**Funziona con SSO?**

Sì.  L’integrazione con Adobe IMS supporta gli utenti Universal ID e SSO. L’SSO è ora gestito da Adobe IMS ed è configurato a livello di organizzazione in Adobe Admin Console. Tuttavia, esistono differenze nel supporto avviato da Marketo Engage IdP rispetto al supporto avviato da Adobe SP ([ulteriori informazioni qui](https://helpx.adobe.com/it/enterprise/using/set-up-identity.html){target="_blank"}). Se hai bisogno di assistenza per le differenze SSO dopo la migrazione ad Admin Console, contatta l&#39;[Assistenza clienti Adobe](https://helpx.adobe.com/contact.html){target="_blank"}.

**Qual è la differenza tra un amministratore di prodotto Adobe e un amministratore di Marketo Engage?**

* L’amministratore di prodotto Adobe è un nuovo ruolo nella piattaforma Marketo.
* Il ruolo di amministratore di prodotto di Adobe viene concesso agli utenti aggiunti come amministratore di prodotto in Adobe Admin Console
* L’amministratore di prodotto Adobe è un ruolo di sola lettura e non può essere modificato o eliminato da Marketo Engage.
* L’amministratore di prodotto Adobe dispone degli stessi diritti e privilegi di un amministratore Marketo standard.
* Il ruolo di amministratore di Marketo Engage è ancora amministratore e viene concesso a un utente in Marketo Engage.
* Solo gli utenti con il ruolo Amministratore predefinito di Marketo vengono assegnati come Amministratore di prodotto Marketo in Admin Console.

**Sono state apportate modifiche al supporto client API per la gestione utenti?**

Sì.  Gli utenti che hanno effettuato l’onboarding in Adobe IMS non possono utilizzare tutte le API di gestione utenti di Marketo esistenti. Per le azioni di invito, aggiornamento ed eliminazione degli utenti, è necessario utilizzare le [API IMS](https://www.adobe.io/apis/experienceplatform/umapi-new.html){target="_blank"} di Adobe. Per la gestione dei ruoli, si applicano ancora le API di gestione utenti di Marketo. Inoltre, non vi sono altre modifiche al supporto client API REST di Marketo.

**A chi rivolgerci per richiedere assistenza se siamo integrati con IMS?**

* Migrazione pre-utente: casi di supporto dei file in [Marketing Nation Community](https://nation.marketo.com/t5/support/ct-p/Support) o e-mail `customercare@marketo.com`.

* Migrazione post-utente: casi di supporto file in [Marketing Nation Community](https://nation.marketo.com/t5/support/ct-p/Support) o e-mail `customercare@marketo.com`.

* Completamento della migrazione post-supporto: gli amministratori del supporto del prodotto possono segnalare i casi tramite il portale di supporto Experience League.

Se disponi di Ultimate Success, puoi accedere al servizio Admin Console Migration White Glove. Rivolgiti al team dell’account di Adobe (il tuo Account Manager) per assistenza.

**Se si utilizza un&#39;identità Adobe per accedere ad altre applicazioni Adobe, è possibile utilizzarla per accedere a Marketo?**

Anche se disponi di altri prodotti Adobe, non puoi accedere a Marketo con Adobe Identity finché l’abbonamento non viene migrato a IMS.

**I ruoli utente di Marketo (all&#39;interno delle aree di lavoro) sono gestiti in Adobe Admin Console?**

No. La gestione dei ruoli utente (all’interno delle aree di lavoro) viene completata in Marketo Engage.

**Sono un amministratore di Marketo in una sottoscrizione integrata IMS e non ho accesso ad Admin Console. Come posso ottenere l&#39;accesso?**

Qualsiasi amministratore di prodotto o di sistema di Adobe che ha accesso all’Admin Console della tua organizzazione può concederti l’accesso. Se non sai chi dispone dei privilegi di amministratore nella console all&#39;interno della tua organizzazione, contatta l&#39;[Assistenza clienti Adobe](https://helpx.adobe.com/contact.html){target="_blank"}.

**In che modo un amministratore aggiungerebbe utenti a Marketo [!DNL Sales Connect]?**

Anche se in Admin Console sarà disponibile una scheda prodotto per [!DNL Sales Connect], non utilizzare Admin Console per aggiungere/gestire gli utenti. Il seguente collegamento consentirà agli amministratori di gestire gli utenti tramite Marketo [!DNL Sales Connect]: [https://toutapp.com/next#settings/admin/user-management](https://toutapp.com/next#settings/admin/user-management){target="_blank"}.

**Dove posso trovare ulteriori informazioni su Adobe Admin Console?**

[https://helpx.adobe.com/enterprise/admin-guide.html](https://helpx.adobe.com/it/enterprise/admin-guide.html){target="_blank"}.

**Vado comunque alla sezione Amministratore in Marketo per apportare modifiche all&#39;account utente per il mio account?**

No, passare a [account.adobe.com](https://account.adobe.com){target="_blank"}.

**Come funziona con l&#39;ID universale di Marketo?**

Chi ha effettuato l’onboarding in Adobe identity può accedere senza problemi a tutti gli abbonamenti abilitati IMS tramite il selettore di abbonamento nel prodotto.

**Funziona con SSO?**

Sì.  L’integrazione di Marketo con Adobe IMS supporta gli utenti Universal ID e SSO. L’SSO è ora gestito da Adobe IMS ed è configurato a livello di organizzazione in Adobe Admin Console. [Ulteriori informazioni](https://helpx.adobe.com/it/enterprise/using/set-up-identity.html){target="_blank"}.

**Ho già effettuato l&#39;onboarding in Adobe Identity e ora voglio implementare il SSO. Cosa posso fare?**

Se desideri implementare Single Sign On e il tuo abbonamento è stato effettuato a Adobe Identity senza SSO implementato nell&#39;organizzazione Adobe, invia un ticket al [Supporto Marketo](https://nation.marketo.com/){target="_blank"} e specifica l&#39;argomento come &quot;Marketo su Admin Console, implementazione di SSO&quot;.

**Come funziona l&#39;autorizzazione del dispositivo?**

Adobe IMS al momento non supporta nulla come la funzione di autorizzazione dei dispositivi di Marketo.

**È ancora possibile utilizzare la funzione &quot;Accedi alla finestra di dialogo Invita utente&quot; per rendere univoco l&#39;accesso di un utente dall&#39;e-mail?**

No. Il flusso di lavoro Invito utente non è più attivo quando una sottoscrizione è abilitata per IMS, pertanto la funzione non è più valida. L’identità di Adobe richiede che l’identità di un utente sia guidata dalla sua e-mail.

**Per Adobe IMS, è possibile utilizzare Adobe ID, Enterprise ID o Federated ID?**

Sì, è possibile determinare il tipo di identità per il supporto dell&#39;organizzazione. Ulteriori informazioni sono disponibili qui: [Panoramica identità](https://helpx.adobe.com/it/enterprise/using/identity.html) e qui: [Configura identità](https://helpx.adobe.com/it/enterprise/using/set-up-identity.html){target="_blank"}.

**Quali schede prodotto sono supportate in Adobe Admin Console?**

Le schede prodotto supportate sono: Marketo Engage, Marketo Measure, Marketo Dynamic Chat, Marketo Sales Connect e Marketo Sales Insight Actions.

**Cosa succede se il mio accesso utente non corrisponde al mio indirizzo e-mail quando viene effettuata la migrazione a un&#39;identità Adobe?**

Gli attuali utenti di Marketo Engage con accessi diversi dal proprio indirizzo e-mail non accederanno più con tale credenziale una volta migrati a un’identità Adobe. Le identità di Adobe si autenticano sempre con l’indirizzo e-mail di un utente. Puoi aggiornare un indirizzo e-mail di identità Adobe all&#39;indirizzo [account.adobe.com](https://account.adobe.com){target="_blank"}.

**Cosa succede dopo la migrazione di Adobe Identity se la sottoscrizione utilizza le impostazioni di restrizione IP?**

Le restrizioni IP correnti rimarranno attive fino al primo trimestre del 2026 (questo vale per gli abbonamenti che li avevano abilitati prima della migrazione). Queste restrizioni verranno applicate anche agli utenti di Adobe ID, in modo che i controlli di accesso continuino a funzionare come previsto.

A partire dal primo trimestre del 2026, le restrizioni IP legacy verranno ritirate. Da quel momento in poi, l&#39;accesso basato su IP sarà gestito esclusivamente nel Adobe Admin Console (AAC). Per mantenere un accesso sicuro, devi configurare le restrizioni IP in AAC. Per ulteriori informazioni, consulta questo [post di blog della nazione di marketing](https://nation.marketo.com/t5/product-blogs/updated-important-update-ip-restrictions-feature-transition/ba-p/358420){target="_blank"}.

**Cosa succede dopo la migrazione di Adobe Identity se dispongo di utenti con un ruolo con l&#39;opzione &#39;Ignora Single Sign-On&#39;?**

Adobe Admin Console viene fornito con una directory Business ID predefinita. Gli utenti al di fuori dei domini rivendicati nelle directory di Federated ID in un’organizzazione Adobe verranno assegnati a questa directory con un tipo di identità Adobe ID. Questi utenti potranno accedere a Marketo Engage senza passare attraverso il Single Sign On (SSO) e la proprietà della licenza rimane a carico dell’azienda, non dei singoli utenti.

**Ho più di una sottoscrizione, ma non tutte hanno Single Sign-On abilitato. Cosa succede dopo la migrazione di Adobe Identity?**

Quando si effettua l’onboarding degli abbonamenti in Adobe Identity, viene configurato il Single Sign On (SSO) a livello di organizzazione Adobe. Questo significa che l’SSO si applica a tutte le istanze di prodotto nell’organizzazione Adobe. Una volta configurato, l’SSO verrà applicato a tutte le istanze Marketo in tale organizzazione Adobe. In precedenza, Marketo supportava questa impostazione a livello di istanza. Non supportato da Adobe Identity Management System.

**Sono necessarie modifiche a CNAME, SPF o DKIM attualmente utilizzati per Marketo Engage dopo la migrazione di Adobe Identity?**

No, non vi sono impatti su queste configurazioni.

**Come posso evitare il timeout delle sessioni?**

In [Impostazioni avanzate](https://helpx.adobe.com/enterprise/using/authentication-settings.html#advanced-settings){target="_blank"}, è possibile personalizzare la durata massima della sessione desiderata (sono necessarie le autorizzazioni di amministratore di sistema). Si consiglia di stabilire questa impostazione dopo la migrazione del prodotto, ma prima della migrazione degli utenti.

**Ora devo passare ad Experience Cloud per accedere a Marketo Engage. Esiste un modo per semplificare questo flusso?**

Sì.  Puoi creare un segnalibro del browser del collegamento che viene avviato dopo aver fatto clic sul pulsante **Launch** nella pagina di ingresso dell&#39;istanza di Marketo Engage per ignorare la pagina in corso.

![](assets/faq-1.png)
