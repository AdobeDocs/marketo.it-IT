---
description: Domande frequenti su Adobe Identity per Marketo Engage, tra cui migrazione, URL, SSO, amministratore di prodotto e amministratore di Marketo e inserisce nell'elenco Consentiti di.
title: Domande frequenti su Adobe Identity Management
feature: Marketo with Adobe Identity
exl-id: 2401def7-1696-4d77-a8a3-96c490517121
source-git-commit: a2c5ee6591b688ca262fbab94f0b13bae481daff
workflow-type: tm+mt
source-wordcount: '1591'
ht-degree: 98%

---

# Domande frequenti su Adobe Identity Management {#adobe-identity-management-faq}

**Cos’è Adobe Identity?**

Adobe Identity Management System è costituito da tre componenti.

* [!DNL Adobe Identity Service]: gestisce l’autenticazione e la convalida dell’utente finale, inclusi la federazione e il Single Sign-On (SSO) in fase di runtime.

* Adobe Admin Console: Admin Console offre un’unica posizione centrale per la gestione dei diritti Adobe per l’intera organizzazione. Consente di gestire gli utenti, il servizio cloud, i diritti delle licenze desktop e la configurazione della federazione; inoltre fornisce funzioni di sicurezza per la prevenzione della perdita di dati.

* API di Adobe User Management (UMAPI): consente alle organizzazioni di gestire gli utenti e i diritti Enterprise in Adobe Admin Console a livello di API.

**Quando verranno integrati con IMS gli abbonamenti Marketo Engage esistenti?**

Gli abbonamenti a Marketo Engage esistenti sono attualmente in fase di migrazione ad Adobe IMS in occasione di qualsiasi evento di vendita, quali rinnovi, modifiche al contratto e/o aggiunte. Le migrazioni al di fuori di un evento di vendita sono supportate a partire da ottobre 2024.

**Dopo la migrazione, gli URL di Marketo Engage rimarranno invariati?**

No. Dopo la migrazione, gli URL appariranno nel formato seguente: `https://experience.adobe.com/#/@tenantID/so:XXX-XXX-XXX/marketo-engage/classic/` (dove gli XXX rappresentano l’ID Munchkin e @tenantID proviene dalla tua organizzazione Adobe).

**È necessario fare qualcosa per prepararsi alla modifica dell’URL?**

Sì. Dopo la migrazione, Marketo Engage passerà dall’essere fornito tramite experience.adobe.com ad Adobe Experience Cloud. Per evitare interruzioni all’accesso a Marketo Engage, dovrai collaborare con il tuo team IT per inserire nell’elenco Consentiti tutti i domini Adobe elencati [all’inizio di questo articolo](/help/marketo/getting-started/initial-setup/configure-protocols-for-marketo.md){target="_blank"}.

I collegamenti e i segnalibri precedenti per le risorse Marketo Engage nel dominio engage-xx.marketo.com _continueranno_ a funzionare. Tuttavia, devi prima accedere all’istanza di Marketo Engage per l’URL di destinazione. Ad esempio, se usi un segnalibro per passare a una campagna avanzata nell’istanza con ID Munchkin 123-ABC-456, devi prima accedere all’istanza Marketo Engage con ID Munchkin 123-ABC-456.

Anche se non è previsto, è possibile che sviluppi futuri compromettano questa funzione di reindirizzamento. Per evitare interruzioni impreviste, si consiglia di aggiornare i segnalibri il prima possibile.

**Funziona con SSO?**

