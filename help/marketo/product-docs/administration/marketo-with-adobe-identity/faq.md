---
description: Domande frequenti su Identity Management per Adobe - Documentazione di Marketo - Documentazione del prodotto
title: Domande frequenti su Identity Management Adobe
feature: Marketo with Adobe Identity
exl-id: 2401def7-1696-4d77-a8a3-96c490517121
source-git-commit: eca77d8426c8f696dc35dbfb9e20abcb46e53127
workflow-type: tm+mt
source-wordcount: '1180'
ht-degree: 1%

---

# Domande frequenti su Identity Management Adobe {#adobe-identity-management-faq}

**Che cos’è l’identità Adobe?**

Adobe Identity Management System è costituito da tre componenti.

* [!DNL Adobe Identity Service]: gestisce l’autenticazione e la convalida dell’utente finale, incluso il Single Sign-On (SSO) di federazione e runtime.

* Adobe Admin Console: l’Admin Console fornisce una posizione centrale per la gestione dei diritti Adobi in tutta l’organizzazione. Gestisce la gestione degli utenti, il servizio cloud, il diritto alla licenza del desktop, la configurazione della federazione e fornisce funzioni di sicurezza per la prevenzione della perdita di dati.

* Adobe User Management API (UMAPI): consente alle organizzazioni di gestire gli utenti e le autorizzazioni Enterprise in Adobe Admin Console a livello di API.

**Quando verranno integrati con IMS gli abbonamenti di Marketo Engage esistenti?**

Gli abbonamenti Marketo esistenti verranno migrati al sistema Identity Management Adobe più avanti nel corso dell’anno. Il supporto Marketo non sarà in grado di fornire aggiornamenti relativi alla migrazione Adobe IMS. Il team dell’account Adobe raggiungerà la tempistica stimata nei prossimi mesi.

**Qual è la differenza tra un amministratore di prodotto Adobe e un amministratore di Marketo Engage?**

* L’amministratore di prodotto di Adobe è un nuovo ruolo nella piattaforma Marketo.
* Adobe Il ruolo di amministratore di prodotto è concesso agli utenti aggiunti come amministratore di prodotto in Adobe Admin Console
* Adobe L’amministratore del prodotto è un ruolo di sola lettura e non può essere modificato o eliminato dal Marketo Engage.
* L’amministratore di prodotto Adobe dispone degli stessi diritti e privilegi di un amministratore Marketo standard.
* Il ruolo di amministratore di Marketo Engage è ancora amministratore e viene concesso a un utente del Marketo Engage.

**È stato modificato il supporto client API per la gestione degli utenti?**

Sì. Gli utenti che hanno effettuato l’onboarding in Adobe IMS non possono utilizzare tutte le API di gestione utenti di Marketo esistenti. Per le azioni di invito, aggiornamento ed eliminazione degli utenti, l&#39;Adobe [API IMS](https://www.adobe.io/apis/experienceplatform/umapi-new.html){target="_blank"} deve essere utilizzato. Per la gestione dei ruoli, si applicano ancora le API di gestione utenti di Marketo. Inoltre, non vi sono altre modifiche al supporto client API REST di Marketo.

**Chi contatteremo per il supporto se siamo integrati con IMS?**

