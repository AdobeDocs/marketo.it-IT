---
description: Elenco di controllo dell’amministratore dell’istanza ereditata - Documentazione di Marketo - Documentazione del prodotto
title: Elenco di controllo amministrazione istanza ereditata
feature: Getting Started
source-git-commit: 2120b700fde80f470b5e221c0212c8d29e3920ae
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Istanza ereditata: elenco di controllo sezione amministratore {#inherited-instance-admin-section-checklist}

Le seguenti liste di controllo (le successive sono collegate in fondo a ciascun articolo) sono state create da Adobe Professional Services con il contributo dei campioni Marketo per aiutarti a imparare a usare al meglio la funzione. È inoltre possibile [scaricare gli elenchi di controllo](/help/marketo/getting-started/inheriting-a-marketo-engage-instance/assets/adobe-marketo-engage-inherited-instance-admin-checklist.xlsx) e tieni traccia dei tuoi progressi.

>[!TIP]
>
>Se sei un nuovo utente del Marketo Engage e non conosci molti dei termini, controlla [Glossario Marketo Engage](/help/marketo/getting-started/marketo-engage-glossary.md){target="_blank"}.

## Adobe Identity Management {#adobe-identity-management}

>[!NOTE]
>
>Questo è applicabile solo agli abbonamenti a cui è stato effettuato l’onboarding [Sistema Adobe Identity Management (IMS)](/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md){target="_blank"}. If your Marketo Engage subscription has not onboarded Adobe IMS yet, proceed with the [legacy user roles and permissions experience](/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md){target="_blank"} in Marketo Engage > Amministratore > Utenti e ruoli.

<table> 
 <tbody> 
  <tr> 
   <th style="width:20%">Area</th> 
   <th>Rivedi focus</th>
  </tr> 
  <tr> 
   <td>Amministratore prodotti abbonamento e Marketo Engage</td> 
   <td><li>È stata effettuata la migrazione della sottoscrizione di Marketo Engage a <a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md" target="_blank">Adobe IMS</a> già? 
<br/>     In caso affermativo, l'amministratore di sistema di Adobe Admin Console ti ha assegnato il ruolo di "Amministratore di prodotto Adobe Admin Console"? Se non sai chi dispone dei privilegi di amministratore nella console all’interno della tua organizzazione, contatta <a href="https://helpx.adobe.com/contact.html" target="_blank">Assistenza clienti Adobe</a>.</li>
<li>Hai accettato l’invito "Amministratore prodotto di Marketo Engage"? L’e-mail viene inviata quando il ruolo viene assegnato nel Adobe Admin Console.
<br/>     In caso contrario, cercare <a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/admin-setup.md#initial-setup" target="_blank">e-mail di benvenuto</a> nella tua casella in entrata e accetta l’invito ad attivare il tuo Adobe ID.</li></td>
  </tr>
  <tr> 
   <td>Profilo prodotto</td> 
   <td><li>Tutti gli utenti appropriati sono assegnati al profilo di prodotto del Marketo Engage in Adobe Admin Console?
<br/>     In caso contrario, assicurarsi di <a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md" target="_blank">aggiungere e/o rimuovere utenti</a> dai profili di prodotto di Marketo Engage in Adobe Admin Console. Non puoi assegnare i ruoli degli utenti in Marketo Engage &gt; Amministratore &gt; Utenti e ruoli se sono stati aggiunti a un profilo di prodotto.</li>
<p><img src="assets/note-icon.png" alt="icona nota"> NOTA: se un utente indesiderato viene aggiunto a più profili di prodotto, devi rimuoverlo da tutti i profili di prodotto. Altrimenti avranno ancora accesso al Marketo Engage.</td>
  </tr>
  <tr> 
   <td>API User Management</td> 
   <td><li>Il tuo abbonamento utilizza qualche API di gestione utenti di Marketo?
<br/>     In tal caso, dovrai utilizzare <a href="https://www.adobe.io/apis/experienceplatform/umapi-new.html" target="_blank">API di Adobe IMS</a> per invitare, aggiornare ed eliminare gli utenti da un momento all'altro.</li>
<p><img src="assets/note-icon.png" alt="icona nota"> NOTA: "Gestione dei ruoli" rimane nel Marketo Engage e le API di gestione utenti Marketo possono ancora essere utilizzate per la gestione dei ruoli.</td>
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
   <td><img src="assets/note-icon.png" alt="icona nota"> NOTA: se il tuo abbonamento è già in Adobe IMS, procedi alla seguente revisione della gestione utenti in Adobe Admin Console. In caso contrario, passa ad Amministratore &gt; Utenti e ruoli &gt; Utenti nel Marketo Engage.
   <p>
   <li><a href="/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md" target="_blank">Quanti utenti</a> ci sono?</li>
<li>Ci sono utenti che dovrebbero essere <a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user.md#remove-a-user" target="_blank">rimosso</a>?</li>
<li>La tua azienda applica delle policy sull’eliminazione degli utenti?</li> 
<li>Quanti utenti hanno <a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md" target="_blank">Autorizzazioni amministratore</a>?</li>
<li>Se uno di questi utenti deve essere modificato in <a href="/help/marketo/product-docs/administration/users-and-roles/managing-user-roles-and-permissions.md" target="_blank">altri ruoli?</a></li> 
<li>Chi sono i <a href="/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user.md" target="_blank">Utenti API</a> in questo caso?</li></td>
  </tr>
  <tr> 
   <td>Ruoli</td> 
   <td><img src="assets/note-icon.png" alt="icona nota"> NOTA: indipendentemente dal fatto che si utilizzi Marketo con Adobe Identity o meno, procedere con la revisione delle autorizzazioni dei ruoli nel Marketo Engage in Amministratore &gt; Utenti e ruoli &gt; Ruoli.
   <p><li>Quanti ruoli ci sono?</li>  
<li>Cosa <a href="/help/marketo/product-docs/administration/users-and-roles/descriptions-of-role-permissions.md" target="_blank">autorizzazioni/accesso</a> ciascun ruolo dispone di? Qualcosa dovrebbe essere regolato?</li>
<li>Quanti utenti ci sono per ruolo?</li>
<li>Con quale frequenza gli utenti <a href="/help/marketo/product-docs/administration/audit-trail/user-login-history.md" target="_blank">accesso</a>?</li>
<li>Ogni utente API ha il proprio <a href="/help/marketo/product-docs/administration/users-and-roles/create-an-api-only-user-role.md" target="_blank">ruolo utente proprio</a>? In caso contrario, è consigliabile implementarlo per semplificare la risoluzione dei problemi.</li> 
<li>I ruoli utente e le autorizzazioni sono in linea con le politiche sulla privacy dei dati aziendali per garantire la conformità alle normative (ad esempio, <a href="https://gdpr-info.eu/" target="_blank">RGPD</a>)? I dati aziendali <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/privacy-management.md" target="_blank">informativa sulla privacy</a> consentire agli utenti di scaricare e condividere i dati utente del Marketo Engage? È necessaria l’attività di autorizzazione?</li></td>
  </tr>
  <tr> 
   <td>Utenti di supporto</td> 
   <td><li>Hai impostato il <a href="/help/marketo/getting-started/setup/setup-steps.md#set-up-your-authorized-support-contacts" target="_blank">contatti autorizzati</a> nel portale di assistenza?</li></td>
  </tr>
  <tr> 
   <td>Documentazione interna</td> 
   <td><li>Gli utenti e i ruoli sono chiaramente definiti nella tua organizzazione?</li>
<li>Qual è il processo per aggiungere un nuovo utente/amministratore?</li></td>
  </tr>
  <tr> 
   <td>Sandbox (se applicabile)</td> 
   <td><li>Hai un <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/marketo-sandbox.md" target="_blank">istanza sandbox</a>?
   <br/>     In tal caso, controlla le categorie precedenti per la sandbox.</li>
<li>È <a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/import-a-program.md" target="_blank">Importazione programma</a> collegato alla sandbox?</li></td>
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
   <td><li>Quanti <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.md" target="_blank">Aree di lavoro e/o partizioni</a> l'hai fatto?</li>
<li>Qual è lo scopo principale di ogni area di lavoro e partizione?</li>
<li>Effettua una delle seguenti operazioni <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/edit-a-workspace.md" target="_blank">Aree di lavoro</a> o <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/edit-an-existing-person-partition.md" target="_blank">Partizioni</a> deve essere controllato/modificato?</li>
<li>Qual è la relazione tra le aree di lavoro e le partizioni?</li>
<li>Quanti utenti <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/allow-user-access-to-a-workspace.md" target="_blank">avere accesso</a> in ogni area di lavoro?</li></td>
  </tr>
  <tr> 
   <td>Documentazione interna</td> 
   <td><li>Come vengono definite le aree di lavoro e le partizioni?</li>
<li>Qual è il processo per aggiungere aree di lavoro all’istanza o utenti a un’area di lavoro?</li></td>
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
   <td><li><a href="/help/marketo/product-docs/administration/email-setup/enable-person-restrictions-for-smart-campaigns.md" target="_blank">Hai una restrizione?</a> sulle dimensioni di Smart Campaign? 
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
   <td><li>Ci sono <a href="/help/marketo/product-docs/administration/email-setup/enable-communication-limits.md" target="_blank">limiti di comunicazione</a> sul posto? La tua azienda dispone di criteri in cui potrebbero essere necessari limiti di comunicazione?</li>
<p><img src="assets/note-icon.png" alt="icona nota"> NOTA: si consiglia di limitare la comunicazione a 1 al giorno e 3 ogni 7 giorni, con <b>non</b>-<a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/make-an-email-operational.md" target="_blank">operative</a> e-mail bloccate.</td>
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
   <td><li><a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/understanding-tags.md" target="_blank">Quanti tag</a> ci sono? Quanti tag sono in uso? È necessario aggiungerne qualcuno?</li>
<li>I tag sono richiesti all’interno dei programmi?</li></td>
  </tr>
  <tr> 
   <td>Canali</td> 
   <td><li><a href="/help/marketo/product-docs/administration/tags/create-a-program-channel.md" target="_blank">Quanti canali</a> ci sono? Quanti ne vengono utilizzati?</li>
<li>Sono tutti <a href="/help/marketo/product-docs/administration/tags/hide-unhide-a-program-channel.md" target="_blank">stati dei programmi canale appropriati</a>? Mostrano la progressione all'interno del programma?</li>
<li>I canali sono correlati a tipi di programmi specifici?</li>
<li>Quali stati sono considerati di successo per ogni canale? Sono in linea con i tuoi obiettivi di marketing?</li>
<li>Il canale operativo viene utilizzato in modo appropriato?</li>
<li>Per il Report Builder avanzato (Revenue Cycle Explorer/RCE), il comportamento di analisi dei canali è impostato per l’allineamento con le procedure del programma che includono il costo del periodo?</li></td>
  </tr>
  <tr> 
   <td>Calendario marketing (se applicabile)</td> 
   <td><li>Quanti <a href="/help/marketo/product-docs/core-marketo-concepts/marketing-calendar/understanding-the-calendar/navigating-the-marketing-calendar.md" target="_blank">tipi di voci del calendario</a> ci sono? Sono ancora tutti rilevanti?</li></td>
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
   <br/>     Clic <a href="/help/marketo/product-docs/administration/field-management/export-a-list-of-all-marketo-api-field-names.md" target="_blank">Esporta nomi campi</a> per rivedere un elenco dei campi, dei campi personalizzati e dei relativi nomi API.</li>
<li>Quanti <a href="/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md" target="_blank">campi personalizzati</a> ci sono?</li>
<li>Quanti campi vengono utilizzati? 
<br/>     Seleziona <a href="/help/marketo/product-docs/administration/field-management/export-used-by-data-for-a-field.md" target="_blank">Esporta utilizzato da</a> nel menu a discesa Azioni campo per esaminare le risorse correlate di un campo.</li>
<li>Quanti campi sono sincronizzati tra il Marketo Engage e il CRM?</li>
<li>I campi CRM sono sincronizzati con gli oggetti appropriati?</li>
<li>Esiste un <a href="/help/marketo/product-docs/administration/settings/creating-a-custom-tab-for-the-person-detail-page.md" target="_blank">set di visualizzazioni personalizzate</a> per i dettagli della persona? Ci dovrebbe essere?</li>
<li>Disponi di una convenzione di denominazione per i campi basata sull’origine? 
<br/>     In caso contrario, puoi implementarlo.</li>
<li>Sono presenti campi <a href="/help/marketo/product-docs/administration/field-management/block-updates-to-a-field.md" target="_blank">bloccato</a>? 
<br/>     Se è così, assicurati di capire perché lo sono.</li></td>
  </tr>
  <tr> 
   <td>Attività personalizzate</td> 
   <td><li>Ci sono <a href="/help/marketo/product-docs/administration/marketo-custom-activities/understanding-custom-activities.md" target="_blank">attività personalizzate</a>?
<br/>     In tal caso, fai clic su di essi per capire quali attività non sono correlate a un modulo di Marketo, a un’e-mail o a una pagina di destinazione.</li></td>
  </tr>
  <tr> 
   <td>Oggetti personalizzati</td> 
   <td><li>Quanti <a href="/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md" target="_blank">oggetti personalizzati</a> ci sono? Come vengono sincronizzati con il tuo sistema CRM?</li>
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
   <td><li>In Amministratore &gt; E-mail, tutte le impostazioni predefinite sono aggiornate (ad esempio, <a href="/help/marketo/product-docs/administration/email-setup/change-the-default-from-email-and-from-label.md" target="_blank">E-mail/etichetta "da"</a>, <a href="/help/marketo/product-docs/administration/email-setup/add-multiple-branding-domains/edit-your-default-branding-domain.md" target="_blank">dominio di branding</a>, <a href="/help/marketo/product-docs/administration/email-setup/edit-the-unsubscribe-message.md" target="_blank">messaggio di annullamento iscrizione</a>, ecc.)?</li></td>
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
<li>Stai utilizzando un’ <a href="https://nation.marketo.com/t5/product-blogs/instructions-for-creating-a-custom-sync-rule/ba-p/242758" target="_blank">sincronizzazione personalizzata</a>?</li>
<li>[Solo per Salesforce] L’istanza dispone di filtri di sincronizzazione personalizzati implementati? 
<p><img src="assets/note-icon.png" alt="icona nota"> NOTA: contatta il supporto Marketo per identificare filtri di sincronizzazione personalizzati o richiedere l’implementazione di una regola di sincronizzazione personalizzata.</li></td>
  </tr>
  <tr> 
   <td>Pagine di destinazione</td> 
   <td><li>Cos'è <a href="/help/marketo/product-docs/administration/settings/edit-landing-page-settings.md" target="_blank">dominio impostato come</a>?</li>
   <li>Qual è la pagina home impostata come?</li>
<li>Cos'è <a href="/help/marketo/product-docs/administration/settings/set-a-fallback-page.md" target="_blank">fallback impostato come</a>?</li>
<li>La precompilazione del modulo è abilitata?</li>
<li>Sono <a href="/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/enable-personalized-urls-for-your-account.md" target="_blank">URL personalizzati</a> abilitato?</li>
<li>Esistono regole impostate per <a href="/help/marketo/product-docs/demand-generation/landing-pages/landing-page-actions/redirect-a-marketo-landing-page-to-another-page.md" target="_blank">reindirizzamenti</a>?</li>
<li>Sono presenti alias di dominio? Stai monitorando come utilizzi gli alias di dominio?</li>
<li>È <a href="https://nation.marketo.com/t5/knowledgebase/setting-up-secured-domains-for-marketo-landing-pages-first-time/ta-p/250370" target="_blank">Domini protetti per le pagine di destinazione</a> abilitato? 
<br/>     Conferma se le risorse della pagina di destinazione contengono un URL "http".</li></td>
  </tr>
  <tr> 
   <td>Munchkin</td> 
   <td><li>È il <a href="/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md" target="_blank">Codice di tracciamento Munchkin</a> sul tuo sito web (non è una pagina di destinazione del Marketo Engage)?</li>
<li>È un <a href="/help/marketo/product-docs/administration/settings/edit-do-not-track-browser-support-settings.md" target="_blank">Do Not Track</a> Richiesta browser abilitata?</li>
<li>È il <a href="https://developers.marketo.com/javascript-api/lead-tracking/" target="_blank">API Munchkin</a> configurato? 
<p><img src="assets/tip-icon.png" alt="icona di suggerimento">SUGGERIMENTO: se manca la documentazione su dove si trova il codice munchkin sul sito web, puoi visualizzare tutti gli URL creando un <a href="/help/marketo/product-docs/reporting/basic-reporting/report-types/web-page-activity-report.md" target="_blank">Rapporto attività pagina web</a>.</li></td>
  </tr>
  <tr> 
   <td>Servizi Web</td> 
   <td><li>Sono <a href="/help/marketo/product-docs/administration/additional-integrations/create-an-allowlist-for-ip-based-api-access.md" target="_blank">Restrizioni IP</a> abilitato? Dovrebbero esserlo?</li>
<li>Quali utenti/app eseguono chiamate API nell’istanza?</li>
<li>Stai raggiungendo o stai per raggiungere il limite API? 
<br/>     In tal caso, puoi aumentarlo o controllare l’istanza per ridurre tali chiamate API.</li></td>
  </tr>
  <tr> 
   <td>Marketo Sales Insight (se applicabile)</td> 
   <td><li>Ha <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md" target="_blank">Pacchetto MSI installato</a>?</li>
<li>Hai <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md" target="_blank">aggiornato all’ultima versione di Sales Insight</a>?</li>
<li>Hai completato la configurazione di Sales Insight? <br/>     Utenti Enterprise/Unlimited <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md" target="_blank">fai clic qui</a>, utenti professionali <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md" target="_blank">fai clic qui</a>.</li>
<li>Hai <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/add-sales-insight-permission-set.md" target="_blank">accesso dato ai tuoi utenti</a> in base al numero di posti che hai acquistato?</li>
<li>Sono <a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/stars-and-flames/customize-stars-and-flames.md" target="_blank">Stelle e fiamme</a> personalizzato?</li></td>
  </tr>
  <tr> 
   <td>Launchpoint (se applicabile)</td> 
   <td><li>Quali servizi hai configurato (ad es. <a href="/help/marketo/product-docs/administration/additional-integrations/add-webex-as-a-launchpoint-service.md" target="_blank">BrightTALK</a>, <a href="/help/marketo/product-docs/administration/additional-integrations/connect-brighttalk-to-marketo.md" target="_blank">Zoom</a>, ecc.)? Qualcuno è vicino alla loro scadenza?</li>
<li><a href="https://nation.marketo.com/t5/knowledgebase/viewing-your-number-of-api-calls-to-marketo/ta-p/254256" target="_blank">Quante chiamate API</a> le integrazioni utilizzano?</li>
<li>Hai le integrazioni corrette per i tuoi casi d’uso?</li></td>
  </tr>
  <tr> 
   <td>Webhook (se applicabile)</td> 
   <td><li><a href="/help/marketo/product-docs/administration/additional-integrations/create-a-webhook.md" target="_blank">Quali connessioni</a> hai preparato?</li>
<li>Non sono più in uso?</li></td>
  </tr>
  <tr> 
   <td>App mobili (se applicabile)</td> 
   <td><li>Quale <a href="/help/marketo/product-docs/mobile-marketing/admin/add-a-mobile-app.md" target="_blank">app mobili</a> l'hai fatto?</li>
<li>Avere <a href="/help/marketo/product-docs/mobile-marketing/push-notifications/adding-a-new-test-device.md" target="_blank">dispositivi di prova</a>  è stato aggiunto?</li></td>
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
   <td><li>Funzionamento di <a href="/help/marketo/product-docs/administration/settings/enable-or-disable-treasure-chest-features.md" target="_blank">Treasure Chest</a>?</li>
<li>È necessario attivare o disattivare alcune funzionalità?</li></td>
  </tr>
  <tr> 
   <td>Ispettore campagna</td> 
   <td><li>È <a href="/help/marketo/product-docs/administration/settings/campaign-inspector.md" target="_blank">Ispettore campagna</a> acceso?
<br/>In caso contrario, puoi attivarlo per identificare facilmente quali campagne sono: attive, in sincronizzazione con il tuo sistema di gestione delle relazioni con i clienti e/o eliminando record.</li></td>
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
   <td>Aggiornamenti stato Marketo Engage</td> 
   <td><li>La tua istanza è abbonata a <a href="https://nation.marketo.com/t5/knowledgebase/how-to-subscribe-to-status-page-notifications/ta-p/296749" target="_blank">Aggiornamenti stato Marketo Engage</a>?</li></td>
  </tr>
  <tr> 
   <td>Avvisi</td> 
   <td><li>Ci sono <a href="/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/send-alert.md" target="_blank">avvisi attivi</a> essere inviati dal Marketo Engage ai team interni?</li>
<li>In caso affermativo, tali avvisi funzionano in modo appropriato?</li></td>
  </tr>
  <tr> 
   <td>Notifiche</td> 
   <td><li>Sei abbonato all’amministratore appropriato? <a href="/help/marketo/product-docs/core-marketo-concepts/miscellaneous/understanding-notifications.md" target="_blank">notifiche</a>?</li></td>
  </tr>
 </tbody> 
</table>

<br> 

[Controllo di un&#39;istanza ereditata: ► database](/help/marketo/getting-started/inheriting-a-marketo-engage-instance/database-checklist.md)
