---
description: Panoramica di Adobe Identity Management per Marketo Engage, inclusi i tempi di migrazione, la gestione degli utenti e i livelli di profilo, ad esempio Amministratore di sistema e Amministratore di prodotto.
title: Panoramica su Identity Management di Adobe
exl-id: 18ddeebc-bc89-411c-9d2c-23df6841cb3a
feature: Marketo with Adobe Identity
source-git-commit: c06481152e88b8760a4539842a91aea90ab07fa1
workflow-type: tm+mt
source-wordcount: '366'
ht-degree: 6%

---

# Panoramica su Identity Management di Adobe {#adobe-identity-management-overview}

Tutte le nuove sottoscrizioni a Adobe Marketo Engage (31 luglio 2023 o versioni successive) sono integrate con Adobe Identity Management System.

Per gli abbonamenti a cui è stato effettuato l’onboarding in Adobe identity, Adobe Admin Console viene utilizzato per la gestione degli utenti. I concetti relativi all’identità, come il Single Sign-On, vengono gestiti anche in Admin Console.

* Ulteriori informazioni su [Adobe Admin Console](https://helpx.adobe.com/it/enterprise/using/admin-console.html){target="_blank"}.
* Ulteriori informazioni sulla [configurazione dell&#39;organizzazione Adobe relativa alla sottoscrizione a Marketo](https://helpx.adobe.com/it/enterprise/using/set-up-identity.html){target="_blank"}.

>[!NOTE]
>
>Se desideri implementare il Single Sign-On e il tuo abbonamento è stato acquisito a Adobe Identity senza SSO implementato nell&#39;organizzazione Adobe, invia un ticket al [Supporto Marketo](https://nation.marketo.com/){target="_blank"} e specifica l&#39;argomento come &quot;Marketo su Admin Console, implementazione del SSO&quot;.

## Livelli di profilo {#profile-levels}

Gli abbonamenti Adobe Marketo Engage inseriti nel sistema Adobe Identity Management supportano vari profili. Di seguito sono elencati i tipi di profili utente rilevanti per questa integrazione.

<table>
 <tr>
  <td><strong>Amministratore di sistema Adobe Admin Console</strong></td>
  <td>Responsabile dell’impostazione dei concetti di identità per l’organizzazione Adobe e il prodotto Marketo Engage in Adobe Admin Console. Ruolo assegnato nella configurazione dell’organizzazione Adobe.</td>
 </tr>
 <tr>
  <td><strong>Amministratore di prodotto Adobe Admin Console</strong></td>
  <td>Responsabile dell’assegnazione di diritti agli utenti per il prodotto Marketo Engage in Adobe Admin Console. Ruolo assegnato in Adobe Admin Console.</td>
 </tr>
 <tr>
  <td><strong>Amministratore del profilo di prodotto Adobe Admin Console</strong></td>
  <td>Responsabile dell’amministrazione degli utenti all’interno di un profilo di prodotto. Non possono gestire gli utenti al di fuori di quel profilo specifico. Un amministratore del profilo di prodotto non ha accesso all’applicazione Marketo a meno che non venga aggiunto al profilo di prodotto come utente. Il loro ruolo rimarrebbe quello di utente standard (area di lavoro predefinita se ne esistono più di una).
</td>
 </tr>
 <tr>
  <td><strong>Amministratore Marketo Engage</strong></td>
  <td>Persona che ha ottenuto l’accesso a Marketo Engage con privilegi di amministratore. Ruolo assegnato in Marketo Engage, non in Adobe Admin Console (viene visualizzato solo come "Amministratore" nella finestra modale <b>Modifica utente</b>).</td>
 </tr>
 <tr>
  <td><strong>Utente Marketo Engage</strong></td>
  <td>Persona a cui è stato concesso l’accesso a Marketo Engage. Nessun privilegio amministrativo.</td>
 </tr>
</table>

>[!MORELIKETHIS]
>
>* [Installazione amministratore](/help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md){target="_blank"}
>* [Aggiungi o rimuovi amministratore prodotto](/help/marketo/product-docs/administration/users-and-roles/add-or-remove-a-product-admin.md){target="_blank"}
>* [Aggiungere o rimuovere un utente](/help/marketo/product-docs/administration/users-and-roles/add-or-remove-a-user.md){target="_blank"}
