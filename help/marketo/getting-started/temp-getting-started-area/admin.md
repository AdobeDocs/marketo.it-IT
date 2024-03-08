---
description: NUOVA AREA - Documentazione di Marketo - Documentazione del prodotto
title: NUOVA AREA
hide: true
hidefromtoc: true
feature: Getting Started
source-git-commit: d65903d64d068a6f919df78258654414f3b76426
workflow-type: tm+mt
source-wordcount: '985'
ht-degree: 2%

---

# NUOVA AREA: Elenco di controllo amministratore {#new-area-admin-checklist}

Testo introduttivo.

## Ruoli {#roles}

<table>
<thead>
  <tr>
    <th>Area</th>
    <th>Elementi azione</th>
    <th>Priorità</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Ruoli</td>
    <td><li>Esamina i ruoli predefiniti e conferma le autorizzazioni/l’accesso di ciascun ruolo.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#create-a-new-role">Crea un nuovo ruolo</a> o <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#edit-a-role">modificare i ruoli</a> in base alle esigenze della tua organizzazione e alla frequenza di accesso degli utenti.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.html#assign-roles-to-a-user">Assegnare gli utenti ai ruoli appropriati</a>.</li>
    <li>Dopo aver assegnato i ruoli agli utenti, controlla il numero di utenti per ruolo.</li>  <li>Implementa un ruolo univoco per ogni utente API per facilitare la risoluzione dei problemi.</li></td>
    <td></td>
  </tr>
  <tr>
    <td>Documentazione</td>
    <td>Definisci utenti e ruoli per la tua organizzazione. <br>Definisci il processo per aggiungere un nuovo utente/amministratore.</td>
    <td></td>
  </tr>
  <tr>
    <td>Sandbox (se applicabile)</td>
    <td>Controlla le categorie precedenti per la sandbox, se ne hai una.</td>
    <td></td>
  </tr>
</tbody>
</table>

## Aree di lavoro e partizioni {#workspaces-partitions}

