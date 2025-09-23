---
description: Elenco di controllo di Instance Design Studio ereditato - Documenti Marketo - Documentazione del prodotto
title: Elenco di controllo di Design Studio dell'istanza ereditata
feature: Getting Started
exl-id: 41e89120-4ac0-4e70-bed0-da4e5c5542ff
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '561'
ht-degree: 3%

---

# Istanza ereditata: elenco di controllo di Design Studio {#inherited-instance-design-studio-checklist}

La struttura dei modelli e la creazione di moduli globali, snippet, immagini e file aiuteranno a ridurre al minimo gli errori di dati e a semplificare il flusso di lavoro della generazione del programma. Ricordati di [scaricare le liste di controllo](/help/marketo/getting-started/inheriting-a-marketo-engage-instance/assets/adobe-marketo-engage-inherited-instance-admin-checklist.xlsx) e tenere traccia dell&#39;avanzamento.

## Pagine di destinazione {#landing-pages}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">Area</th>
   <th>Rivedi focus</th>
  </tr>
  <tr>
   <td>Pagine di destinazione globali</td>
   <td><li>Quante <a href="/help/marketo/product-docs/demand-generation/landing-pages/understanding-landing-pages/understanding-free-form-vs-guided-landing-pages.md" target="_blank">pagine di destinazione</a> globali sono presenti? Vengono utilizzati dai programmi?</li>
   <li>È stato configurato un <a href="https://experienceleague.adobe.com/docs/marketo-learn/tutorials/lead-and-data-management/subscription-center-learn.html?lang=it" target="_blank">centro sottoscrizioni</a>?
   <br/>     In caso contrario, puoi crearne una.</li></td>
  </tr>
  <tr>
   <td>Modelli</td>
   <td><li>Quanti <a href="/help/marketo/product-docs/demand-generation/landing-pages/landing-page-templates/edit-a-marketo-landing-page-template.md" target="_blank">modelli di pagina di destinazione</a> sono presenti? Vengono sfruttati?</li></td>
  </tr>
  <tr>
   <td>Gruppi di test</td>
   <td><li>Quanti <a href="/help/marketo/product-docs/demand-generation/landing-pages/understanding-landing-pages/landing-page-test-groups.md" target="_blank">gruppi di test della pagina di destinazione</a> sono? Sono ancora tutti rilevanti?</li></td>
  </tr>
   <tr>
   <td>Privacy e conformità</td>
   <td><li>Tutte le pagine di destinazione dispongono dei piè di pagina appropriati?</li></td>
  </tr>
 </tbody>
</table>

## Immagini e file {#images-and-files}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">Area</th>
   <th>Rivedi focus</th>
  </tr>
  <tr>
   <td>Convenzioni di denominazione</td>
   <td><li><a href="/help/marketo/product-docs/demand-generation/images-and-files/add-images-and-files-to-marketo.md" target="_blank">immagini e file</a> hanno convenzioni di denominazione coerenti?</li></td>
  </tr>
  <tr>
   <td>Struttura delle cartelle</td>
   <td><li>Le immagini e i file <a href="/help/marketo/product-docs/demand-generation/images-and-files/organize-your-images-and-files-using-folders.md" target="_blank">sono organizzati in modo appropriato</a> e sono facili da cercare?</li></td>
  </tr>
  <tr>
   <td>Immagini e file</td>
   <td><li>È necessario aggiornare le immagini o i file <a href="/help/marketo/product-docs/demand-generation/images-and-files/find-the-url-of-an-uploaded-image-or-file.md" target="_blank">a cui si fa riferimento nelle pagine Web</a>?
   <p>Esempio: potrebbe essere necessario aggiornare la struttura URL hardcoded <a href="https://nation.marketo.com/t5/product-documents/upcoming-changes-to-design-studio-urls/ta-p/306632#_Toc54870361" target="_blank"></a>, ad esempio <code>http://na-sj01.marketo.com/rs/123-ABC-456/images/puppy.png</code>.
   <p>Collabora con il tuo sviluppatore web per determinare dove è necessario apportare aggiornamenti.</li></td>
  </tr>
 </tbody>
</table>

## Forms {#forms}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">Area</th>
   <th>Rivedi focus</th>
  </tr>
  <tr>
   <td>Forms globale</td>
   <td><li>Quanti <a href="/help/marketo/product-docs/demand-generation/forms/creating-a-form/create-a-form.md" target="_blank">moduli</a> globali sono presenti?</li>
<li>La maggior parte dei programmi utilizza moduli globali o locali?</li>
<li>Tutti i moduli raccolgono i dati giusti per il marketing e le vendite?</li>
<li>I valori nascosti vengono utilizzati in modo appropriato?</li>
<li>Esistono moduli Marketo Engage utilizzati su pagine di destinazione non Marketo Engage? Come vengono referenziati?</li>
<p><img src="assets/tip-icon.png" alt="icona di suggerimento">SUGGERIMENTO: aggiorna le pagine in cui incorpori Marketo Engage Form con il nuovo codice da incorporare introdotto (richiede pagine di destinazione protette).
<p><a href="/help/marketo/getting-started/inheriting-a-marketo-engage-instance/assets/design-studio-checklist-2.png" target="_blank"><img src="assets/design-studio-checklist-1.png" alt="miniatura codice"></a>
</td>
  </tr>
  <tr>
   <td>Standardizzazione dati</td>
   <td><li>I <a href="/help/marketo/product-docs/demand-generation/forms/form-fields/add-a-fieldset-to-a-form.md" target="_blank">campi modulo</a> sono principalmente elenchi a discesa o campi di testo aperti?</li>
