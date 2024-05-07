---
description: Prima di immergerti nella nuova istanza di Marketo Engage, devi completare alcuni passaggi fondamentali per un utilizzo continuo. Questi passaggi includono la configurazione dell’account utente, l’impostazione dell’amministratore di supporto e la sottoscrizione agli aggiornamenti di sistema in corso.
title: Elenco di controllo per l'impostazione dell'utente
feature: Getting Started
exl-id: c7b068fc-a038-4f9c-a037-72440a1a864e
source-git-commit: a3d9fcfa0381933e1a7e62f19b414bc380f325b5
workflow-type: tm+mt
source-wordcount: '799'
ht-degree: 0%

---

# Elenco di controllo per l&#39;impostazione dell&#39;utente {#user-setup-checklist}

Ora che hai completato tutte le [passaggi di configurazione iniziali](/help/marketo/getting-started/initial-setup/setup-steps.md){target="_blank"}È ora di stabilire alcuni elementi fondamentali per garantire un utilizzo continuo e senza problemi. In questo modo, il percorso potrà disporre delle basi necessarie per il Marketo Engage e sarà possibile sfruttarne al meglio le funzionalità. Iniziamo!

>[!NOTE]
>
>È inoltre possibile scaricare questa checklist, [insieme a un elenco di best practice](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx) per la nuova istanza, quindi disattiva i passaggi mentre procedi.

## Marketo Engage su Adobe Identity Management {#marketo-engage-on-adobe-identity-management}

I tuoi nuovi abbonamenti al Marketo Engage sono stati integrati in [Sistema Adobe Identity Management (IMS)](https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html). Procedi alla seguente revisione della gestione utenti in Adobe Admin Console.

<table>
<thead>
  <tr>
    <th style="width:20%">Area</th>
    <th style="width:80%">Elementi azione</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Amministratore prodotti abbonamento e Marketo Engage</td>
    <td><li>Conferma di aver ottenuto il ruolo di amministratore di prodotto Adobe dall’amministratore di sistema dell’organizzazione Adobe.</li>  
    <ul>
    <li>Contatta il team dell’account Adobe (il tuo Account Manager) o invia un’e-mail a <code>customercare@marketo.com</code> o invia un messaggio e-mail a customercare@marketo.comto per scoprire chi dispone di <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html">Amministratore di sistema Adobe Admin Console</a> privilegi.</li></ul>
    <li>Accetta l’invito "Amministratore di prodotto di Marketo Engage" per attivare il tuo Adobe ID. Il <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/admin-setup.html?lang=en#create-a-product-profile">e-mail di benvenuto</a> viene inviato quando il ruolo viene assegnato in Adobe Admin Console.</li></td>
  </tr>
  <tr>
    <td>Profili di prodotto</td>
    <td><li>Assegna al Marketo Engage tutti gli utenti desiderati <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/admin-setup#create-a-product-profile">Profilo prodotto</a> in Adobe Admin Console.</li>
    <ul>
    <li>Non puoi assegnare i ruoli degli utenti in Marketo Engage &gt; Amministratore &gt; Utenti e ruoli prima di aggiungerli a un profilo di prodotto.</li>
    <li>Ogni abbonamento sarà un profilo di prodotto autonomo. Se un utente indesiderato viene aggiunto a più profili di prodotto (ad esempio, sandbox di produzione e di test), devi eliminarlo da tutti i profili di prodotto. In caso contrario, avranno comunque accesso al Marketo Engage.</li></ul></td>
  </tr>
  <tr>
    <td>Utenti</td>
    <td><li>Creare un criterio per determinare quando <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.html">creare un utente</a>.</li> <li>Crea un criterio per determinare quando rimuovere gli utenti.</li>
    <li>Determina chi deve avere <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html">Adobe di autorizzazioni di amministratore di sistema e amministratore di prodotto di Marketo Engage.</a> <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user">Aggiungi utenti</a> al profilo di prodotto desiderato.</li>
    <li>Crea un utente API per ogni caso d’uso dell’API.</li></td>
  </tr>
  <tr>
    <td>API User Management (se applicabile)</td>
    <td><li>Utilizza il <a href="https://www.adobe.io/apis/experienceplatform/umapi-new.html">API per la gestione degli utenti Adobe</a> per invitare, aggiornare ed eliminare utenti.</li>
    <li>Utilizza il <a href="https://developer.adobe.com/umapi/">API per la gestione degli utenti Adobe</a> per aggiungere o rimuovere ruoli (ad esempio, Amministratori, Amministratori di supporto, Sviluppatori).</li>
    </td>
  </tr>
  <tr>
    <td>Amministratore del supporto del prodotto</td>
    <td><li>A <a href="https://experienceleague.adobe.com/docs/customer-one/using/home.html#create-a-support-ticket-with-admin-console">inviare un ticket di supporto in Adobe Admin Console</a>, è necessario che il ruolo di "Amministratore del supporto del prodotto" sia assegnato da un amministratore di sistema agli abbonamenti da gestire. Solo un amministratore di sistema della tua organizzazione può <a href="https://experienceleague.adobe.com/docs/customer-one/using/home.html#assign-the-support-admin-role">ti assegna a questa mansione</a>.</li>
    <li>È possibile che l'amministratore di sistema ti abbia inviato un'e-mail per informarti di essere l'amministratore del supporto per l'abbonamento al Marketo Engage. In tal caso, fare clic su <a href="https://experienceleague.adobe.com/en/docs/customer-one/using/home#assign-the-support-admin-role">'Introduzione'</a> nell’e-mail per partecipare all’organizzazione.</li>
    <li>Determinare i contatti appropriati (con almeno un contatto di backup) e chiedere all'amministratore di sistema di assegnare il ruolo di amministratore del supporto del prodotto.</li></td>
  </tr>
