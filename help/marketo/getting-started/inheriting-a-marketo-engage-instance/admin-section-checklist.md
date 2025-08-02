---
description: Elenco di controllo dell’amministratore dell’istanza ereditata - Documentazione di Marketo - Documentazione del prodotto
title: Elenco di controllo amministrazione istanza ereditata
feature: Getting Started
exl-id: 088f3ce9-bf3d-4323-9cde-c39fec06c20e
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '1858'
ht-degree: 1%

---

# Istanza ereditata: elenco di controllo sezione amministratore {#inherited-instance-admin-section-checklist}

Le seguenti liste di controllo (le successive sono collegate in fondo a ciascun articolo) sono state create da Adobe Professional Services con il contributo dei campioni Marketo per aiutarti a imparare a usare al meglio la funzione. Puoi anche [scaricare le liste di controllo](/help/marketo/getting-started/inheriting-a-marketo-engage-instance/assets/adobe-marketo-engage-inherited-instance-admin-checklist.xlsx) e tenere traccia dei tuoi progressi.

>[!TIP]
>
>Se sei un nuovo utente di Marketo Engage e non conosci molti termini, consulta il [Glossario di Marketo Engage](/help/marketo/getting-started/things-to-know/marketo-engage-glossary.md){target="_blank"}.

## Adobe Identity Management {#adobe-identity-management}

>[!NOTE]
>
>Questo è applicabile solo alle sottoscrizioni Marketo Engage a cui è stato effettuato l&#39;onboarding in [Adobe Identity Management System (IMS)](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md){target="_blank"}. Se il tuo abbonamento non ha ancora effettuato l&#39;onboarding di Adobe IMS, procedi con l&#39;[esperienza precedente per ruoli utente e autorizzazioni](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md){target="_blank"} in Marketo Engage > Amministratore > Utenti e ruoli.

<table>
 <tbody>
  <tr>
   <th style="width:20%">Area</th>
   <th>Rivedi focus</th>
  </tr>
  <tr>
   <td>Iscrizione e amministrazione prodotto Marketo Engage</td>
   <td><li>La sottoscrizione a Marketo Engage è già stata migrata a <a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md" target="_blank">Adobe IMS</a>?
<br/>     In caso affermativo, l'amministratore di sistema di Adobe Admin Console ti ha assegnato il ruolo di "Amministratore di prodotto Adobe Admin Console"? Se non sai chi dispone dei privilegi di amministratore nella console all'interno della tua organizzazione, contatta l'<a href="https://helpx.adobe.com/it/contact.html" target="_blank">Assistenza clienti Adobe</a>.</li>
<li>Hai accettato l’invito "Amministratore di prodotto Marketo Engage"? L’e-mail viene inviata quando il ruolo viene assegnato nel Adobe Admin Console.
<br/>     In caso contrario, cerca l'<a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md#initial-setup" target="_blank">e-mail di benvenuto</a> nella tua casella in entrata e accetta l'invito ad attivare il tuo Adobe ID.</li></td>
  </tr>
  <tr>
   <td>Profilo di prodotto</td>
   <td><li>Tutti gli utenti appropriati sono assegnati al profilo di prodotto Marketo Engage in Adobe Admin Console?
<br/>     In caso contrario, assicurati di <a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md" target="_blank">aggiungere e/o rimuovere utenti</a> dai profili di prodotto di Marketo Engage in Adobe Admin Console. Non puoi assegnare i ruoli degli utenti in Marketo Engage &gt; Amministratore &gt; Utenti e ruoli se sono stati aggiunti a un profilo di prodotto.</li>
<p><img src="assets/note-icon.png" alt="icona nota"> NOTA: se un utente indesiderato viene aggiunto a più profili di prodotto, devi rimuoverlo da tutti. In caso contrario, avranno comunque accesso a Marketo Engage.</td>
  </tr>
  <tr>
   <td>API User Management</td>
   <td><li>Il tuo abbonamento utilizza qualche API di gestione utenti di Marketo?