<p><img src="assets/tip-icon.png" alt="icona di suggerimento">SUGGERIMENTO: se si tratta di campi di testo aperti, è consigliabile passare agli elenchi a discesa per evitare problemi di dati.</td>
  </tr>
  <tr>
   <td>Privacy e conformità</td>
   <td><li>La strategia dei moduli è in linea con i requisiti aziendali relativi alla privacy dei dati e all’opt-in?
   <br/>     Prendi in considerazione <a href="https://business.adobe.com/resources/ebooks/the-gdpr-and-the-marketer.html" target="_blank">il Regolamento generale sulla protezione dei dati (RGPD)</a>, la legge canadese anti-spam (CASL), il Controlling the Assault of Non-Solicited Pornography and Marketing Act of 2003 (CAN-SPAM), il California Consumer Privacy Act (CCPA), ecc., per la conformità alle normative.</li>
<p><img src="assets/tip-icon.png" alt="icona di suggerimento">SUGGERIMENTO: ricorda di consultare sempre il tuo team legale su queste questioni. Chiedi al tuo team quali sono state le iniziative precedenti per mantenere la conformità prima di apportare qualsiasi modifica.</td>
  </tr>
 </tbody>
</table>

## E-mail {#emails}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">Area</th>
   <th>Rivedi focus</th>
  </tr>
  <tr>
   <td>E-mail globali</td>
   <td><li>Quante <a href="/help/marketo/product-docs/email-marketing/general/creating-an-email/create-an-email.md" target="_blank">e-mail globali</a> sono presenti? Vengono utilizzati dai programmi?</li></td>
  </tr>
  <tr>
   <td>Modelli</td>
   <td><li>Quanti <a href="/help/marketo/product-docs/email-marketing/general/email-editor-2/create-an-email-template.md" target="_blank">modelli e-mail</a> sono presenti? Vengono sfruttati?</li></td>
  </tr>
  <tr>
   <td>Test e-mail</td>
   <td><li>In che modo si utilizza <a href="/help/marketo/product-docs/email-marketing/email-programs/email-program-actions/email-test-a-b-test/understanding-email-testing-options.md" target="_blank">test e-mail</a>? Il vostro metodo è ancora efficace?</li></td>
  </tr>
  </tr>
  <tr>
   <td>Privacy e conformità</td>
   <td><li>Tutte le tue e-mail hanno i piè di pagina appropriati? Prendi in considerazione RGPD, CASL, CAN-SPAM, CCPA, ecc. per le implicazioni relative alla conformità.</li>
<p><img src="assets/tip-icon.png" alt="icona di suggerimento">SUGGERIMENTO: ricorda di consultare sempre il tuo team legale per questioni di conformità. Chiedi al tuo team quali sono state le iniziative precedenti per mantenere la conformità prima di apportare qualsiasi modifica.</td>
  </tr>
 </tbody>
</table>

## Snippet {#snippets}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">Area</th>
   <th>Rivedi focus</th>
  </tr>
  <tr>
   <td>Snippet</td>
   <td><li>Quanti <a href="/help/marketo/product-docs/personalization/segmentation-and-snippets/snippets/create-a-snippet.md" target="_blank">snippet</a> sono presenti? Vengono utilizzati?
   <br/>     In caso contrario, è consigliabile utilizzarli per il contenuto del piè di pagina <a href="/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/add-a-snippet-to-an-email.md" target="_blank">e-mail</a> e <a href="/help/marketo/product-docs/demand-generation/landing-pages/personalizing-landing-pages/add-a-snippet-to-a-landing-page.md" target="_blank">Pagina di destinazione</a>, loghi e altro ancora.</li></td>
  </tr>
 </tbody>
</table>

## Tutti Assets {#all-assets}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th style="width:20%">Area</th>
   <th>Rivedi focus</th>
  </tr>
  <tr>
   <td>Stato risorsa</td>
   <td><li>Quante risorse sono in <i>Bozza</i> e <i>Approvate con stato Bozza</i> (ad esempio, <a href="/help/marketo/product-docs/email-marketing/general/creating-an-email/approve-an-email.md" target="_blank">e-mail</a>, <a href="/help/marketo/product-docs/demand-generation/landing-pages/understanding-landing-pages/approve-unapprove-or-delete-a-landing-page.md#approve-a-landing-page" target="_blank">Pagine di destinazione</a>, <a href="/help/marketo/product-docs/demand-generation/forms/creating-a-form/approve-a-form.md" target="_blank">Moduli</a>, <a href="/help/marketo/product-docs/personalization/segmentation-and-snippets/snippets/approve-a-snippet.md" target="_blank">snippet</a>)?
   <br/>     Se ce ne sono molti, puoi eliminarli o approvarli.</li></td>
  </tr>
  <tr>
   <td>Condivisione di risorse</td>
   <td><li>Quali risorse sono <a href="/help/marketo/product-docs/administration/workspaces-and-person-partitions/understanding-workspaces-and-person-partitions.md#sharing-across-workspaces" target="_blank">condivise in Workspace</a>?</li>
   <p><img src="assets/note-icon.png" alt="icona nota"> NOTA: è importante saperlo, in quanto le azioni eseguite in un Workspace potrebbero causare una risorsa inaccessibile a un altro utente in un Workspace diverso.</td>
  </tr>
 </tbody>
</table>
