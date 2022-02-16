---
description: Panoramica - Documentazione Marketo - Documentazione del prodotto
title: Panoramica
exl-id: 18ddeebc-bc89-411c-9d2c-23df6841cb3a
source-git-commit: 7eff888c0fdebf31da4706f70d1e99e8327807ca
workflow-type: tm+mt
source-wordcount: '957'
ht-degree: 0%

---

# Panoramica {#overview}

Se hai un nuovo account con Adobe Marketi Engage (nuovo account, non solo una nuova istanza per un account esistente) a partire dal 15 febbraio 2022, potrebbe venire integrato con l’Adobe Identity Management System, a seconda del pacchetto di prodotti acquistato. Per verificare se è disponibile, contatta il tuo Marketo Admin o il Customer Success Manager del tuo account.

Gli abbonamenti Marketo esistenti verranno migrati al sistema Adobe Identity Management a partire dalla fine di quest&#39;anno.

>[!NOTE]
>
>Il supporto Marketo non sarà in grado di fornire aggiornamenti sulla migrazione ad Adobe IMS. Nei prossimi mesi, il Customer Success Manager contatterà la tempistica stimata.

## Livelli profilo

Le sottoscrizioni di Marketo Engage di Adobe integrate nel sistema Identity Management di Adobe supportano vari profili. Di seguito sono elencati i tipi di profili utente rilevanti per questa integrazione.

<table>
 <tr>
  <td><strong>Amministratore di sistema Adobe Admin Console</strong></td>
  <td>Responsabile dell’impostazione dei concetti di identità per l’organizzazione Adobe e il prodotto Marketo Engage in Adobe Admin Console. Ruolo assegnato alla configurazione dell'organizzazione Adobe.</td>
 </tr>
 <tr>
  <td><strong>Amministratore prodotto Adobe Admin Console</strong></td>
  <td>Responsabile del diritto degli utenti al prodotto di Marketo Engage in Adobe Admin Console. Ruolo concesso in Adobe Admin Console.</td>
 </tr>
 <tr>
  <td><strong>Amministratore prodotto Marketo Engage</strong></td>
  <td>Persona a cui è stato concesso l’accesso al Marketo Engage con privilegi amministrativi. Ruolo concesso nel Marketo Engage, non in Adobe Admin Console.</td>
 </tr>
 <tr>
  <td><strong>Utente Marketo Engage</strong></td>
  <td>Persona a cui è stato concesso l'accesso al Marketo Engage. Nessun privilegio amministrativo.</td>
 </tr>
</table>

## Domande frequenti

**Che cos’è l’identità Adobe?**

Adobe Identity Management System è costituito da tre componenti.

* Servizio Adobe Identity: Gestisce l’autenticazione e la convalida dell’utente finale, inclusa la federazione e il runtime Single-Sign-On (SSO).

* Adobe Admin Console: L’Admin Console fornisce una posizione centrale per la gestione delle adesioni Adobe in tutta l’organizzazione. Gestisce la gestione degli utenti, il servizio cloud, l’adesione alla licenza del desktop, la configurazione della federazione e fornisce funzioni di sicurezza per la prevenzione della perdita dei dati.

* API di gestione utenti di Adobe (UMAPI): Consente alle organizzazioni di gestire gli utenti e le adesioni aziendali in Adobe Admin Console a livello di API.

**Quando saranno integrati gli abbonamenti a Marketi Engage esistenti con IMS?**

Gli abbonamenti Marketo esistenti verranno migrati al sistema Adobe Identity Management nel corso di quest&#39;anno. Il supporto Marketo non sarà in grado di fornire aggiornamenti sulla migrazione ad Adobe IMS. Nei prossimi mesi, il Customer Success Manager contatterà la tempistica stimata.

**Qual è la differenza tra un amministratore di prodotto Adobe e un amministratore di Marketo Engage?**

* Adobe Product Admin è un nuovo ruolo nella piattaforma Marketo.
* Ad Adobe, il ruolo di amministratore prodotto viene assegnato agli utenti aggiunti come amministratore prodotto in Adobe Admin Console
* Adobe Product Admin è un ruolo di sola lettura e non può essere modificato o eliminato dal Marketo Engage.
* L’amministratore di prodotto di Adobe dispone degli stessi diritti e privilegi di un amministratore Marketo standard.
* Il ruolo dell’amministratore di Marketo Engage è ancora un amministratore e viene concesso a un utente del Marketo Engage.