</tbody>
</table>

## Dynamic Chat nella configurazione di Adobe Identity Management {#dynamic-chat-on-adobe-identity-management}

Da utilizzare [Dynamic Chat](https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.html), il canale di automazione della conversazione nativo in Marketi Engage, procedi con la configurazione delle autorizzazioni utente seguendo i passaggi riportati di seguito nel [Adobe Admin Console](https://adminconsole.adobe.com/){target="_blank"}.

<table>
<thead>
  <tr>
    <th style="width:20%">Area</th>
    <th style="width:80%">Elementi azione</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Amministratore prodotti abbonamento e Dynamic Chat (se applicabile)</td>
    <td><li>Conferma di aver ottenuto il ruolo di amministratore di prodotto Adobe dall’amministratore di sistema dell’organizzazione Adobe.</li> 
    <ul><li>Contatta il team dell’account Adobe (il tuo Account Manager) o invia un’e-mail a <code>customercare@marketo.com</code> per scoprire chi dispone di <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.html">Amministratore di sistema Adobe Admin Console</a> privilegi.</li></ul>
    <li>Accetta <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html">'Amministratore prodotto di Dynamic Chat'</a> invitare. Il <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html">e-mail di benvenuto</a> viene inviato quando il Dynamic Chat è abilitato nell’istanza del Marketo Engage e si è designati come amministratore di sistema.</li></td>
  </tr>
  <tr>
    <td>Profili di prodotto</td>
    <td><li>Assegna tutti gli utenti desiderati al profilo di prodotto del Dynamic Chat in Adobe Admin Console.</li> 
    <ul>
    <li>Se un utente indesiderato viene aggiunto a più profili di prodotto, devi eliminarlo da tutti i profili di prodotto. In caso contrario, avranno comunque accesso al Dynamic Chat.</li>
    <li>È possibile <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#edit-existing-permissions">modificare i profili di prodotto nel Dynamic Chat</a> e creare un profilo personalizzato con un set personalizzato di <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#list-of-permissions">autorizzazioni disponibili nell’abbonamento</a>.</li></td>
  </tr>
  <tr>
    <td>Utenti</td>
    <td><li>Crea un criterio per specificare quando aggiungere e rimuovere un utente chat.</li>
    <li>Crea un criterio per stabilire chi deve avere <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup#access-admin-console">Adobe Dynamic Chat di autorizzazioni di amministratore di prodotto.</a></li>
    <li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users#add-a-chat-user">Aggiungere utenti al profilo di prodotto desiderato</a>.</li></td>
  </tr>
</tbody>
</table>

## Aggiornamenti di sistema e comunicazioni continui {#system-updates}

<table>
<thead>
  <tr>
    <th style="width:20%">Area</th>
    <th style="width:80%">Elementi azione</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Adobe di aggiornamenti dello stato di Marketo</td>
    <td><li><a href="https://status.adobe.com/cloud/experience_cloud">Iscriviti agli aggiornamenti relativi allo stato dei Adobe Marketo Engage</a>.</li></td>
  </tr>
  <tr>
    <td>Notifiche</td>
    <td><li><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications#subscribe-to-notifications">Iscriviti alle notifiche dell’amministratore</a> per problemi critici come errori nelle campagne avanzate e problemi critici rilevati con la sincronizzazione CRM.</li></td>
  </tr>
</tbody>
</table>

<p>

Ora che il tuo account di Marketo Engage è pronto, rivedi il nostro [Best practice per una nuova istanza di Marketo Engage](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/where-to-start.md){target="_blank"} sezione per trarre il massimo dall’investimento e prepararsi per il successo a lungo termine.
