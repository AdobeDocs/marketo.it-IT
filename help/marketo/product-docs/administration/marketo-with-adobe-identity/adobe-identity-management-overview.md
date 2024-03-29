---
description: Panoramica di Adobe Identity Management - Documentazione di Marketo - Documentazione del prodotto
title: Panoramica di Adobe Identity Management
exl-id: 18ddeebc-bc89-411c-9d2c-23df6841cb3a
feature: Marketo with Adobe Identity
source-git-commit: 6f9790c2243407f2622970d228c9de6be7697df6
workflow-type: tm+mt
source-wordcount: '402'
ht-degree: 0%

---

# Panoramica di Adobe Identity Management {#adobe-identity-management-overview}

Tutte le nuove sottoscrizioni a Adobe Marketo Engage (31 luglio 2023 o versioni successive) sono integrate con il sistema Identity Management di Adobe. È in corso la migrazione degli abbonamenti Marketo esistenti al sistema Identity Management Adobe al momento del rinnovo e/o del riappalto degli eventi. Al momento non sono supportate le migrazioni al di fuori di un evento di rinnovo o di riassegnazione.

>[!NOTE]
>
>Il supporto Marketo non è in grado di fornire aggiornamenti relativi alla migrazione Adobe IMS. Il team dell’account Adobe raggiungerà la tempistica stimata nei prossimi mesi. Per ulteriori informazioni, consulta [questo articolo](/help/marketo/product-docs/administration/marketo-with-adobe-identity/subscription-and-user-migration/understanding-marketo-subscription-and-user-migration-to-the-adobe-admin-console.md){target="_blank"}, and the [Frequently Asked Questions](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}.

Per gli abbonamenti a cui è stato effettuato l’onboarding dell’identità dell’Adobe, Adobe Admin Console viene utilizzato per la gestione degli utenti. Nell’Admin Console sono gestiti anche i concetti relativi all’identità, come Single Sign On.

* Per ulteriori informazioni su [Adobe Admin Console](https://helpx.adobe.com/it/enterprise/using/admin-console.html){target="_blank"}.
* Ulteriori informazioni su [configurazione dell’organizzazione di Adobi relativa all’abbonamento Marketo](https://helpx.adobe.com/enterprise/using/set-up-identity.html){target="_blank"}.

>[!NOTE]
>
>Se desideri implementare il Single Sign-On e l’abbonamento è stato effettuato all’onboarding per Adobe Identity senza l’SSO implementato nell’organizzazione Adobe, invia un ticket a [Supporto Marketo](https://nation.marketo.com/){target="_blank"} e specifica l’argomento come &quot;Marketo su Admin Console, implementazione dell’SSO&quot;.

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

Domande frequenti [si trova qui](/help/marketo/product-docs/administration/marketo-with-adobe-identity/faq.md){target="_blank"}.

>[!MORELIKETHIS]
>
>* [Configurazione amministratore](/help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md){target="_blank"}
>* [Aggiungere o rimuovere un amministratore di prodotto](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-product-admin.md){target="_blank"}
>* [Aggiungere o rimuovere un utente](/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md){target="_blank"}
