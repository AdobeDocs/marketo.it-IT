---
description: NUOVA AREA - Documentazione di Marketo - Documentazione del prodotto
title: NUOVA AREA
hide: true
hidefromtoc: true
feature: Getting Started
exl-id: c7b068fc-a038-4f9c-a037-72440a1a864e
source-git-commit: 14ccfe39059b9c900a5e5e00b082146bb500d79d
workflow-type: tm+mt
source-wordcount: '1113'
ht-degree: 1%

---

# NUOVA AREA: Elenco di controllo amministratore {#new-area-admin-checklist}

Testo introduttivo.

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
    <td><li>Esamina i ruoli predefiniti e conferma le autorizzazioni/l’accesso di ciascun ruolo.<br><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#create-a-new-role" target="_blank">Crea un nuovo ruolo</a> o <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#edit-a-role" target="_blank">modificare i ruoli</a> in base alle esigenze della tua organizzazione e alla frequenza di accesso degli utenti.<br><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html%22%20/l%20%22assign-roles-to-a-user" target="_blank">Assegnare gli utenti ai ruoli appropriati</a>. Gli utenti devono essere aggiunti all’abbonamento in Adobe Admin Console prima di concedere i loro ruoli in Ruoli. Consultare la sezione "Utenti" nell'elenco di controllo "Initial Setup" [LINK]. <br>Dopo aver assegnato i ruoli agli utenti, controlla il numero di utenti per ruolo.<br>Implementa un ruolo univoco per ogni utente API per facilitare la risoluzione dei problemi.</td>
  </tr>
  <tr>
    <td>Documentazione</td>
    <td>Definisci utenti e ruoli per la tua organizzazione.<br>Definisci il processo per aggiungere un nuovo utente/amministratore.</td>
  </tr>
  <tr>
    <td>Sandbox (se applicabile)</td>
    <td>Controlla le categorie precedenti per la sandbox, se ne hai una.</td>
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
    <td>Determinare il numero di<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.html" target="_blank"> workspace</a> e/o le partizioni che la tua organizzazione deve avere e <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.html" target="_blank">quanti utenti hanno accesso a ogni area di lavoro.</a><br>Definire lo scopo principale di ogni area di lavoro e partizione.<br>Definire la relazione tra aree di lavoro e partizioni.</td>
  </tr>
  <tr>
    <td>Documentazione</td>
    <td>Documentare la definizione delle aree di lavoro e le correlazioni con le partizioni del database (ovvero un'area di lavoro globale che vede tutti, rispetto ai settori aziendali). <br>Importare nuovi record nella partizione appropriata.<br>Definisci il valore in CRM che colloca gli utenti nella partizione appropriata.</td>
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
  <tr>
    <th>Area</th>
    <th>Elementi azione</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Impostazioni Smart Campaign</td>
    <td>Aggiungi un <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.html" target="_blank">restrizione alla dimensione di Smart Campaign</a>, evitando di inviare accidentalmente e-mail all'intero database.</td>
  </tr>
  <tr>
    <td>Documentazione</td>
    <td>Documentare la definizione delle aree di lavoro e le correlazioni con le partizioni del database (ovvero un'area di lavoro globale che vede tutti, rispetto ai settori aziendali).  <br>Importare nuovi record nella partizione appropriata.<br>Definisci il valore in CRM che colloca gli utenti nella partizione appropriata.</td>
  </tr>
</tbody>
</table>

## Impostazioni e-mail {#email-settings}

<table>
<thead>
  <tr>
    <th style="width:20%">Area</th>
    <th style="width:80%">Elementi azione</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Impostazioni predefinite e-mail</td>
    <td>In Dominio di branding, seleziona il dominio e aggiungi il CNAME e-mail. Deve essere nel formato: [EmailTrackingCNAME].[DominioSocietà].com.  <br><a href="https://experienceleague.adobe.com/en/docs/customer-one/using/home#create-a-support-ticket-with-admin-console" target="_blank">Contatta il supporto Marketo</a> per proteggerlo con il provisioning di un certificato SSL. Il completamento di questo processo può richiedere fino a 3 giorni lavorativi.</td>
  </tr>
  <tr>
    <td>SPF/DKIM</td>
    <td><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/set-up-spf-and-dkim-for-your-email-deliverability.html" target="_blank">Configurazione SPF e DKIM</a> per il recapito messaggi e-mail.</td>
  </tr>
  <tr>
  </tr>
  <tr>
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
    <td>Luogo <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-communication-limits.html" target="_blank" rel="noopener noreferrer">Limiti di comunicazione</a>.<br>Stabilire se l'azienda richiede una policy sui limiti di comunicazione </td>
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
    <td>Definire come utilizzare <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/create-a-program-channel.html" target="_blank" rel="noopener noreferrer">canali</a>.</td>
  </tr>
  <tr>
    <td>Tag</td>
    <td>Definire come utilizzare <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html" target="_blank" rel="noopener noreferrer">tag</a>.</td>
  </tr>
  <tr>
    <td>Calendario (se applicabile)</td>
    <td><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/issue-revoke-a-marketing-calendar-license.html" target="_blank" rel="noopener noreferrer">Postazioni calendario di marketing problema</a> a coloro che hanno bisogno di accedervi. <br>Configurazione <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/navigating-the-marketing-calendar.html" target="_blank" rel="noopener noreferrer">Calendario.</a></td>
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
    <td>Implementare convenzioni di denominazione per <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo.html" target="_blank" rel="noopener noreferrer">campi personalizzati.</a> Ad esempio, inizia con "MKTO".<br>Essere selettivi rispetto ai campi sincronizzati. Più campi vengono sincronizzati, più lento sarà il ciclo di sincronizzazione.<br><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/block-updates-to-a-field.html" target="_blank" rel="noopener noreferrer">Blocca aggiornamenti ai campi</a> si desidera scrivere una volta sola (ad esempio origine lead originale, dettagli origine lead originale, campi UTM di primo contatto, ecc.)</td>
  </tr>
  <tr>
  </tr>
  <tr>
    <td>Attività personalizzate</td>
    <td>Definisci <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-activities/understanding-custom-activities.html">Attività personalizzate</a> specifiche per la tua azienda.  </td>
  </tr>
  <tr>
    <td>Oggetti personalizzati</td>
    <td>Controlla quanti <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.html">Oggetti personalizzati</a> ti serve. <br><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.html">Sincronizza gli oggetti personalizzati con il tuo CRM</a>. </td>
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
    <td>Avvia la sincronizzazione CRM. Scegli una delle seguenti opzioni, a seconda del sistema di gestione delle relazioni con i clienti utilizzato dalla tua azienda: <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/salesforce-sync-setup.html">Salesforce</a> | <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/microsoft-dynamics-sync-setup.html">Microsoft Dynamics</a>. <br>Identifica il tipo di accesso necessario per accedere al CRM. <br>Identifica il tuo amministratore CRM per la risoluzione dei problemi. </td>
  </tr>
  <tr>
    <td>Pagine di destinazione</td>
    <td>NOTA: sei cliente di Launch Pack? Puoi saltare questo passaggio. Il tuo consulente ti fornirà un documento con le istruzioni per la configurazione IT durante la tua chiamata di avvio. <br>Imposta il dominio della pagina di destinazione con un <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/edit-landing-page-settings.html">CNAME</a> e <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/edit-landing-page-settings.html">immettere informazioni sul dominio e sulla pagina</a>. Deve essere nel formato: [LandingPageCNAME].[DominioSocietà].com <br>Scegli un CNAME per le pagine di destinazione. Alcuni esempi: <br>* **vai**.[DominioSocietà].com <br>* **www2**.[DominioSocietà].com <br>* **lp**.[DominioSocietà].com <br><a href="https://experienceleague.adobe.com/en/docs/customer-one/using/home#create-a-support-ticket-with-admin-console">Contatta il supporto Marketo</a> per avviare il processo di provisioning di un certificato SSL. Il completamento di questo processo può richiedere fino a 3 giorni lavorativi. <br>SUGGERIMENTO: Sii breve! Gli URL più brevi sono più facili da ricordare. Consigliamo di usare "go" come dominio. <br>Aggiungi il codice di tracciamento di Analytics (ad esempio, Google Analytics o Adobe Analytics) ai modelli della pagina di destinazione. </td>
  </tr>
  <tr>
    <td>Munchkin</td>
    <td>NOTA: se sei un cliente Launch Pack, salta questo passaggio. Il tuo consulente ti fornirà le istruzioni relative al codice Munchkin nel tuo documento di istruzioni per la configurazione IT. <br><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.html">Aggiungi codice di tracciamento Munchkin</a> sul tuo sito web. Il codice Munchkin può essere <a href="https://developers.marketo.com/javascript-api/lead-tracking/">hardcoded</a> o implementato tramite Google Tag Manager.  </td>
  </tr>
  <tr>
    <td>Servizi Web</td>
    <td>Abilita <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.html">le restrizioni IP</a> se applicabile. <br>Determinare gli utenti/le app che possono <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/create-an-api-only-user.html">Chiamate API</a> nella tua istanza. <br>Controlla tutte le app che effettueranno chiamate API e determina se è necessario un aumento o un taglio per le chiamate API.  </td>
  </tr>
  <tr>
    <td>LaunchPoint</td>
    <td>Configurazione richiesta <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.html">LaunchPoint</a> servizi per la tua azienda. Per facilitare la risoluzione dei problemi, ogni LaunchPoint deve essere associato a un utente API univoco.  </td>
  </tr>
  <tr>
    <td>Webinar interattivi (se applicabile)</td>
    <td>NOTA: il provisioning dei webinar interattivi viene eseguito solo per le istanze di produzione. <br>Per la creazione di webinar interattivi, la funzione integrata del webinar, <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/events/interactive-webinars/user-and-license-management">aggiungere utenti alla sezione 'Utente'</a> nella scheda Webinar interattivo. </td>
  </tr>
  <tr>
    <td>Adobe Dynamic Chat (se applicabile)</td>
    <td>Per l’utilizzo di <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.html">Dynamic Chat</a>, il canale di automazione della conversazione nativo in Marketi Engage, procederai con la configurazione delle autorizzazioni utente seguendo i passaggi seguenti su <a href="https://adminconsole.adobe.com/">Adobe Admin Console</a>. <br>Conferma se l’amministratore di sistema dell’organizzazione di Adobe ti ha assegnato un ruolo di amministratore di prodotto Adobe. Contatto <a href="https://helpx.adobe.com/contact.html">Assistenza clienti Adobe</a> per scoprire chi dispone dei privilegi di amministratore nella console all’interno della tua organizzazione. <br>Accetta <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html">l’invito "Amministratore prodotto di Dynamic Chat"</a>. Il <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html">e-mail di benvenuto</a> viene inviato quando il Dynamic Chat è abilitato nell’istanza del Marketo Engage e si è designati come amministratore di sistema.  <br>Assegna tutti gli utenti appropriati al profilo di prodotto del Dynamic Chat in Adobe Admin Console. <br>Se un utente indesiderato viene aggiunto a più profili di prodotto, devi eliminarlo da tutti i profili di prodotto. In caso contrario, avranno comunque accesso al Dynamic Chat. <br>È possibile <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#edit-existing-permissions">modificare i profili di prodotto nel Dynamic Chat</a> e creare un profilo personalizzato con un set personalizzato di <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions#list-of-permissions">autorizzazioni disponibili nell’abbonamento</a>. <br>Assegna utenti a <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users#add-dynamic-chat-access-to-marketo-role">Ruoli "Dynamic Chat di accesso"</a> in Marketo Engage/Amministratore/Utenti e ruoli. </td>
  </tr>
  <tr>
    <td>Informazioni sulla vendita (se applicabile)</td>
    <td><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide#set-up-marketo-sales-account">Imposta azione approfondimento vendite</a> in Informazioni sulla vendita&gt;Configurazione azioni.  <br><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html#invite-individual-users-to-msi-actions">Rilasciare posti agli utenti appropriati.</a>  <br><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.html">Configurare l’API</a>. <br><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.html">Personalizza i punteggi dei lead.</a> </td>
  </tr>
  <tr>
    <td>Sales Connect (se applicabile)</td>
    <td><a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-sales-connect/getting-started/accessing-your-new-sales-connect-instance">Invita gli amministratori di Marketo Engage appropriati nell'istanza Sales Connect</a>. <br>Completa il <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/marketo-sales-connect/getting-started/getting-started-guide-for-sales-connect-admins">configurazione aggiuntiva dell'amministratore Sales Connect</a> in Sales Connect e Salesforce. </td>
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
    <td><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/enable-or-disable-treasure-chest-features.html">Abilita cassa del tesoro</a> per sperimentare le funzioni di guida.  <br>Determinare le feature da attivare o disattivare. </td>
  </tr>
  <tr>
    <td>Ispettore campagna </td>
    <td><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/campaign-inspector.html">Attiva Campaign Inspector</a> per visualizzare tutte le campagne avanzate contemporaneamente. </td>
  </tr>
</tbody>
</table>