<br/>     In tal caso, sarà necessario utilizzare <a href="https://www.adobe.io/apis/experienceplatform/umapi-new.html" target="_blank">API Adobe IMS</a> per invitare, aggiornare ed eliminare gli utenti in futuro.</li>
<p><img src="assets/note-icon.png" alt="icona nota"> NOTA: "Gestione dei ruoli" rimane in Marketo Engage e le API di gestione utenti di Marketo possono ancora essere utilizzate per la gestione dei ruoli.</td>
  </tr>
 </tbody>
</table>

## Utenti e ruoli {#users-and-roles}

<table>
 <tbody>
  <tr>
   <th style="width:20%">Area</th>
   <th>Rivedi focus</th>
  </tr>
  <tr>
   <td>Utenti</td>
   <td><img src="assets/note-icon.png" alt="icona nota"> NOTA: se il tuo abbonamento è già in Adobe IMS, procedi alla seguente revisione della gestione utenti in Adobe Admin Console. In caso contrario, passa ad Amministratore &gt; Utenti e ruoli &gt; Utenti in Marketo Engage.
   <p>
   <li><a href="/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md" target="_blank">Quanti utenti</a> ci sono?</li>
<li>Ci sono utenti che devono essere <a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md#remove-a-user" target="_blank">rimossi</a>?</li>
<li>La tua azienda applica delle policy sull’eliminazione degli utenti?</li>
<li>Quanti utenti dispongono di <a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md" target="_blank">autorizzazioni amministratore</a>?</li>
<li>Uno di questi utenti deve essere modificato in <a href="/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md" target="_blank">altri ruoli?</a></li>
<li>Chi sono gli <a href="/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md" target="_blank">utenti API</a> in questa istanza?</li></td>
  </tr>
  <tr>
   <td>Ruoli</td>
   <td><img src="assets/note-icon.png" alt="icona nota"> NOTA: indipendentemente dal fatto che si utilizzi Marketo con Adobe Identity o meno, è necessario rivedere le autorizzazioni dei ruoli in Marketo Engage in Amministratore &gt; Utenti e ruoli &gt; Ruoli.
   <p><li>Quanti ruoli ci sono?</li>
<li>Di quali <a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md" target="_blank">autorizzazioni/accesso</a> dispone ogni ruolo? Qualcosa dovrebbe essere regolato?</li>
<li>Quanti utenti ci sono per ruolo?</li>
<li>Con quale frequenza gli utenti <a href="/help/marketo/product-docs/administration/audit-trail/user-login-history.md" target="_blank">accedono</a>?</li>
<li>Ogni utente API ha il proprio <a href="/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md" target="_blank">ruolo utente</a>? In caso contrario, è consigliabile implementarlo per semplificare la risoluzione dei problemi.</li>
<li>I tuoi ruoli utente e le tue autorizzazioni sono in linea con le politiche sulla privacy dei dati aziendali per la conformità alle normative (ad esempio, <a href="https://gdpr-info.eu/" target="_blank">RGPD</a>)? I <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/privacy-management.md" target="_blank">criteri sulla privacy</a> dei dati aziendali consentono agli utenti di scaricare e condividere i dati utente di Marketo Engage? È necessaria l’attività di autorizzazione?</li></td>
  </tr>
  <tr>
   <td>Utenti di supporto</td>
   <td><li>Hai impostato i <a href="/help/marketo/getting-started/initial-setup/setup-steps.md#set-up-your-authorized-support-contacts" target="_blank">contatti autorizzati</a> appropriati nel portale di assistenza?</li></td>
  </tr>
  <tr>
   <td>Documentazione interna</td>
   <td><li>Gli utenti e i ruoli sono chiaramente definiti nella tua organizzazione?</li>
