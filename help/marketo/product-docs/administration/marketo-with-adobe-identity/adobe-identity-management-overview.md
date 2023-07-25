---
description: Panoramica di Adobe Identity Management - Documentazione di Marketo - Documentazione del prodotto
title: Panoramica di Adobe Identity Management
exl-id: 18ddeebc-bc89-411c-9d2c-23df6841cb3a
feature: Marketo with Adobe Identity
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '1087'
ht-degree: 0%

---

# Panoramica di Adobe Identity Management {#adobe-identity-management-overview}

Se a partire dal 15 febbraio 2022 disponi di un nuovo account con Adobe Marketo Engage (nuovo account, non solo una nuova istanza per un account esistente), questo potrebbe essere integrato con Identity Management System di Adobe, a seconda del pacchetto di prodotti acquistato. Per sapere se ne sei in possesso, contatta l’Adobe Account Team (il tuo Account Manager).

Gli abbonamenti Marketo esistenti inizieranno a essere migrati al sistema Identity Management Adobe nella seconda metà del 2023.

>[!NOTE]
>
>Il supporto Marketo non sarà in grado di fornire aggiornamenti relativi alla migrazione Adobe IMS. Il team dell’account Adobe raggiungerà la tempistica stimata nei prossimi mesi.

## Livelli di profilo {#profile-levels}

Gli abbonamenti Adobe Marketo Engage inseriti nel sistema Identity Management di Adobe supportano vari profili. Di seguito sono elencati i tipi di profili utente rilevanti per questa integrazione.

<table>
 <tr>
  <td><strong>Amministratore di sistema Adobe Admin Console</strong></td>
  <td>Responsabile dell’impostazione dei concetti di identità per l’organizzazione di Adobi e il prodotto di Marketo Engage in Adobe Admin Console. Ruolo assegnato nella configurazione dell'organizzazione di Adobe.</td>
 </tr>
 <tr>
  <td><strong>Amministratore di prodotto Adobe Admin Console</strong></td>
  <td>Responsabile dell’assegnazione di diritti agli utenti per il prodotto di Marketo Engage in Adobe Admin Console. Ruolo assegnato in Adobe Admin Console.</td>
 </tr>
 <tr>
  <td><strong>Amministratore del profilo di prodotto Adobe Admin Console</strong></td>
  <td>Responsabile dell’amministrazione degli utenti all’interno di un profilo di prodotto. Non possono gestire gli utenti al di fuori di quel profilo specifico. Un amministratore del profilo di prodotto non ha accesso all’applicazione Marketo a meno che non venga aggiunto al profilo di prodotto come utente. Il loro ruolo rimarrebbe quello di utente standard (area di lavoro predefinita se ne esistono più di una).
</td>
 </tr>
 <tr>
  <td><strong>Amministratore prodotto Marketo Engage</strong></td>
  <td>Una persona a cui è stato concesso l’accesso al Marketo Engage con privilegi amministrativi. Ruolo assegnato nel Marketo Engage, non in Adobe Admin Console.</td>
 </tr>
 <tr>
  <td><strong>Utente Marketo Engage</strong></td>
  <td>Una persona a cui è stato dato accesso al Marketo Engage. Nessun privilegio amministrativo.</td>
 </tr>
</table>

## Domande frequenti {#faq}

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

[https://helpx.adobe.com/enterprise/admin-guide.html](https://helpx.adobe.com/enterprise/admin-guide.html){target="_blank"}.

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

>[!MORELIKETHIS]
>
>* [Configurazione amministratore](/help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md){target="_blank"}
>* [Aggiungere o rimuovere un amministratore di prodotto](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-product-admin.md){target="_blank"}
>* [Aggiungere o rimuovere un utente](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md){target="_blank"}
