---
description: Imposta la sezione Amministratore per la nuova istanza di Marketo Engage.
title: Best practice per le nuove istanze - Elenco di controllo sezione amministratore
feature: Getting Started
exl-id: 4fa90a32-7e97-404c-90b1-90d05c2561d0
source-git-commit: df8087dbaf2b621d0d877eba1c16f160ee9bf460
workflow-type: tm+mt
source-wordcount: '634'
ht-degree: 1%

---

# Best practice per le nuove istanze: elenco di controllo sezione amministratore {#new-instance-best-practices-admin-section-checklist}

In qualità di nuovo amministratore che naviga in una nuova istanza del Marketo Engage, applica l’elenco di controllo seguente per aiutarti a guidare attraverso il processo di implementazione. Come per tutte queste guide, puoi anche [scaricare le liste di controllo](/help/marketo/getting-started/implementing-a-new-marketo-engage-instance/assets/adobe-marketo-engage-new-instance-admin-checklist.xlsx) e tenere traccia dei tuoi progressi.

## Ruoli {#roles}

<table>
<thead>
  <tr>
    <th style="width:20%">Area</th>
    <th style="width:80%">Elementi azione</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Ruoli</td>
    <td><li>Esamina i ruoli predefiniti e conferma le autorizzazioni/l’accesso di ciascun ruolo.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html?lang=it#create-a-new-role" target="_blank">Crea un nuovo ruolo</a> o <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html?lang=it#edit-a-role" target="_blank">modifica i ruoli</a> in base alle esigenze della tua organizzazione.</li>
    <li><a href="https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions#assign-roles-to-a-user" target="_blank">Assegnare gli utenti ai ruoli appropriati</a>. Gli utenti devono essere aggiunti all’abbonamento in Adobe Admin Console prima di concedere i loro ruoli in "Ruoli". Fare riferimento alla sezione Utenti nell'<a href="/help/marketo/getting-started/initial-setup/user-setup.md">Elenco di controllo installazione iniziale</a>.</li>
    <li>Dopo aver assegnato i ruoli agli utenti, controlla il numero di utenti per ruolo.</li>
    <li>Implementa un ruolo univoco per ogni utente API per facilitare la risoluzione dei problemi.</li></td>
  </tr>
  <tr>
    <td>Sandbox (se applicabile)</td>
    <td><li>Controlla le categorie qui sopra per la tua <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/marketo-sandbox.md" target="_blank">sandbox</a>.</li></td>
  </tr>
</tbody>
</table>

## Aree di lavoro e partizioni {#workspaces-partitions}

<table>
<thead>
  <tr>
    <th style="width:20%">Area</th>
    <th style="width:80%">Elementi azione</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Aree di lavoro e partizioni (se applicabile)</td>
    <td><li>Determina il numero di <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.html?lang=it" target="_blank"> aree di lavoro</a> e/o partizioni necessarie per l'organizzazione e <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.html?lang=it" target="_blank">quanti utenti hanno accesso a ogni area di lavoro.</a></li>
    <li>Definire lo scopo principale di ogni area di lavoro e partizione.</li>
    <li>Definire la relazione tra aree di lavoro e partizioni.</li></td>
  </tr>
</tbody>
</table>

## Impostazioni Smart Campaign {#smart-campaign-settings}

<table>
<thead>
  <tr>
    <th style="width:20%">Area</th>
    <th style="width:80%">Elementi azione</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Impostazioni Smart Campaign</td>
    <td><li>Aggiungi una <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.html?lang=it" target="_blank">restrizione alle dimensioni di Smart Campaign</a>, per evitare di inviare accidentalmente e-mail all'intero database.</li></td>
  </tr>
</tbody>
</table>

## Limiti di comunicazione {#communication-limits}

<table>
<thead>
  <tr>
    <th style="width:20%">Area</th>
    <th style="width:80%">Elementi azione</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Limiti di comunicazione</td>
    <td><li>Implementare <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-communication-limits.html?lang=it" target="_blank">limiti di comunicazione</a>.</li>
    <li>Determina se la tua azienda richiede una politica sui limiti di comunicazione.</li></td>
  </tr>
</tbody>
</table>

## Tag {#tags}

<table>
<thead>
  <tr>
    <th style="width:20%">Area</th>
    <th style="width:80%">Elementi azione</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Canali</td>
    <td><li>Definisci come utilizzare <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/create-a-program-channel.html?lang=it" target="_blank">canali</a>.</li></td>
  </tr>
  <tr>
    <td>Tag</td>
    <td><li>Definisci come utilizzare <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html?lang=it" target="_blank">tag</a>.</li></td>
  </tr>
  <tr>
    <td>Calendario<br> 
    (se applicabile)</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/issue-revoke-a-marketing-calendar-license.html?lang=it" target="_blank">Invia la Issue alle postazioni del Calendario di Marketing</a> per coloro che hanno bisogno di accedervi.</li>
    <li>Configura il <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/navigating-the-marketing-calendar.html?lang=it" target="_blank">Calendario</a>.</li></td>
  </tr>
</tbody>
</table>

## Gestione database {#database-management}