<li>Qual è il processo per aggiungere un nuovo utente/amministratore?</li></td>
  </tr>
  <tr>
   <td>Sandbox (se applicabile)</td>
   <td><li>Hai un'istanza <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/marketo-sandbox.md" target="_blank">sandbox</a>?
   <br/>     In tal caso, controlla le categorie precedenti per la sandbox.</li>
<li><a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program.md" target="_blank">Il programma di importazione</a> è collegato alla tua sandbox?</li></td>
  </tr>
 </tbody>
</table>

## Audit Trail {#audit-trail}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">Area</th>
   <th>Rivedi focus</th>
  </tr>
  <tr>
   <td>Audit Trail</td>
   <td><li><a href="/help/marketo/product-docs/administration/audit-trail/audit-trail-overview.md" target="_blank">Chi sta lavorando</a> nell'istanza?</li></td>
  </tr>
 </tbody>
</table>

## Aree di lavoro e partizioni {#workspaces-and-partitions}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">Area</th>
   <th>Rivedi focus</th>
  </tr>
  <tr>
   <td>Aree di lavoro e partizioni</td>
   <td><li>Quante <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.md" target="_blank">aree di lavoro e/o partizioni</a> hai?</li>
<li>Qual è lo scopo principale di ogni Workspace e partizione?</li>
<li>Le <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/edit-a-workspace.md" target="_blank">aree di lavoro</a> o le <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/edit-an-existing-person-partition.md" target="_blank">partizioni</a> devono essere controllate/modificate?</li>
<li>Qual è la relazione tra le aree di lavoro e le partizioni?</li>
<li>Quanti utenti <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.md" target="_blank">hanno accesso</a> a ogni Workspace?</li></td>
  </tr>
  <tr>
   <td>Documentazione interna</td>
   <td><li>Come vengono definite le aree di lavoro e le partizioni?</li>
<li>Qual è il processo per aggiungere aree di lavoro all’istanza o utenti a un Workspace?</li></td>
  </tr>
 </tbody>
</table>

## Campagne avanzate {#smart-campaigns}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">Area</th>
   <th>Rivedi focus</th>
  </tr>
  <tr>
   <td>Campagne avanzate</td>
   <td><li><a href="/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md" target="_blank">Hai una restrizione</a> sulle dimensioni di Smart Campaign?
   <br/>     In caso contrario, puoi aggiungerne uno. È consigliabile limitare i limiti di Smart Campaign al 25% del database per evitare comunicazioni eccessive o l’elaborazione dell’intero database nei flussi di lavoro; questo non solo protegge il brand, ma aiuta anche a proteggere le prestazioni dell’istanza.</li></td>
  </tr>
 </tbody>
</table>

## Limiti di comunicazione {#communication-limits}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">Area</th>
   <th>Rivedi focus</th>
  </tr>
  <tr>
   <td>Limiti di comunicazione</td>
   <td><li>Sono presenti <a href="/help/marketo/product-docs/administration/email-setup/enable-communication-limits.md" target="_blank">limiti di comunicazione</a>? La tua azienda dispone di criteri in cui potrebbero essere necessari limiti di comunicazione?</li>
<p><img src="assets/note-icon.png" alt="icona nota"> NOTA: ti consigliamo di limitare le comunicazioni a 1 al giorno e a 3 ogni 7 giorni, con <b>messaggi e-mail non</b>-<a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md" target="_blank">operativi</a> bloccati.</td>
  </tr>
 </tbody>
</table>

## Tag {#tags}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">Area</th>
   <th>Rivedi focus</th>
  </tr>
  <tr>
   <td>Tag</td>
   <td><li><a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-tags.md" target="_blank">Quanti tag</a> sono presenti? Quanti tag sono in uso? È necessario aggiungerne qualcuno?</li>
<li>I tag sono richiesti all’interno dei programmi?</li></td>
  </tr>
  <tr>
   <td>Canali</td>
   <td><li><a href="/help/marketo/product-docs/administration/tags/create-a-program-channel.md" target="_blank">Quanti canali</a> ci sono? Quanti ne vengono utilizzati?</li>