Sì. L’integrazione con Adobe IMS supporta gli utenti con ID universale e SSO. L’SSO è ora gestito da Adobe IMS ed è configurato a livello di organizzazione in Adobe Admin Console. Tuttavia, esistono differenze nel supporto di Marketo Engage avviato da un provider di identità (IdP) o dal provider di servizi (SP) di Adobe (per ulteriori informazioni, [ulteriori consulta questo articolo](https://helpx.adobe.com/it/enterprise/using/set-up-identity.html){target="_blank"}). Se hai bisogno di assistenza per le differenze a livello di SSO dopo la migrazione ad Admin Console, contatta l’[assistenza clienti Adobe](https://helpx.adobe.com/it/contact.html){target="_blank"}.

**Qual è la differenza tra un amministratore di prodotto Adobe e un amministratore di Marketo Engage?**

* L’amministratore di prodotto Adobe è un nuovo ruolo nella piattaforma Marketo.
* Il ruolo di amministratore di prodotto Adobe viene concesso agli utenti aggiunti come amministratore di prodotto in Adobe Admin Console
* L’amministratore di prodotto Adobe è un ruolo di sola lettura e non può essere modificato né eliminato da Marketo Engage.
* L’amministratore di prodotto Adobe dispone degli stessi diritti e privilegi di un amministratore Marketo standard.
* Il ruolo di amministratore di Marketo Engage è ancora quello di amministratore e viene concesso a un utente in Marketo Engage.
* Solo agli utenti con il ruolo di amministratore predefinito di Marketo viene assegnato quello di amministratore di prodotto di Marketo in Admin Console.

**Sono state apportate modifiche al supporto dei client API per la gestione degli utenti?**

Sì. Gli utenti per i quali è stato eseguito l’onboarding in Adobe IMS non possono utilizzare tutte le API per la gestione degli utenti di Marketo esistenti. Per le azioni di invito, aggiornamento ed eliminazione di utenti, è necessario utilizzare le [API IMS](https://www.adobe.io/apis/experienceplatform/umapi-new.html){target="_blank"} di Adobe. Per la gestione dei ruoli, restano valide le API per la gestione degli utenti di Marketo. Inoltre, non vi sono altre modifiche al supporto dei client API REST di Marketo.

**A chi bisogna rivolgersi per assistenza in caso di integrazione con IMS?**

* Prima della migrazione degli utenti: registra un casi di supporto nella [community Marketing Nation](https://nation.marketo.com/t5/support/ct-p/Support) o tramite e-mail all¦indirizzo `marketocares@adobe.com`.

* Dopo la migrazione degli utenti: registra un caso di supporto nella [community Marketing Nation](https://nation.marketo.com/t5/support/ct-p/Support) o tramite e-mail all’indirizzo `marketocares@adobe.com`.

* Dopo il completamento della migrazione del supporto: gli amministratori del supporto del prodotto possono aprire casi tramite il portale di assistenza Experience League.

Se hai un piano Ultimate Success, puoi accedere al servizio White Glove per la migrazione in Admin Console. Per assistenza, rivolgiti al team Adobe Account (il tuo Account Manager).

**Se utilizzo già un Adobe Identity per accedere ad altre applicazioni Adobe, posso utilizzarlo anche per accedere a Marketo?**

Anche se hai altri prodotti Adobe, potrai accedere a Marketo con Adobe Identity solo dopo che l’abbonamento sarà stato migrato a IMS.

**I ruoli utente di Marketo (all’interno delle aree di lavoro) sono gestiti in Adobe Admin Console?**

No. La gestione dei ruoli utente (all’interno delle aree di lavoro) viene completata in Marketo Engage.

**Sono un amministratore di Marketo per un abbonamento integrato con IMS e non ho accesso ad Admin Console. Come posso ottenere l’accesso?**

Qualsiasi amministratore di prodotto o di sistema Adobe che ha accesso ad Admin Console per la tua organizzazione può concederti l’accesso. Se non sai chi dispone dei privilegi di amministratore nella console all’interno della tua organizzazione, contatta l’[Assistenza clienti Adobe](https://helpx.adobe.com/it/contact.html){target="_blank"}.

**In che modo un amministratore può aggiungere utenti a Marketo [!DNL Sales Connect]?**

Anche se in Admin Console sarà disponibile una scheda prodotto per [!DNL Sales Connect], non utilizzare Admin Console per aggiungere/gestire gli utenti. Il collegamento seguente consentirà agli amministratori di gestire gli utenti tramite Marketo [!DNL Sales Connect]: [https://toutapp.com/next#settings/admin/user-management](https://toutapp.com/next#settings/admin/user-management){target="_blank"}.

**Dove posso trovare ulteriori informazioni su Adobe Admin Console?**

[https://helpx.adobe.com/it/enterprise/admin-guide.html](https://helpx.adobe.com/it/enterprise/admin-guide.html){target="_blank"}.

**Per modificare il mio account utente, devo ancora accedere alla sezione Amministrazione di Marketo?**

No, devi accedere a [account.adobe.com](https://account.adobe.com/it/){target="_blank"}.

**Come funziona con l’ID universale di Marketo?**

Gli utenti per i quali è stato eseguito l’onboarding in Adobe identity possono accedere direttamente a tutti gli abbonamenti abilitati per IMS tramite il selettore di abbonamento nel prodotto.

**Funziona con SSO?**

Sì. L’integrazione di Marketo con Adobe IMS supporta gli utenti con ID universale e SSO. L’SSO è ora gestito da Adobe IMS ed è configurato a livello di organizzazione in Adobe Admin Console. Per ulteriori informazioni, [consulta questo articolo](https://helpx.adobe.com/it/enterprise/using/set-up-identity.html){target="_blank"}.

**Il mio onboarding in Adobe Identity è già stato eseguito e ora desidero implementare l’SSO. Cosa devo fare?**

Se desideri implementare Single Sign On e per il tuo abbonamento è già stato completato l’onboarding in Adobe Identity, ma l’SSO non è stato implementato nella tua organizzazione Adobe, invia un ticket all’[assistenza di Marketo](https://nation.marketo.com/){target="_blank"} utilizzando l’argomento “Marketo on Admin Console, implementing SSO”.

**Come funziona l’autorizzazione dei dispositivi?**

Adobe IMS al momento non supporta alcuna funzione di autorizzazione dei dispositivi di Marketo.

**È ancora possibile utilizzare la funzione “Accesso nella finestra di dialogo Invita utente” per rendere l’accesso di un utente univoco dal suo indirizzo e-mail?**

No. Quando un abbonamento è abilitato per IMS, il flusso di lavoro Invita utente non è più attivo, pertanto questa funzione non è più valida. Adobe Identity richiede che l’identità di un utente dipenda dal suo indirizzo e-mail.

**Per Adobe IMS, è possibile utilizzare Adobe ID, Enterprise ID o Federated ID?**

Sì, sei tu a determinare il tipo di identità che deve essere supportata dalla tua organizzazione. Ulteriori informazioni sono disponibili in [Panoramica sull’identità](https://helpx.adobe.com/it/enterprise/using/identity.html) e in [Configurare l’identità](https://helpx.adobe.com/it/enterprise/using/set-up-identity.html){target="_blank"}.

**Quali schede prodotto sono supportate in Adobe Admin Console?**

Le schede prodotto supportate sono: Marketo Engage, Marketo Measure, Marketo Dynamic Chat, Marketo Sales Connect e Marketo Sales Insight Actions.

**Cosa succede se il mio accesso utente non corrisponde al mio indirizzo e-mail al momento della migrazione ad Adobe Identity?**

Dopo la migrazione ad Adobe Identity, gli utenti attuali di Marketo Engage le cui credenziali di accesso sono diverse dal proprio indirizzo e-mail non potranno più accedere con tali credenziali. L’autenticazione delle identità Adobe avviene sempre mediante l’indirizzo e-mail dell’utente. Puoi aggiornare un indirizzo e-mail di Adobe Identity in [account.adobe.com](https://account.adobe.com/it/){target="_blank"}.

**Cosa succede dopo la migrazione ad Adobe Identity se il mio abbonamento utilizza impostazioni di restrizione IP?**

Le restrizioni IP correnti rimarranno attive fino al primo trimestre del 2026 (questo vale per gli abbonamenti per i quali tali restrizioni erano abilitate prima della migrazione). Le restrizioni verranno applicate anche agli utenti con Adobe ID, in modo che i controlli di accesso continuino a funzionare come previsto.

A partire dal primo trimestre del 2026, le restrizioni IP precedenti verranno ritirate. Da quel momento in poi, l’accesso basato su IP sarà gestito esclusivamente in Adobe Admin Console (AAC). Per mantenere sicuri gli accessi, devi configurare le restrizioni IP in AAC. Per ulteriori informazioni, consulta questo [post di blog su Marketing Nation](https://nation.marketo.com/t5/product-blogs/updated-important-update-ip-restrictions-feature-transition/ba-p/358420){target="_blank"}.

**Cosa succede dopo la migrazione ad Adobe Identity se alcuni utenti hanno un ruolo con l’opzione “Ignora Single Sign-On”?**

Adobe Admin Console viene fornito con una directory di Business ID predefinita. Gli utenti che appartengono a domini non inclusi nelle directory di Federated ID in un’organizzazione Adobe verranno assegnati a questa directory con un tipo di identità Adobe ID. Tali utenti potranno accedere a Marketo Engage senza passare attraverso il Single Sign On (SSO) e la licenza rimane di proprietà dell’azienda, non dei singoli utenti.

**Ho più di un abbonamento, ma non tutti sono abilitati per Single Sign-On. Cosa succede dopo la migrazione ad Adobe Identity?**

Quando si effettua l’onboarding degli abbonamenti in Adobe Identity, viene configurato il Single Sign On (SSO) a livello di organizzazione Adobe. Questo significa che l’SSO si applica a tutte le istanze di prodotto nell’organizzazione Adobe. Una volta configurato, l’SSO verrà applicato a tutte le istanze di Marketo in tale organizzazione Adobe. In precedenza, Marketo supportava questa impostazione a livello di istanza. Questo non è supportato da Adobe Identity Management System.

**Sono necessarie modifiche a CNAME, SPF o DKIM attualmente utilizzati per Marketo Engage dopo la migrazione ad Adobe Identity?**

No, non vi è alcun impatto su queste configurazioni.

**Come posso evitare il timeout delle sessioni?**

In [Impostazioni avanzate](https://helpx.adobe.com/it/enterprise/using/authentication-settings.html#advanced-settings){target="_blank"}, è possibile personalizzare la durata massima desiderata per le sessioni (sono necessarie autorizzazioni di amministratore di sistema). Si consiglia di stabilire questa impostazione dopo la migrazione del prodotto, ma prima della migrazione degli utenti.

**Ora devo passare ad Experience Cloud per accedere a Marketo Engage. Esiste un modo per semplificare questo flusso?**

Sì. Fai clic sul pulsante **Avvia** nella pagina di ingresso dell’istanza di Marketo Engage, quindi crea un segnalibro nel browser per il collegamento risultante. In futuro, potrai usare direttamente tale segnalibro.

![](assets/faq-1.png)