<table>
<thead>
  <tr>
    <th>Area</th>
    <th>Elementi azione</th>
    <th>Priorità</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Aree di lavoro e partizioni </td>
    <td><li>Determinare il numero di<a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.html"> workspace</a> e/o le partizioni che la tua organizzazione deve avere e <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.html">quanti utenti hanno accesso a ogni area di lavoro.</a></li>
    <li>Definire lo scopo principale di ogni area di lavoro e partizione.</li>
    <li>Definire la relazione tra aree di lavoro e partizioni.</li></td>
    <td></td>
  </tr>
  <tr>
    <td>Documentazione</td>
    <td><li>Documentare la definizione delle aree di lavoro e le correlazioni con le partizioni del database (ovvero un'area di lavoro globale che vede tutti, rispetto ai settori aziendali).</li>
    <li>Importare nuovi record nella partizione appropriata.</li>
    <li>Definisci il valore in CRM che colloca gli utenti nella partizione appropriata.</li></td>
    <td></td>
  </tr>
</tbody>
</table>

## Impostazioni Smart Campaign {#smart-campaign-settings}

<table>
<thead>
  <tr>
    <th>Area</th>
    <th>Elementi azione</th>
    <th>Priorità</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Impostazioni Smart Campaign </td>
    <td><li>Aggiungi un <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.html">restrizione alla dimensione di Smart Campaign</a>, evitando di inviare accidentalmente e-mail all'intero database.</li>
    <li>Abilitare le restrizioni per le persone per le campagne intelligenti</li></td>
    <td></td>
  </tr>
</tbody>
</table>

## Impostazioni e-mail {#email-settings}

<table>
<thead>
  <tr>
    <th>Area</th>
    <th>Elementi azione</th>
    <th>Priorità</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Impostazioni predefinite e-mail</td>
    <td><li>In Dominio di branding, seleziona il dominio e aggiungi il CNAME e-mail. Deve essere nel formato: [EmailTrackingCNAME].[DominioSocietà].com.</li></td>
    <td></td>
  </tr>
  <tr>
    <td>SPF/DKIM</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/email-marketing/deliverability/set-up-spf-and-dkim-for-your-email-deliverability.html">Configurazione SPF e DKIM</a> per il recapito messaggi e-mail.</li></td>
    <td></td>
  </tr>
</tbody>
</table>

## Limiti di comunicazione {#communication-limits}

<table>
<thead>
  <tr>
    <th>Area</th>
    <th>Elementi azione</th>
    <th>Priorità</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Limiti di comunicazione</td>
    <td><li>Luogo <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/email-setup/enable-communication-limits.html">Limiti di comunicazione</a>.</li>
    <li>Stabilisci se la tua azienda richiede una policy sui limiti di comunicazione.</li></td>
    <td></td>
  </tr>
</tbody>
</table>

## Tag {#tags}

<table>
<thead>
  <tr>
    <th>Area</th>
    <th>Elementi azione</th>
    <th>Priorità</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Canali</td>
    <td><li>Definire come utilizzare <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/create-a-program-channel.html">canali</a>.</li></td>
    <td></td>
  </tr>
  <tr>
    <td>Tag </td>
    <td><li>Definire come utilizzare <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html">tag</a>.</li></td>
    <td></td>
  </tr>
  <tr>
    <td>Calendario (se applicabile) </td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/issue-revoke-a-marketing-calendar-license.html">Postazioni calendario di marketing problema</a> a coloro che hanno bisogno di accedervi.</li> 
    <li>Configurazione <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/tags/managing-tag-values.html">Calendario</a>.</li></td>
    <td></td>
  </tr>
</tbody>
</table>

## Gestione database {#database-management}

<table>
<thead>
  <tr>
    <th>Area</th>
    <th>Elementi azione</th>
    <th>Priorità</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Gestione dei campi</td>
    <td><li>Implementare convenzioni di denominazione per <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo.html" target="_blank">campi personalizzati.</a> Ad esempio, inizia con "MKTO".</li>
    <li>Essere selettivi rispetto ai campi sincronizzati. Più campi vengono sincronizzati, più lento sarà il ciclo di sincronizzazione.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/field-management/block-updates-to-a-field.html" target="_blank">Blocca aggiornamenti ai campi</a> si desidera scrivere una volta sola (ad esempio origine lead originale, dettagli origine lead originale, campi UTM di primo contatto, ecc.).</li></td>
    <td></td>
  </tr>
  <tr>
    <td>Attività personalizzate </td>
    <td><li>Definisci <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-activities/understanding-custom-activities.html" target="_blank">Attività personalizzate</a> specifiche per la tua azienda.</li></td>
    <td></td>
  </tr>
  <tr>
    <td>Oggetti personalizzati </td>
    <td><li>Controlla quanti <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.html" target="_blank">Oggetti personalizzati</a> ti serve.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-custom-object-sync.html" target="_blank">Sincronizza gli oggetti personalizzati con il tuo CRM</a>.</li></td>
    <td></td>
  </tr>
</tbody>
</table>

## Integrazioni {#integrations}

<table>
<thead>
  <tr>
    <th>Area</th>
    <th>Elementi azione</th>
    <th>Priorità</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>CRM</td>
    <td><li>Avvia la sincronizzazione CRM. Scegli una delle seguenti opzioni, a seconda del sistema di gestione delle relazioni con i clienti utilizzato dalla tua azienda: <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/salesforce-sync-setup.html" target="_blank">Salesforce</a> | <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/integrations/microsoft-dynamics-sync-setup.html" target="_blank">Microsoft Dynamics</a>.</li>
    <li>Identifica il tipo di accesso necessario per accedere al CRM.</li>
    <li>Identifica il tuo amministratore CRM per la risoluzione dei problemi.</li></td>
    <td></td>
  </tr>
  <tr>
    <td>Informazioni sulla vendita (se applicabile)</td>
    <td><li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html" target="_blank">Imposta Insight vendite.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/actions/getting-started/sales-insight-actions-admin-setup-guide.html#invite-individual-users-to-msi-actions" target="_blank">Rilasciare posti agli utenti appropriati.</a></li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/marketo-sales-insight-configuration-tab-in-salesforce.html" target="_blank">Configurare l’API</a>.</li>
    <li><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/priority-urgency-relative-score-and-best-bets.html" target="_blank">Personalizza i punteggi dei lead.</a></li></td>
    <td></td>
  </tr>
  <tr>
    <td>Pagine di destinazione </td>
    <td>NOTA: sei cliente di Launch Pack? Puoi saltare questo passaggio. Il tuo consulente ti fornirà un documento con le istruzioni per la configurazione IT durante la tua chiamata di avvio. <br>Imposta il dominio della pagina di destinazione con un <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/edit-landing-page-settings.html" target="_blank">CNAME</a> e <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/edit-landing-page-settings.html" target="_blank">immettere informazioni sul dominio e sulla pagina</a>. Deve essere nel formato: [LandingPageCNAME].[DominioSocietà].com <br>Scegli un CNAME per le pagine di destinazione. Alcuni esempi: <br>* **vai**.[DominioSocietà].com <br>* **www2**.[DominioSocietà].com <br>* **lp**.[DominioSocietà].com <br>SUGGERIMENTO: Sii breve! Gli URL più brevi sono più facili da ricordare. Consigliamo di usare "go" come dominio. <br>Aggiungi il codice di tracciamento di Analytics (ad esempio, Google Analytics o Adobe Analytics) ai modelli della pagina di destinazione. </td>
    <td><a href="https://docs.marketo.com/display/public/DOCS/Edit+Landing+Page+Settings">Modifica impostazioni pagina di destinazione</a></td>
  </tr>
  <tr>
    <td rowspan="2">Munchkin </td>
    <td rowspan="2">NOTA: se sei un cliente Launch Pack, salta questo passaggio. Il tuo consulente ti fornirà le istruzioni relative al codice Munchkin nel tuo documento di istruzioni per la configurazione IT. <br><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.html" target="_blank">Aggiungi codice di tracciamento Munchkin</a> sul tuo sito web. Il codice Munchkin può essere <a href="https://developers.marketo.com/javascript-api/lead-tracking/" target="_blank">hardcoded</a> o implementato tramite Google Tag Manager.</td>
    <td><a href="https://docs.marketo.com/display/public/DOCS/Add+Munchkin+Tracking+Code+to+Your+Website">Aggiungere il codice del brano Munchkin al sito Web</a> </td>
  </tr>
  <tr>
    <td><a href="https://developers.marketo.com/javascript-api/lead-tracking/">Tracciamento lead</a> </td>
  </tr>
  <tr>
    <td>Servizi Web </td>
    <td>Abilita <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.html" target="_blank">le restrizioni IP</a> se applicabile. <br>Determinare gli utenti/le app che possono <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/users-and-roles/create-an-api-only-user.html" target="_blank">Chiamate API</a> nella tua istanza. <br>Controlla tutte le app che effettueranno chiamate API e determina se è necessario un aumento o un taglio per le chiamate API.</td>
    <td><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.html#product-docs">Creazione di un Inserisco nell'elenco Consentiti di accesso API basato su IP </a> </td>
  </tr>
  <tr>
    <td>Adobe Dynamic Chat(se applicabile) </td>
    <td>Per l’utilizzo di <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/dynamic-chat-overview.html" target="_blank">Dynamic Chat</a>, il canale di coinvolgimento conversazionale nativo in Marketi Engage, procederai con la configurazione delle autorizzazioni utente seguendo i passaggi seguenti su <a href="https://adminconsole.adobe.com/" target="_blank">Adobe Admin Console</a>. <br> <br>Conferma se l’amministratore di sistema dell’organizzazione di Adobe ti ha assegnato un ruolo di amministratore di prodotto Adobe. Contatto <a href="https://helpx.adobe.com/contact.html" target="_blank">Assistenza clienti Adobe</a><a href="https://helpx.adobe.com/contact.html)." target="_blank">https://helpx.adobe.com/contact.html</a> per scoprire chi dispone dei privilegi di amministratore nella console all’interno della tua organizzazione. <br>Accetta <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html" target="_blank">l’invito "Amministratore prodotto di Dynamic Chat"</a>. Il <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.html" target="_blank">e-mail di benvenuto</a> viene inviato quando il Dynamic Chat è abilitato nell’istanza del Marketo Engage e si è designati come amministratore di sistema.  <br>Assegna tutti gli utenti appropriati al profilo di prodotto del Marketo Engage in Adobe Admin Console. <br>Non puoi assegnare i ruoli degli utenti in Marketo Engage/Amministratore/Utenti e ruoli prima di aggiungerli a un profilo di prodotto.  <br>Se un utente indesiderato viene aggiunto a più profili di prodotto, devi eliminarlo da tutti i profili di prodotto. In caso contrario, avranno comunque accesso al Dynamic Chat. </td>
    <td> </td>
  </tr>
  <tr>
    <td>Launchpoint (se applicabile) </td>
    <td>Configura le richieste <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.html" target="_blank">LaunchPoint</a> servizi per la tua azienda.  <br>NOTA: i webinar interattivi sono una funzione integrata che offre un’integrazione nativa con Adobe Connect. Non è necessaria alcuna integrazione aggiuntiva, ma l’istanza dovrà: <a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/add-adobe-connect-as-a-launchpoint-service.html" target="_blank">sincronizza con Adobe Connect as a LaunchPoint Service.</a>  </td>
    <td><a href="https://docs.marketo.com/display/public/DOCS/Additional+Integrations">Integrazioni aggiuntive</a> </td>
  </tr>
  <tr>
    <td>Webhook (se applicabile)</td>
    <td><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/additional-integrations/create-a-webhook.html" target="_blank">Crea i webhook richiesti</a> per i tuoi affari.  </td>
    <td><a href="https://docs.marketo.com/display/public/DOCS/Create+a+Webhook">Creare un webhook</a> </td>
  </tr>
</tbody>
</table>

## Treasure Chest {#treasure-chest}

<table>
<thead>
  <tr>
    <th>Area</th>
    <th>Oggetto Azione</th>
    <th>Priorità</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Treasure Chest</td>
    <td><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/enable-or-disable-treasure-chest-features.html" target="_blank">Abilita cassa del tesoro</a> per sperimentare le funzioni di guida.  <br>Determinare le feature da attivare o disattivare.</td>
    <td>Testo</td>
  </tr>
  <tr>
    <td>Ispettore campagna </td>
    <td><a href="https://experienceleague.adobe.com/docs/marketo/using/product-docs/administration/settings/campaign-inspector.html" target="_blank">Attiva Campaign Inspector</a> per visualizzare tutte le campagne avanzate contemporaneamente.</td>
    <td>Testo</td>
  </tr>
</tbody>
</table>