<li>Tutti gli stati del programma di <a href="/help/marketo/product-docs/administration/tags/hide-unhide-a-program-channel.md" target="_blank">canale sono appropriati</a>? Mostrano la progressione all'interno del programma?</li>
<li>I canali sono correlati a tipi di programmi specifici?</li>
<li>Quali stati sono considerati di successo per ogni canale? Sono in linea con i tuoi obiettivi di marketing?</li>
<li>Il canale operativo viene utilizzato in modo appropriato?</li>
<li>In Advanced Report Builder (Revenue Cycle Explorer/RCE), il comportamento dell’analisi dei canali è impostato in modo da essere in linea con le procedure del programma che incorporano il costo del periodo?</li></td>
  </tr>
  <tr>
   <td>Calendario marketing (se applicabile)</td>
   <td><li>Quanti <a href="/help/marketo/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/navigating-the-marketing-calendar.md" target="_blank">tipi di voci del calendario</a> sono presenti? Sono ancora tutti rilevanti?</li></td>
  </tr>
 </tbody>
</table>

## Gestione database {#database-management}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">Area</th>
   <th>Rivedi focus</th>
  </tr>
  <tr>
   <td>Gestione dei campi</td>
   <td><li>Quanti campi ci sono?
   <br/>     Fai clic su <a href="/help/marketo/product-docs/administration/field-management/export-a-list-of-all-marketo-api-field-names.md" target="_blank">Esporta nomi campi</a> per esaminare un elenco dei campi, dei campi personalizzati e dei relativi nomi API.</li>
<li>Quanti <a href="/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md" target="_blank">campi personalizzati</a> sono presenti?</li>
<li>Quanti campi vengono utilizzati?
<br/>     Seleziona <a href="/help/marketo/product-docs/administration/field-management/export-used-by-data-for-a-field.md" target="_blank">Esporta utilizzato da</a> nel menu a discesa Azioni campo per esaminare le risorse correlate di un campo.</li>
<li>Quanti campi sono sincronizzati tra Marketo Engage e il tuo sistema di gestione delle relazioni con i clienti?</li>
<li>I campi CRM sono sincronizzati con gli oggetti appropriati?</li>
<li>Esiste un <a href="/help/marketo/product-docs/administration/settings/creating-a-custom-tab-for-the-person-detail-page.md" target="_blank">set di visualizzazioni personalizzate</a> per i dettagli della persona? Ci dovrebbe essere?</li>
<li>Disponi di una convenzione di denominazione per i campi basata sull’origine?
<br/>     In caso contrario, puoi implementarlo.</li>
<li>Sono presenti campi <a href="/help/marketo/product-docs/administration/field-management/block-updates-to-a-field.md" target="_blank">bloccati</a>?
<br/>     Se è così, assicurati di capire perché lo sono.</li></td>
  </tr>
  <tr>
   <td>Attività personalizzate</td>
   <td><li>Sono presenti <a href="/help/marketo/product-docs/administration/marketo-custom-activities/understanding-custom-activities.md" target="_blank">attività personalizzate</a>?
<br/>     In tal caso, fai clic su di essi per capire quali attività non sono correlate a un modulo di Marketo, a un’e-mail o a una pagina di destinazione.</li></td>
  </tr>
  <tr>
   <td>Oggetti personalizzati</td>
   <td><li>Quanti <a href="/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md" target="_blank">oggetti personalizzati</a> sono presenti? Come vengono sincronizzati con il tuo sistema CRM?</li>
<li>In che modo questi oggetti personalizzati vengono utilizzati dai programmi e dalle query elenco?</li></td>
  </tr>
 </tbody>
</table>