<table>
<thead>
  <tr>
    <th style="width:20%">Area</th>
    <th style="width:80%">Elementi azione</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Gestione dei campi</td>
    <td><li>Implementa una convenzione di denominazione per <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo.html?lang=it" target="_blank">campi personalizzati</a> (ad esempio, a partire da "MKTO").</li>
    <li>Essere selettivi rispetto ai campi sincronizzati. Più campi vengono sincronizzati, più lento sarà il ciclo di sincronizzazione.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/block-updates-to-a-field.html?lang=it" target="_blank">Blocca aggiornamenti ai campi</a> che si desidera scrivere una sola volta (ad esempio origine lead originale, dettagli origine lead originale, campi UTM di primo contatto, ecc.).</li></td>
  </tr>
  <tr>
    <td>Attività personalizzate</td>
    <td><li>Definisci <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-activities/understanding-custom-activities.html?lang=it" target="_blank">Attività personalizzate</a> specifiche per la tua azienda.</li></td>
  </tr>
  <tr>
    <td>Oggetti personalizzati</td>
    <td><li>Controlla quanti <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.html?lang=it" target="_blank">oggetti personalizzati</a> sono necessari.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.html?lang=it" target="_blank">Sincronizza gli oggetti personalizzati</a> con il tuo CRM.</li></td>
  </tr>
</tbody>
</table>

## Integrazioni {#integrations}

<table>
<thead>
  <tr>
    <th style="width:20%">Area</th>
    <th style="width:80%">Elementi azione</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>CRM </td>
    <td><li>Identifica le autorizzazioni necessarie per accedere al CRM.</li>
    <li>Identifica il tuo amministratore CRM per la risoluzione dei problemi.</li></td>
  </tr>
  <tr>
    <td>Servizi Web</td>
    <td><li>Determina gli utenti/app che possono effettuare <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/create-an-api-only-user.html?lang=it" target="_blank">chiamate API</a> nella tua istanza.</li>
    <li>Controlla tutte le app che effettueranno chiamate API e determina se è necessario un aumento o una diminuzione delle chiamate API.</li></td>
  </tr>
  <tr>
    <td>LaunchPoint</td>
    <td><li>Configura i servizi <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.html?lang=it" target="_blank">LaunchPoint</a> per la tua azienda. Per facilitare la risoluzione dei problemi, ogni LaunchPoint deve essere associato a un utente API univoco.</li></td>
  </tr>
  <tr>
    <td>Webinar interattivi (se applicabile)</td>
    <td><li>Per la creazione di webinar interattivi, la funzionalità integrata del Marketo Engage, <a href="https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/demand-generation/events/interactive-webinars/user-and-license-management" target="_blank">aggiungere utenti alla sezione 'Utente'</a> della scheda Webinar interattivo.</li>
    <p><img src="assets/note-icon.png" alt="icona nota"> NOTA: il provisioning dei webinar interattivi viene eseguito solo per le istanze di produzione.</td>
  </tr>
  <tr>
    <td>Adobe Dynamic Chat (se applicabile)</td>
    <td><li>Assegnare gli utenti a <a href="https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users#add-dynamic-chat-access-to-marketo-role" target="_blank"> ruoli 'Dynamic Chat di accesso'</a> in Marketo Engage &gt; Amministratore &gt; Utenti e ruoli.</li></td>
  </tr>
  <tr>
    <td>Informazioni sulla vendita (se applicabile)</td>
    <td><li><a href="https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide#set-up-marketo-sales-account" target="_blank">Configura azione approfondimento vendite</a> in Insight vendite &gt; Configurazione azioni.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html?lang=it#invite-individual-users-to-msi-actions" target="_blank">Postazioni problema</a> per gli utenti appropriati.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.html?lang=it" target="_blank">Configura l'API</a>.</li>
    <li>Personalizza i <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.html?lang=it" target="_blank">punteggi di lead</a>.</li></td>
  </tr>
  <tr>
    <td>Sales Connect (se applicabile)</td>
    <td><li>Invita gli amministratori di Marketo Engage appropriati nell'<a href="https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/marketo-sales-connect/getting-started/accessing-your-new-sales-connect-instance" target="_blank">istanza Sales Connect</a>.</li>
    <li>Completare la <a href="https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/marketo-sales-connect/getting-started/getting-started-guide-for-sales-connect-admins" target="_blank">configurazione aggiuntiva dell'amministratore di Sales Connect</a> in Sales Connect e Salesforce.</li></td>
  </tr>
  <tr>
    <td>Webhook (se applicabile)</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/create-a-webhook.html?lang=it" target="_blank">Crea i webhook</a> richiesti per la tua azienda.</li>
    </td>
  </tr>
</tbody>
</table>

## Treasure Chest {#treasure-chest}

<table>
<thead>
  <tr>
    <th style="width:20%">Area</th>
    <th style="width:80%">Elementi azione</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Treasure Chest </td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/enable-or-disable-treasure-chest-features.html?lang=it" target="_blank">Abilita Treasure Chest</a> per sperimentare le funzionalità pilota.</li>
    <li>Determinare le feature che si desidera attivare o disattivare.</li></td>
  </tr>
  <tr>
    <td>Ispettore campagna </td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/campaign-inspector.html?lang=it" target="_blank">Attiva Campaign Inspector</a> per visualizzare tutte le campagne Smart in un'unica posizione.</li></td>
  </tr>
</tbody>
</table>
