---
description: Panoramica - Documentazione Marketo - Documentazione del prodotto
title: Panoramica
hide: true
hidefromtoc: true
source-git-commit: 6047665cf94a4b212734667feeb5fce911ffdebb
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 0%

---

# Panoramica {#overview}

Se l’abbonamento al Marketo Engage di Adobe è stato effettuato il 21/04/o dopo, verrà integrato con il sistema Identity Management di Adobe. AIMS consente agli utenti di accedere ad Marketi Engage e ad altre applicazioni Experience Cloud utilizzando una comune identità Adobe.

## Livelli profilo

Ci sono tre livelli di profilo.

<table>
 <tr>
  <td><strong>Amministratore di sistema</strong></td>
  <td>Responsabile dell’impostazione dei concetti di identità per l’organizzazione Adobe e il prodotto Marketo Engage in Adobe Admin Console.</td>
 </tr>
 <tr>
  <td><strong>Amministratore del prodotto</strong></td>
  <td>Responsabile del diritto degli utenti al prodotto di Marketo Engage in Adobe Admin Console.</td>
 </tr>
 <tr>
  <td><strong>Utente</strong></td>
  <td>Persona a cui è stato concesso l'accesso al Marketo Engage. Nessun privilegio amministrativo.</td>
 </tr>
</table>

## Domande frequenti

**Che cos’è l’identità Adobe?**

Adobe Identity Management System è costituito da tre componenti.

* Servizio Adobe Identity: Gestisce l’autenticazione e la convalida dell’utente finale, inclusa la federazione e il runtime Single-Sign-On (SSO).

* Adobe Admin Console: L’Admin Console fornisce una posizione centrale per la gestione delle adesioni Adobe in tutta l’organizzazione. Gestisce la gestione degli utenti, il servizio cloud, l’adesione alla licenza del desktop, la configurazione della federazione e fornisce funzioni di sicurezza per la prevenzione della perdita dei dati.

* API di gestione utenti di Adobe (UMAPI): Consente alle organizzazioni di gestire gli utenti e le adesioni aziendali in Adobe Admin Console a livello di API.

**Qual è la differenza tra un amministratore di prodotto Adobe e un amministratore di Marketo Engage?**

* Adobe Product Admin è un nuovo ruolo nella piattaforma Marketo.
* È un ruolo di sola lettura e non può essere modificato o eliminato da Marketo.
* Dispone degli stessi diritti e privilegi dell’amministratore Marketo standard.

**C&#39;è qualche modifica nel supporto client API?**

Sì. Chi è stato effettuato l’accesso ad Adobe IMS non può utilizzare le API di gestione utenti di Marketo esistenti. Userebbero [API IMS](https://www.adobe.io/apis/experienceplatform/umapi-new.html).

**Chi contiamo per il supporto?**

Segui la procedura standard per contattare [Supporto Marketo](https://nation.marketo.com/t5/support/ct-p/Support).

**I ruoli utente di Marketo (all’interno delle aree di lavoro) sono gestiti in Adobe Admin Console?**

No. La gestione del ruolo utente (all’interno delle aree di lavoro) viene completata in Marketo.

**Sono un amministratore di Marketo e non ho accesso all&#39;Admin Console. Come posso accedere?**

Qualsiasi amministratore di prodotto o di sistema che ha accesso all’Admin Console della tua organizzazione può concederti l’accesso. Se non sai chi dispone dei privilegi di amministratore nella console all’interno della tua organizzazione, contatta [Adobe Customer Care](https://helpx.adobe.com/contact.html).

**In che modo un amministratore può aggiungere utenti a Marketo Sales Connect?**

Mentre ci sarà una scheda prodotto in AC per Sales Connect, AC non deve essere utilizzato per aggiungere/gestire gli utenti. Il seguente collegamento consente agli amministratori di gestire gli utenti tramite Marketo Sales Connect: [https://toutapp.com/next#settings/admin/user-management](https://toutapp.com/next#settings/admin/user-management).

**Dove posso saperne di più su Adobe Admin Console?**

[https://helpx.adobe.com/enterprise/admin-guide.html](https://helpx.adobe.com/enterprise/admin-guide.html).

**Vado ancora alla sezione Amministratore in Marketo per apportare modifiche all’account?**

No, devi passare a [account.adobe.com](https://account.adobe.com).

**Come funziona questo con Marketo Universal ID?**

Coloro che hanno effettuato l’accesso all’identità Adobe possono accedere facilmente a tutte le iscrizioni IMS tramite lo switcher di abbonamento nel prodotto.

**Questo funziona con SSO?**

Sì. L’integrazione di Marketo con Adobe IMS supporta gli utenti Universal ID e SSO. L’SSO è ora gestito da Adobe IMS ed è configurato a livello di organizzazione in Adobe Admin Console. [Ulteriori informazioni qui](https://helpx.adobe.com/enterprise/using/set-up-identity.html).

**Come funziona l’autorizzazione dei dispositivi?**

Adobe IMS al momento non supporta funzioni simili a quelle di autorizzazione dei dispositivi Marketo.

**È ancora possibile utilizzare la funzione &quot;Login in Invite User Dialog&quot; per rendere l&#39;accesso unico dalla nostra e-mail?**

No. Il flusso di lavoro Invito utente non è più attivo quando un abbonamento è abilitato per IMS, pertanto la funzione non è più valida. L’identità di Adobe richiede che l’identità di un utente sia determinata dalla sua e-mail.

**Per Adobe IMS, è possibile utilizzare Adobe ID, Enterprise ID o Federated ID?**

Sì, è possibile determinare il tipo di identità per ottenere il supporto dell&#39;organizzazione. Ulteriori informazioni [qui](https://helpx.adobe.com/enterprise/using/identity.html) e [qui](https://helpx.adobe.com/enterprise/using/set-up-identity.html).

>[!MORELIKETHIS]
>
>* [Configurazione amministratore](/help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md)
>* [Aggiungere o rimuovere un amministratore di prodotto](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-product-admin.md)
>* [Aggiungi o rimuovi un utente](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md)