## E-mail {#email}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">Area</th>
   <th>Rivedi focus</th>
  </tr>
  <tr>
   <td>Impostazioni predefinite e-mail</td>
   <td><li>In Amministratore &gt; E-mail, tutte le impostazioni predefinite sono aggiornate (ad esempio, <a href="/help/marketo/product-docs/administration/email-setup/change-the-default-from-email-and-from-label.md" target="_blank"> "da" e-mail/etichetta</a>, <a href="/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/edit-your-default-branding-domain.md" target="_blank">dominio di branding</a>, <a href="/help/marketo/product-docs/administration/email-setup/edit-the-unsubscribe-message.md" target="_blank">messaggio di annullamento dell'iscrizione</a>, ecc.)?</li></td>
  </tr>
 </tbody>
</table>

## Integrazioni {#integrations}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">Area</th>
   <th>Rivedi focus</th>
  </tr>
  <tr>
   <td>CRM</td>
   <td><li>A quale CRM stai eseguendo la sincronizzazione? Salesforce? MS Dynamics? Veeva?</li>
<li>Stai utilizzando una <a href="https://nation.marketo.com/t5/product-blogs/instructions-for-creating-a-custom-sync-rule/ba-p/242758" target="_blank">sincronizzazione personalizzata</a>?</li>
<li>[Solo per Salesforce] L’istanza dispone di filtri di sincronizzazione personalizzati implementati?
<p><img src="assets/note-icon.png" alt="icona nota"> NOTA: contatta il supporto Marketo per identificare filtri di sincronizzazione personalizzati o richiedere l’implementazione di una regola di sincronizzazione personalizzata.</li></td>
  </tr>
  <tr>
   <td>Pagine di destinazione</td>
   <td><li>Qual è il <a href="/help/marketo/product-docs/administration/settings/edit-landing-page-settings.md" target="_blank">dominio impostato come</a>?</li>
   <li>Qual è la pagina home impostata come?</li>
<li>Qual è il <a href="/help/marketo/product-docs/administration/settings/set-a-fallback-page.md" target="_blank">fallback impostato come</a>?</li>
<li>La precompilazione del modulo è abilitata?</li>
<li><a href="/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/enable-personalized-urls-for-your-account.md" target="_blank">gli URL personalizzati</a> sono abilitati?</li>
<li>Esistono regole impostate per <a href="/help/marketo/product-docs/demand-generation/landing-pages/landing-page-actions/redirect-a-marketo-landing-page-to-another-page.md" target="_blank">reindirizzamenti</a>?</li>
<li>Sono presenti alias di dominio? Stai monitorando come utilizzi gli alias di dominio?</li>
<li><a href="https://nation.marketo.com/t5/knowledgebase/setting-up-secured-domains-for-marketo-landing-pages-first-time/ta-p/250370" target="_blank">I domini protetti per le pagine di destinazione</a> sono abilitati?
<br/>     Conferma se le risorse della pagina di destinazione contengono un URL "http".</li></td>
  </tr>
  <tr>
   <td>Munchkin</td>
   <td><li>Il tuo <a href="/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md" target="_blank">codice di tracciamento di Munchkin</a> è sul tuo sito Web (non è una pagina di destinazione di Marketo Engage)?</li>
<li>Una richiesta browser <a href="/help/marketo/product-docs/administration/settings/edit-do-not-track-browser-support-settings.md" target="_blank">Do Not Track</a> è abilitata?</li>
<li>La tua <a href="https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/javascriptapi/leadtracking/lead-tracking" target="_blank">API Munchkin</a> è configurata?
<p><img src="assets/tip-icon.png" alt="icona di suggerimento">SUGGERIMENTO: se manca la documentazione sulla posizione del codice munchkin sul sito Web, puoi visualizzare tutti gli URL creando un <a href="/help/marketo/product-docs/reporting/basic-reporting/report-types/web-page-activity-report.md" target="_blank">report attività pagina Web</a>.</li></td>
  </tr>
  <tr>
   <td>Servizi Web</td>
   <td><li>Le <a href="/help/marketo/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.md" target="_blank">restrizioni IP</a> sono abilitate? Dovrebbero esserlo?</li>
<li>Quali utenti/app eseguono chiamate API nell’istanza?</li>
<li>Stai raggiungendo o stai per raggiungere il limite API?
<br/>     In tal caso, puoi aumentarlo o controllare l’istanza per ridurre tali chiamate API.</li></td>
  </tr>
  <tr>
   <td>Adobe Dynamic Chat (se applicabile)</td>
<td>Seguendo i passaggi seguenti sarà necessario accedere a <a href="https://adminconsole.adobe.com/" target="_blank">Adobe Admin Console</a>. Se non hai ancora configurato un Adobe ID, <a href="https://helpx.adobe.com/it/manage-account/using/create-update-adobe-id.html" target="_blank">scopri come farlo qui</a>.
<br/>
<li>Hai accettato l'<a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/initial-setup.md" target="_blank">invito dell'amministratore di prodotto Dynamic Chat</a>? L’e-mail viene inviata quando Dynamic Chat è abilitato nella tua istanza di Marketo Engage e sei designato come Amministratore di sistema.
<br/>     In caso contrario, cerca l’e-mail di benvenuto nella tua casella in entrata e accetta l’invito a configurare il tuo Adobe ID.</li>
<li>Hai aggiunto gli <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/add-or-remove-chat-users.md#add-a-chat-user" target="_blank">utenti desiderati</a> al profilo di prodotto Dynamic Chat in Adobe Admin Console?
<li>Assicurati che gli utenti idonei abbiano aggiunto il profilo di prodotto Dynamic Chat alla propria identità Adobe. Non puoi assegnare i ruoli "Access Dynamic Chat" (Accedi a) in Marketo Engage &gt; Amministratore &gt; Utenti e ruoli se sono stati aggiunti a un profilo di prodotto.</li>
<li>Nella scheda "Profili di prodotto", le Autorizzazioni profilo predefinite sono allineate alle esigenze della tua organizzazione?<br/>
In caso contrario, modifica le autorizzazioni per il profilo specifico. </li>
<li>Se disponi di più di un abbonamento, gli utenti vengono aggiunti agli abbonamenti corretti?</li>
<br>
Dopo aver completato il controllo delle impostazioni Utenti e ruoli, accedi a Dynamic Chat per continuare il controllo.
<li>Hai <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/integrations/adobe-marketo-engage.md" target="_blank">connesso la tua istanza di Marketo Engage</a> a Dynamic Chat?</li>
<li>I cinque profili predefiniti con autorizzazioni predefinite sono applicabili alla tua organizzazione?<br/>
     In caso contrario, è possibile <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions.md#edit-existing-permissions" target="_blank">modificarli in Dynamic Chat</a>. Puoi anche <a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/permissions.md#create-a-profile" target="_blank">creare un profilo personalizzato</a> con un set di autorizzazioni personalizzato.</li>
<li>Per consentire agli utenti di accedere a Dynamic Chat, hai selezionato "Accedi a Dynamic Chat" per il ruolo Marketo Engage applicabile in Amministratore &gt; Utenti e ruoli &gt; Ruoli?
<br/><img src="assets/note-icon.png" alt="icona nota"> NOTA: i ruoli 'Admin' e 'Marketing User' devono avere accesso a Dynamic Chat.</li>
</td>
  </tr>
  <td>Marketo Sales Insight (se applicabile)</td>
   <td><li>Il pacchetto <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md" target="_blank">MSI è stato installato</a>?</li>
<li>Hai <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md" target="_blank">aggiornato all'ultima versione di Sales Insight</a>?</li>
<li>Hai completato la configurazione di Sales Insight? <br/>     Utenti Enterprise/Unlimited <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md" target="_blank">fai clic qui</a>, utenti Professional <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md" target="_blank">fai clic qui</a>.</li>
<li>Hai <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-permission-set.md" target="_blank">dato accesso ai tuoi utenti</a> in base al numero di postazioni che hai acquistato?</li>
<li><a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/customize-stars-and-flames.md" target="_blank">Stelle e fiamme</a> sono personalizzate?</li></td>
  </tr>
  <tr>
   <td>Launchpoint (se applicabile)</td>
   <td><li>Quali servizi hai configurato (ad esempio <a href="/help/marketo/product-docs/administration/additional-integrations/add-webex-as-a-launchpoint-service.md" target="_blank">BrightTALK</a>, <a href="/help/marketo/product-docs/administration/additional-integrations/connect-brighttalk-to-marketo.md" target="_blank">Zoom</a>, ecc.)? Qualcuno è vicino alla loro scadenza?</li>
<li><a href="https://nation.marketo.com/t5/knowledgebase/viewing-your-number-of-api-calls-to-marketo/ta-p/254256" target="_blank">Quante chiamate API</a> vengono utilizzate dalle integrazioni?</li>
<li>Hai le integrazioni corrette per i tuoi casi d’uso?</li></td>
  </tr>
  <tr>
   <td>Webhook (se applicabile)</td>
   <td><li><a href="/help/marketo/product-docs/administration/additional-integrations/create-a-webhook.md" target="_blank">Quali connessioni</a> hai configurato?</li>
<li>Non sono più in uso?</li></td>
  </tr>
  <tr>
   <td>App mobili (se applicabile)</td>
   <td><li>Quali <a href="/help/marketo/product-docs/mobile-marketing/admin/add-a-mobile-app.md" target="_blank">app per dispositivi mobili</a> hai?</li>
<li>Sono stati aggiunti <a href="/help/marketo/product-docs/mobile-marketing/push-notifications/adding-a-new-test-device.md" target="_blank">dispositivi di test</a>?</li></td>
  </tr>
 </tbody>
</table>

## Treasure Chest {#treasure-chest}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">Area</th>
   <th>Rivedi focus</th>
  </tr>
  <tr>
   <td>Treasure Chest</td>
   <td><li>Che cosa è attivato nel <a href="/help/marketo/product-docs/administration/settings/enable-or-disable-treasure-chest-features.md" target="_blank">scrigno del tesoro</a>?</li>
<li>È necessario attivare o disattivare alcune funzionalità?</li></td>
  </tr>
  <tr>
   <td>Ispettore campagna</td>
   <td><li><a href="/help/marketo/product-docs/administration/settings/campaign-inspector.md" target="_blank">Ispettore campagna</a> è attivato?
<br/>In caso contrario, potrebbe essere utile attivarlo per identificare facilmente le campagne attive, sincronizzarle con il tuo sistema di gestione delle relazioni con i clienti e/o eliminare record.</li></td>
  </tr>
 </tbody>
</table>

## Avvisi e aggiornamenti {#alerts-and-updates}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">Area</th>
   <th>Rivedi focus</th>
  </tr>
  <tr>
   <td>Aggiornamenti dello stato del Marketo Engage</td>
   <td><li>La tua istanza è abbonata a <a href="https://nation.marketo.com/t5/knowledgebase/how-to-subscribe-to-status-page-notifications/ta-p/296749" target="_blank">Aggiornamenti dello stato del Marketo Engage</a>?</li></td>
  </tr>
  <tr>
   <td>Avvisi</td>
   <td><li>Sono presenti <a href="/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md" target="_blank">avvisi attivi</a> inviati a team interni da Marketo Engage?</li>
<li>In caso affermativo, tali avvisi funzionano in modo appropriato?</li></td>
  </tr>
  <tr>
   <td>Notifiche</td>
   <td><li>Sei abbonato alle <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications.md" target="_blank">notifiche</a> di amministrazione appropriate?</li></td>
  </tr>
 </tbody>
</table>
