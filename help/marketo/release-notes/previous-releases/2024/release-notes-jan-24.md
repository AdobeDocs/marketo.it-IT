---
description: Note sulla versione - Gennaio 2024 - Documentazione Marketo - Documentazione del prodotto
title: Note sulla versione - Gennaio 2024
feature: Release Information
exl-id: 64e85f6c-b746-46b6-ab51-5ad1817396b2
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '782'
ht-degree: 1%

---

# Note sulla versione: gennaio 2024 {#release-notes-jan-24}

Qui sotto troverai tutte le funzioni incluse nella versione di gennaio 2024. Verifica la disponibilità delle funzioni nella tua edizione di Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Le funzionalità contrassegnate da una stella (![stella](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante del Marketo Engage.

## Funzioni del ciclo di rilascio standard {#standard-release-cycle-features}

Le seguenti funzionalità rientrano nel ciclo di rilascio standard e inizieranno a essere rilasciate il **12 gennaio 2024**, con un rollout graduale delle funzioni rimanenti nelle settimane successive. Le funzioni e le date di rilascio sono soggette a modifiche. Verifica lo stato di ciascuna funzionalità.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Funzione</th> 
   <th style="width:10%">Stato</th>
   <th style="width:25%">Documentazione</th>
  </tr>
    <tr> 
   <td><strong>Webinar on demand per webinar interattivi</strong>: i webinar on demand consentono di pubblicare la registrazione del webinar e di tenere traccia delle visite/degli orologi. Questo ti aiuterà a ottenere più lead attraverso gli utenti che non hanno partecipato al webinar (no-show) ma sono ancora interessati a scoprire ulteriori dettagli e visualizzare la registrazione.</td> 
   <td>Spedito</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/on-demand-webinars.md" target="_blank">Webinar on demand</a></td>
  </tr>
   <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>Pagine di destinazione conversazionali</strong>: incorpora un flusso conversazionale di Dynamic Chat direttamente in una pagina di destinazione del Marketo Engage in modo che i visitatori possano pianificare una riunione attraverso il Dynamic Chat senza dover compilare un modulo o interagire con un chatbot.</td> 
   <td><i>In arrivo</i></td>
   <td><i>In arrivo</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>Filtro attività bot e-mail</strong>: migliora l'acquisizione dell'attività bot per il coinvolgimento e-mail consentendo di scegliere il livello di aggressività desiderato per il filtro di identificazione dell'attività bot.</td> 
   <td>Spedito</td>
   <td><a href="/help/marketo/product-docs/administration/email-setup/filtering-email-bot-activity.md" target="_blank">Filtraggio dell’attività bot e-mail</a></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
   </tr>
    <tr> 
   <td><strong>Aggiornamento API Importazione lead in blocco</strong>: è stata apportata una modifica minore al comportamento dell'API Importazione lead in blocco quando <b>id</b> è specificato come <b>lookupField</b> durante la creazione del processo. Se un record persona collegato al <b>id</b> specificato non viene trovato nel database di Marketo Engage, non verrà eseguito alcun aggiornamento del record, poiché non è possibile individuare il record. Il comportamento aggiornato ora include l'incremento del conteggio nella proprietà <b>numOfRowsFailed</b> all'interno della risposta, segnalando che l'operazione non è riuscita in questi casi.</td> 
   <td>Spedito</td>
   <td>n/d</td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
   </tr>
  <tr> 
   <td><strong>Co-host per webinar interattivi</strong>: i co-host nella sezione Team webinar dei webinar interattivi consentono al creatore dell'evento di aggiungere utenti interni o esterni al programma Webinar interattivi per condividere responsabilità amministrative e di consegna.</td> 
   <td>Spedito</td>
   <td><a href="/help/marketo/product-docs/demand-generation/events/interactive-webinars/create-an-interactive-webinar.md#adding-a-webinar-team" target="_blank">Aggiunta di un team di webinar</a></td>
  </tr>
  <tr>
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>Rimozione di un utente nei webinar interattivi</strong>: un amministratore di Marketo Engage può ora rimuovere uno o più utenti specifici nei webinar interattivi.</td> 
   <td>Spedito</td>
   <td>n/d</td>
  </tr>
 </tbody> 
</table>
<br/>

## Funzioni di rilascio Agile {#agile-release-features}

Tutte le funzioni seguenti seguono un formato Agile e vengono rilasciate in varie date prima o dopo la data di rilascio standard. Verifica lo stato di ciascuna funzionalità.

### Azioni approfondimento vendite {#sales-insight-actions}

![(stella)](assets/yellow-star.png)

<table style="border: 0px">
 <tbody> 
  <tr> 
   <th style="width:65%">Funzione</th> 
   <th style="width:15%">Stato</th>
   <th style="width:20%">Documentazione</th>
  </tr> 
  </tr>
    <tr> 
   <td><strong>Finestra di composizione espandibile</strong>: la finestra di posta elettronica di composizione comprimerà automaticamente lo spazio inutilizzato, consentendo una maggiore quantità di spazio nell'editor. Inoltre, la finestra può aprirsi ed espandersi ulteriormente, offrendo agli utenti tutto lo spazio necessario per apportare modifiche alle e-mail.</td> 
   <td><i>In arrivo</i></td>
   <td><i>In arrivo</i></td>
  </tr>
 </tbody> 
</table>
<br/>
  </tbody> 
</table>

### Dynamic Chat {#dynamic-chat}

<table style="border: 0px">
 <tbody> 
  <tr> 
   <th style="width:65%">Funzione</th> 
   <th style="width:15%">Stato</th>
   <th style="width:20%">Documentazione</th>
  </tr> 
  </tr>
    <tr> 
   <td><strong>Interfaccia chatbot per Forms conversazionale</strong>: i visitatori del sito Web possono ora richiedere una chat in tempo reale in un flusso conversazionale.</td> 
   <td><i>In arrivo</i></td>
   <td><i>In arrivo</i></td>
  </tr>
   <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
   </tr>
    <tr> 
   <td><strong>Opzioni colore carattere chatbot</strong>: personalizza i colori dei caratteri in una configurazione chatbot.</td> 
   <td><i>In arrivo</i></td>
   <td><i>In arrivo</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
   </tr>
    <tr> 
   <td><strong>Opzione per ripetere la finestra di dialogo</strong>: è ora possibile riavviare la finestra di dialogo all'inizio dopo che un visitatore ha raggiunto la fine.</td> 
   <td><i>In arrivo</i></td>
   <td><i>In arrivo</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    </tr>
    <tr> 
   <td><strong>Terminazione manuale chat in diretta</strong>: sia i visitatori che gli agenti possono ora terminare manualmente una sessione di chat in diretta.</td> 
   <td>Spedito</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/live-chat/agent-inbox.md#end-a-session" target="_blank">Casella in entrata agente</a></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    </tr>
    <tr> 
   <td><strong>Attività di Marketo Engage recenti nella casella in entrata dell'agente</strong>: le attività di Marketo Engage recenti, ad esempio E-mail aperta e modulo compilato, verranno visualizzate per i lead nella casella in entrata dell'agente.</td> 
   <td><i>In arrivo</i></td>
   <td><i>In arrivo</i></td>
  </tr>
  <tr> 
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
    <tr> 
   <td><strong>Diramazione condizionale</strong>: ora puoi mostrare ai visitatori contenuti di conversazione diversi in base a condizioni predefinite, ad esempio la posizione del visitatore o la disponibilità dell'agente live.</td> 
   <td><i>In arrivo</i></td>
   <td><i>In arrivo</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## Annunci {#announcements}

* **Aggiornamento per annullamento iscrizione a mailing list con un solo clic**: Gmail e Yahoo hanno implementato diversi nuovi requisiti del mittente che sono entrati in vigore il 1° febbraio 2024. Scopri [cosa sono e come ti interessano](https://nation.marketo.com/t5/employee-blogs/update-support-for-one-click-list-unsubscribe-for-marketo/ba-p/344514#M352){target="_blank"}.

* **Aggiornamento API lead sincronizzazione**: il comportamento dell&#39;API lead [Sincronizza](https://developer.adobe.com/marketo-apis/api/mapi/#tag/Leads/operation/syncLeadUsingPOST){target="_blank"} è stato leggermente modificato per quanto riguarda gli aggiornamenti al campo `unsubscribed`. Ora, quando si passa `null` come valore, equivale a passare un valore di `false`.

* **Marketo Engage Forms jQuery 1.x**: nella versione di gennaio 2024, aggiorneremo jQuery per Marketo Engage Forms a jQuery 3.x. Questo può influire sull’implementazione di moduli personalizzati basati su versioni precedenti di jQuery. [Ulteriori informazioni](https://nation.marketo.com/t5/product-blogs/marketo-engage-forms-amp-forms2-js-jquery-update/ba-p/341705){target="_blank"}.

* **Verifica e-mail per solo utenti SSO**: solo gli utenti SSO venivano verificati automaticamente, consentendo loro di utilizzare un account e-mail inaccessibile. A partire dalla metà di gennaio, tutti gli utenti SSO Only esistenti non saranno più verificati e verrà richiesto di ricontrollare la posta elettronica tramite un collegamento inviato all&#39;account di posta elettronica. Tutti i nuovi utenti Solo SSO dovranno verificare i propri indirizzi e-mail in futuro.

* Guarda il webinar sulla versione del Marketo Engage di [gennaio 2024](https://engage.marketo.com/2024_January_Release_Webinar_OnDemandPage.html){target="_blank"}.
