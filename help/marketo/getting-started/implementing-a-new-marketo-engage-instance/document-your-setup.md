---
description: Documenta la configurazione della nuova istanza di Marketo Engage.
title: Tecniche consigliate per le nuove istanze - Documentare la configurazione
feature: Getting Started
exl-id: c64d25e8-564b-487d-824e-7fcbfbf5d8bb
TQID: https://experienceleague.adobe.com/pqbf84tAUt49rWUD7rONRuZNgR8v5yMmYTqwqlXqgAs
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2:
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
  - id: c5f60233-d5ea-4453-a799-0ad258b4d399
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
  - id: e64968b2-4ee5-47f9-8cae-0588f184b9eb
topic_v2:
  - id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adeb
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 536
ht-degree: 4%

---

# Best practice per la nuova istanza: documenta la tua configurazione {#new-instance-best-practices-document-your-setup}

Dopo aver appreso le aree principali del prodotto da configurare per una nuova istanza di Marketo Engage, il passaggio successivo consiste nel creare la documentazione per la configurazione dell’istanza e lo stack tecnologico. La documentazione, sia che venga creata tramite foglio di calcolo o un’applicazione di gestione dei progetti, sarà un’ottima risorsa per monitorare lo stato di avanzamento e registrare i dettagli, nonché per mantenere la struttura e la sostenibilità della tua istanza per gli esperti di marketing futuri all’interno della tua organizzazione.

## Dati {#data}

<table>
<thead>
  <tr>
    <th style="width:20%">Area</th>
    <th style="width:80%">Elementi azione</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Importazione elenco</td>
    <td><li>Raccogliere un elenco di origini dati da cui verranno estratti i record in <a href="https://experienceleague.adobe.com/it/docs/marketo/using/getting-started/quick-wins/import-a-list-of-people" target="_blank">importa in Marketo Engage</a>.</li>
    <li>Se si esegue l'importazione da più origini dati, è consigliabile utilizzare Elenchi master o <a href="https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/administration/field-management/create-a-custom-field-in-marketo" target="_blank">creare un campo personalizzato</a> nel record persona per indicare l'origine dati.</li></td>
  </tr>
  <tr>
    <td>Integrazione del database</td>
    <td><li>Se sfrutti la sincronizzazione nativa tra Marketo Engage e il CRM, considera con attenzione quali campi desideri sincronizzare tra i sistemi. Non tutti i campi devono essere sincronizzati, quindi fai attenzione ai flussi di dati in modo strategico.</li></td>
  </tr>
</tbody>
</table>

## Documentazione {#documentation}

<table>
<thead>
  <tr>
    <th style="width:20%">Area</th>
    <th style="width:80%">Elementi azione</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Utenti</td>
    <td><li>Documenta gli <a href="https://experienceleague.adobe.com/en/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/add-or-remove-a-user#add-a-user" target="_blank">utenti correnti</a> nella tua istanza per motivi di sicurezza. I seguenti dettagli devono essere inclusi come minimo (e sono tutti visibili andando in Amministratore &gt; Utenti e ruoli):</li>
    <ul>
    <li>Nome</li>
    <li>E-mail</li>
    <li>Login</li>
    <li>Ruolo</li>
    <li>Data di scadenza dell’accesso</li>
    <li>Data di creazione utente</li>
    <li>Data di accesso più recente</li></ul>
    <p><img src="assets/note-icon.png" alt="icona nota"> NOTA: puoi anche approfondire questo argomento per includere la documentazione su ruoli/autorizzazioni.
    <p>
    <li>In qualità di amministratore di prodotto Marketo Engage, sviluppa un processo interno per controllare e aggiornare l’elenco degli utenti di Marketo Engage con cadenza regolare. Per apportare modifiche all'elenco degli utenti in Adobe Admin Console, considera <a href="https://helpx.adobe.com/it/enterprise/using/users.html" target="_blank">azioni in blocco</a>, ad esempio il caricamento di un file CSV, l'utilizzo dell'API REST per la gestione degli utenti e così via.</li></td>
  </tr>
  <tr>
    <td>Organizzazione</td>
    <td><li>Documenta la struttura delle cartelle concordata, le convenzioni di denominazione standard per programmi, risorse e così via, e il motivo delle decisioni adottate. <a href="https://experienceleague.adobe.com/it/docs/marketo-learn/tutorials/fundamentals/best-practices-to-organize-a-new-instance" target="_blank">Ulteriori informazioni sulle best practice disponibili qui.</a></li></td>
  </tr>
  <tr>
    <td>Changelog</td>
    <td><li>Crea un registro delle modifiche in cui puoi documentare le modifiche apportate all’istanza e il motivo per cui sono state apportate. <a href="https://experienceleague.adobe.com/it/docs/marketo-learn/auditing-an-inherited-instance/develop-an-instance-governance-guide" target="_blank">Ulteriori informazioni sulle best practice disponibili qui.</a></li></td>
  </tr>
  <tr>
    <td>Playbook</td>
    <td><li>Crea un playbook utente o un playbook amministratore per gli utenti interni che effettuano l’onboarding nell’istanza.</li></td>
  </tr>
  <tr>
    <td>Conversazioni con i team interni</td>
    <td><li>Allinea le aspettative del team di marketing interno su Marketo Engage alle funzionalità di Marketo Engage.</li>
    <li>Identifica i team che saranno le parti interessate nell’istanza di Marketo Engage e documenta i loro obiettivi da raggiungere utilizzando Marketo Engage come tecnologia.</li></td>
  </tr>
  <tr>
    <td>Aree di lavoro e partizioni (se applicabile)</td>
    <td><li>Documenta la definizione delle aree di lavoro e le correlazioni con le partizioni del database (ad esempio, un’area di lavoro globale che mostra tutti rispetto ai settori aziendali).</li>
    <li>Importare nuovi record nella partizione appropriata.</li>
    <li>Definisci il valore nel CRM che colloca gli utenti nella partizione appropriata.</li></td>
  </tr>
</tbody>
</table>