**C&#39;è qualche modifica nel supporto client API di gestione utenti?**

Sì. Chi è stato effettuato l’accesso ad Adobe IMS non può utilizzare tutte le API di gestione utenti di Marketo esistenti. Per le azioni di invito, aggiornamento ed eliminazione degli utenti, l&#39;Adobe [API IMS](https://www.adobe.io/apis/experienceplatform/umapi-new.html) devono essere utilizzati. Per la gestione dei ruoli, si applicano ancora le API di gestione utenti di Marketo. Oltre a questo, non ci sono altre modifiche al supporto client Marketo REST API.

**Chi contatteremo per richiedere assistenza se siamo integrati con IMS?**

Segui la procedura standard per contattare [Supporto Marketo](https://nation.marketo.com/t5/support/ct-p/Support).

**I ruoli utente di Marketo (all’interno delle aree di lavoro) sono gestiti in Adobe Admin Console?**

No. La gestione del ruolo utente (all’interno delle aree di lavoro) viene completata in Marketo Engage.

**Sono un amministratore Marketo in un abbonamento integrato IMS e non ho accesso all’Admin Console. Come posso accedere?**

Qualsiasi amministratore di prodotto o di sistema di Adobe che ha accesso all’Admin Console della tua organizzazione può concederti l’accesso. Se non sai chi dispone dei privilegi di amministratore nella console all’interno della tua organizzazione, contatta [Adobe Customer Care](https://helpx.adobe.com/contact.html).

**In che modo un amministratore può aggiungere utenti a Marketo Sales Connect?**

Anche se in Admin Console sarà presente una scheda prodotto per Sales Connect, non utilizzare Admin Console per aggiungere/gestire gli utenti. Il seguente collegamento consente agli amministratori di gestire gli utenti tramite Marketo Sales Connect: [https://toutapp.com/next#settings/admin/user-management](https://toutapp.com/next#settings/admin/user-management).

**Dove posso saperne di più su Adobe Admin Console?**

[https://helpx.adobe.com/enterprise/admin-guide.html](https://helpx.adobe.com/enterprise/admin-guide.html).

**Vado ancora alla sezione Amministratore in Marketo per apportare modifiche all’account utente per il mio account?**

No, devi passare a [account.adobe.com](https://account.adobe.com).

**Come funziona questo con Marketo Universal ID?**

Coloro che hanno effettuato l’accesso all’identità Adobe possono accedere facilmente a tutte le iscrizioni IMS tramite lo switcher di abbonamento nel prodotto.

**Questo funziona con SSO?**

Sì. L’integrazione di Marketo con Adobe IMS supporta gli utenti Universal ID e SSO. L’SSO è ora gestito da Adobe IMS ed è configurato a livello di organizzazione in Adobe Admin Console. [Ulteriori informazioni qui](https://helpx.adobe.com/enterprise/using/set-up-identity.html).

**Come funziona l’autorizzazione dei dispositivi?**

Adobe IMS al momento non supporta funzioni simili a quelle di autorizzazione dei dispositivi Marketo.

**È ancora possibile utilizzare la funzione &quot;Login in Invita finestra di dialogo utente&quot; per rendere unico l&#39;accesso di un utente dal suo messaggio e-mail?**

No. Il flusso di lavoro Invito utente non è più attivo quando un abbonamento è abilitato per IMS, pertanto la funzione non è più valida. L’identità di Adobe richiede che l’identità di un utente sia determinata dalla sua e-mail.

**Per Adobe IMS, è possibile utilizzare Adobe ID, Enterprise ID o Federated ID?**

Sì, è possibile determinare il tipo di identità per ottenere il supporto dell&#39;organizzazione. Maggiori informazioni sono disponibili qui: [Panoramica dell’identità](https://helpx.adobe.com/enterprise/using/identity.html) e qui: [Imposta identità](https://helpx.adobe.com/enterprise/using/set-up-identity.html).

>[!MORELIKETHIS]
>
>* [Configurazione amministratore](/help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md)
>* [Aggiungere o rimuovere un amministratore di prodotto](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-product-admin.md)
>* [Aggiungi o rimuovi un utente](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md)