Segui la procedura standard per contattare [Supporto Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

**Se utilizzo un’identità Adobe per accedere ad altre applicazioni Adobe, posso utilizzarla per accedere a Marketo?**

Anche se disponi di altri prodotti Adobe, non puoi accedere a Marketo con Identità Adobe finché l’abbonamento non viene migrato a IMS.

**I ruoli utente di Marketo (all’interno delle aree di lavoro) sono gestiti in Adobe Admin Console?**

No. La gestione dei ruoli utente (all’interno delle aree di lavoro) viene completata nel Marketo Engage.

**Sono un amministratore di Marketo in un abbonamento integrato IMS e non ho accesso all’Admin Console. Come posso ottenere l’accesso?**

Qualsiasi amministratore di prodotto o di sistema di Adobe che ha accesso all’Admin Console della tua organizzazione può concederti l’accesso. Se non sai chi dispone dei privilegi di amministratore nella console all’interno della tua organizzazione, contatta [Assistenza clienti Adobe](https://helpx.adobe.com/contact.html){target="_blank"}.

**In che modo un amministratore aggiungerebbe utenti a Marketo [!DNL Sales Connect]?**

Mentre sarà disponibile una scheda prodotto in Admin Console per [!DNL Sales Connect], Admin Console non deve essere utilizzato per aggiungere/gestire gli utenti. Il seguente collegamento consente agli amministratori di gestire gli utenti tramite Marketo [!DNL Sales Connect]: [https://toutapp.com/next#settings/admin/user-management](https://toutapp.com/next#settings/admin/user-management){target="_blank"}.

**Dove posso trovare ulteriori informazioni su Adobe Admin Console?**

[https://helpx.adobe.com/it/enterprise/admin-guide.html](https://helpx.adobe.com/it/enterprise/admin-guide.html){target="_blank"}.

**Vado comunque alla sezione Amministratore in Marketo per apportare modifiche all’account utente?**

No, dovrai passare a [account.adobe.com](https://account.adobe.com){target="_blank"}.

**Come funziona con l&#39;Universal ID di Marketo?**

Coloro che utilizzano l’identità Adobe possono accedere facilmente a tutti gli abbonamenti abilitati per IMS tramite il selettore di abbonamento nel prodotto.

**Funziona con SSO?**

Sì. L’integrazione di Marketo con Adobe IMS supporta gli utenti Universal ID e SSO. L’SSO è ora gestito da Adobe IMS ed è configurato a livello di organizzazione in Adobe Admin Console. [Fai clic qui per ulteriori informazioni](https://helpx.adobe.com/enterprise/using/set-up-identity.html){target="_blank"}.

**Come funziona l&#39;autorizzazione del dispositivo?**

Adobe IMS al momento non supporta nulla come la funzione di autorizzazione dei dispositivi di Marketo.

**È ancora possibile utilizzare la funzione &quot;Accedi alla finestra di dialogo Invita utente&quot; per rendere univoco l’accesso di un utente dall’e-mail?**

No. Il flusso di lavoro Invito utente non è più attivo quando una sottoscrizione è abilitata per IMS, pertanto la funzione non è più valida. L’identità Adobe richiede che l’identità di un utente sia guidata dalla sua e-mail.

**Per Adobe IMS, abbiamo la possibilità di utilizzare Adobe ID, Enterprise ID o Federated ID?**

Sì, è possibile determinare il tipo di identità per il supporto dell&#39;organizzazione. Ulteriori informazioni sono disponibili qui: [Panoramica dell’identità](https://helpx.adobe.com/enterprise/using/identity.html) e qui: [Impostare l’identità](https://helpx.adobe.com/enterprise/using/set-up-identity.html){target="_blank"}.

**Quali schede prodotto sono supportate in Adobe Admin Console?**

Le schede prodotto supportate sono: Marketi Engage, Marketo Measure, Marketo Dynamic Chat, Marketo Sales Connect e Marketo Sales Insight Actions.

**Cosa succede se il mio accesso utente non corrisponde al mio indirizzo e-mail quando vengo migrato a un&#39;identità Adobe?**

Gli attuali utenti di Marketo con accessi diversi dal proprio indirizzo e-mail non accederanno più con quella credenziale una volta migrati a un’identità di Adobe. Le identità di Adobe si autenticano sempre con l’indirizzo e-mail di un utente.

**Cosa succede dopo la migrazione dell’identità di Adobe se il mio abbonamento utilizza le impostazioni di restrizione IP?**

Quando si effettua l’onboarding delle sottoscrizioni in Adobe Identity, non viene effettuata la migrazione delle impostazioni di restrizione IP a Adobe Admin Console. Le impostazioni di restrizione IP di Marketo includono l’autorizzazione all’accesso solo da indirizzi IP specifici e il blocco dell’accesso da parte di indirizzi IP specifici. Al momento, Adobe Identity Management System non supporta le funzioni di restrizione IP.

Nel 2024, Adobe Identity Management System rilascerà una funzione per supportare solo indirizzi IP specifici, supportando una transizione per gli utenti di Marketo che attualmente utilizzano questa funzione. Gli utenti che attualmente utilizzano questa funzione non verranno sottoposti a migrazione fino al rilascio della funzione. Una volta distribuita la funzione, gli utenti riceveranno una notifica della pianificazione della migrazione. Se disponibili, verranno fornite ulteriori informazioni sulla funzione.

Gli utenti che attualmente utilizzano la restrizione IP, che blocca l’accesso a indirizzi specifici, non potranno più utilizzare questa funzione dopo la migrazione ad Adobe Identity, in quanto non supportata da Adobe Identity Management System.

**Cosa succede dopo la migrazione di Adobe Identity se dispongo di utenti con un ruolo con l’opzione &quot;Bypass Single Sign On&quot; (Ignora Single Sign On)?**

Quando si effettua l’onboarding degli abbonamenti in Adobe Identity, a livello di organizzazione Adobe viene impostato il Single Sign On (SSO) per tutti gli utenti. Quando è configurato, l’SSO viene applicato per tutti gli utenti Marketo e per tutte le istanze Marketo in tale organizzazione di Adobe. In precedenza, Marketo supportava l’impostazione di un ruolo utente con l’opzione &quot;Bypass Single Sign On&quot; (Ignora accesso singolo). Questo non è supportato da Adobe Identity Management System.

**È presente più di un abbonamento, ma non tutti hanno Single Sign-On abilitato. Cosa succede dopo la migrazione dell’identità di Adobe?**

Quando si effettua l’onboarding degli abbonamenti in Adobe Identity, viene impostato il Single Sign On (SSO) a livello di organizzazione Adobe. Ciò significa che l’SSO si applica a tutte le istanze di prodotto nell’organizzazione Adobe. Una volta configurato, l’SSO verrà applicato a tutte le istanze Marketo in tale organizzazione di Adobe. In precedenza, Marketo supportava questa impostazione a livello di istanza. Non supportato da Adobe Identity Management System.
