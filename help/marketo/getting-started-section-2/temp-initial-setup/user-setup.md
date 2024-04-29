---
description: Elenco di controllo per la configurazione anticipata - Documentazione di Marketo - Documentazione del prodotto
title: Elenco di controllo per la configurazione anticipata
hide: true
hidefromtoc: true
feature: Getting Started
exl-id: c7b068fc-a038-4f9c-a037-72440a1a864e
source-git-commit: 8473c4d59210bb18c3968a56883034febf00c320
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 0%

---

# NUOVA AREA: elenco di controllo per la configurazione anticipata {#early-setup-checklist}

Testo introduttivo.

## Marketo Engage su Adobe Identity Management {#marketo-engage-on-adobe-identity-management}

<table>
<thead>
  <tr>
    <th style="width:20%">Area</th>
    <th style="width:80%">Elementi azione</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Amministratore prodotti abbonamento e Marketo Engage </td>
    <td><li>Conferma di aver ottenuto un ruolo di amministratore di prodotto Adobe dall’amministratore di sistema dell’organizzazione Adobe.</li>  
    <ul>
    <li>Contatto <a href="https://helpx.adobe.com/contact.html">Assistenza clienti Adobe</a> per scoprire chi dispone di <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html">Amministratore di sistema Adobe Admin Console</a> privilegi.</li></ul>
    <li>Accetta l’invito "Amministratore di prodotto di Marketo Engage" per attivare il tuo Adobe ID. Il <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/admin-setup.html?lang=en#create-a-product-profile">e-mail di benvenuto</a> viene inviato quando il ruolo viene assegnato in Adobe Admin Console.</li></td>
  </tr>
  <tr>
    <td>Profili di prodotto</td>
    <td><li>Assegna tutti gli utenti appropriati al Marketo Engage <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/admin-setup#create-a-product-profile">Profilo prodotto</a> in Adobe Admin Console.</li>
    <ul>
    <li>Non puoi assegnare i ruoli degli utenti in Marketo Engage/Amministratore/Utenti e ruoli prima di aggiungerli a un profilo di prodotto.</li>
    <li>Ogni abbonamento sarà un profilo di prodotto autonomo. Se un utente indesiderato viene aggiunto a più profili di prodotto (ad esempio, sandbox di produzione e di test), devi eliminarlo da tutti i profili di prodotto. In caso contrario, avranno comunque accesso al Marketo Engage.</li></ul></td>
  </tr>
  <tr>
    <td>Utenti</td>
    <td><li>Creare un criterio per determinare quando <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.html">creare un utente</a>.</li> <li>Crea un criterio per determinare quando rimuovere gli utenti.</li>
    <li>Determina chi deve avere <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html">Adobe di autorizzazioni di amministratore di sistema e amministratore di prodotto di Marketo Engage.</a> <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user">Aggiungi utenti</a> al profilo di prodotto desiderato.</li>
    <li>Crea un utente API per ogni caso d’uso dell’API.</li></td>
  </tr>
  <tr>
    <td>Amministratore del supporto del prodotto </td>
    <td><li>A <a href="https://experienceleague.adobe.com/docs/customer-one/using/home.html#create-a-support-ticket-with-admin-console">inviare un ticket di supporto in Adobe Admin Console</a>, è necessario che il ruolo di "Amministratore del supporto del prodotto" sia assegnato da un amministratore di sistema agli abbonamenti da gestire. Solo un amministratore di sistema della tua organizzazione può <a href="https://experienceleague.adobe.com/docs/customer-one/using/home.html#assign-the-support-admin-role">ti assegna a questa mansione</a>.</li>
    <li>È possibile che l'amministratore di sistema ti abbia inviato un'e-mail per informarti di essere l'amministratore del supporto per l'abbonamento al Marketo Engage. In tal caso, fare clic su <a href="https://experienceleague.adobe.com/en/docs/customer-one/using/home#assign-the-support-admin-role">"Inizia" nell’e-mail</a> per aderire all’organizzazione.</li>
    <li>Determinare i contatti appropriati (con almeno un contatto di backup) e chiedere all'amministratore di sistema di assegnare il ruolo di amministratore del supporto del prodotto in anticipo.</li></td>
  </tr>
</tbody>
</table>

## Dynamic Chat nella configurazione di Adobe Identity Management {#dynamic-chat-on-adobe-identity-management}

TESTO

<table>
<thead>
  <tr>
    <th style="width:20%">Area</th>
    <th style="width:80%">Elementi azione</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Amministratore prodotto Dynamic Chat e abbonamento (se applicabile) </td>
    <td><li>Conferma se l’amministratore di sistema dell’organizzazione di Adobe ti ha assegnato un ruolo di amministratore di prodotto Adobe. Contatto <a href="https://helpx.adobe.com/contact.html">Assistenza clienti Adobe</a> per scoprire chi dispone dei privilegi di amministratore nella console all’interno della tua organizzazione.</li>
    <li>Accetta <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html">l’invito "Amministratore prodotto di Dynamic Chat"</a>. Il <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html">e-mail di benvenuto</a> viene inviato quando il Dynamic Chat è abilitato nell’istanza del Marketo Engage e si è designati come amministratore di sistema.</li></td>
  </tr>
  <tr>
    <td>Profili di prodotto </td>
    <td><li>Assegna tutti gli utenti appropriati al profilo di prodotto del Dynamic Chat in Adobe Admin Console.</li> 
    <ul>
    <li>Se un utente indesiderato viene aggiunto a più profili di prodotto, devi eliminarlo da tutti i profili di prodotto. In caso contrario, avranno comunque accesso al Dynamic Chat.</li>
    <li>È possibile <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#edit-existing-permissions">modificare i profili di prodotto nel Dynamic Chat</a> e creare un profilo personalizzato con un set personalizzato di <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#list-of-permissions">autorizzazioni disponibili nell’abbonamento</a>.</li></td>
  </tr>
  <tr>
    <td>Utenti </td>
    <td><li>Crea un criterio per specificare quando aggiungere e rimuovere un utente chat.</li>
    <li>Crea un criterio per stabilire chi deve avere <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup#access-admin-console">Adobe Dynamic Chat di autorizzazioni di amministratore di prodotto.</a></li>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users#add-a-chat-user">Aggiungere utenti al profilo di prodotto desiderato</a>.</li></td>
  </tr>
</tbody>
</table>

## Aggiornamenti continui del sistema e comunicazioni

<table>
<thead>
  <tr>
    <th style="width:20%">Area</th>
    <th style="width:80%">Elementi azione</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Adobe di aggiornamenti dello stato di Marketo </td>
    <td><li><a href="https://status.adobe.com/cloud/experience_cloud">Iscriviti agli aggiornamenti relativi allo stato dei Adobe Marketo Engage</a>.</li></td>
  </tr>
  <tr>
    <td>Notifiche </td>
    <td><li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications#subscribe-to-notifications">Iscriviti alle notifiche dell’amministratore</a> per problemi critici come errori nelle campagne avanzate e problemi critici rilevati con la sincronizzazione CRM.</li></td>
  </tr>
</tbody>
</table>
