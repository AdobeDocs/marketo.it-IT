---
description: Note sulla versione corrente - Documenti Marketo - Documentazione del prodotto
title: Note sulla versione corrente
exl-id: a2eccad5-73ad-48f9-8091-51cee23824e1
feature: Release Information
source-git-commit: a837ec558ae5a845a841d8ea7d9eb3b8a37313e1
workflow-type: tm+mt
source-wordcount: '513'
ht-degree: 1%

---

# Note sulla versione: ottobre 2024 {#release-notes-oct-24}

Qui sotto troverai tutte le funzioni incluse nella versione di ottobre 2024. Verifica la disponibilità delle funzioni nella tua edizione di Adobe Marketo Engage.

Le note sulla versione specificatamente per l&#39;Adobe Dynamic Chat [ si trovano qui](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Le funzionalità contrassegnate da una stella (![stella](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante del Marketo Engage.

## Funzioni del ciclo di rilascio standard {#standard-release-cycle-features}

Le seguenti funzionalità rientrano nel ciclo di rilascio standard e inizieranno a essere rilasciate il **4 ottobre 2024**, con un rollout graduale delle funzioni rimanenti nelle settimane successive. Le funzioni e le date di rilascio sono soggette a modifiche. Verifica lo stato di ciascuna funzionalità.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th style="width:65%">Funzione</th> 
   <th style="width:10%">Stato</th>
   <th style="width:25%">Documentazione</th>
  </tr>
    <tr> 
   <td><strong>Dati di registrazione migliorati in Engagement Dashboard per webinar interattivi</strong>: è ora possibile vedere quali società hanno avuto più presenze e ottenere l'aggiornamento di società, titolo e settore a livello di lead nei report disponibili in Engagement Dashboard.</td> 
   <td><i>In arrivo</i></td>
   <td><i>In arrivo</i></td>
  </tr>
   <td> </td> 
   <td> </td>
   <td> </td>
  </tr>
  </tr>
    <tr> 
   <td><strong>Tokenizzazione per i webinar interattivi</strong>: ora puoi utilizzare i token per promuovere i webinar interattivi nelle e-mail e nelle pagine di destinazione senza dover aggiungere manualmente i dettagli del webinar.</td> 
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
   <td><strong>Conteggio "Influenza" elenco smart</strong>: verifica il numero di persone interessate dalla modifica delle regole di qualifica di una campagna smart.</td> 
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
   <td><strong>Pulsante Account personale nella barra di navigazione</strong>: per coloro che hanno eseguito la migrazione ad Adobe Identity Management System, un nuovo pulsante "Account personale" nella barra di navigazione a sinistra consente di configurare il fuso orario e di accedere ai dettagli dell'abbonamento.</td> 
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
   <td><strong>Metriche backlog sincronizzazione Salesforce</strong>: è ora possibile monitorare le tendenze della velocità effettiva di sincronizzazione e del backlog per pianificare e pianificare gli aggiornamenti CRM per un'esperienza di sincronizzazione ottimale.</td> 
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
   <td><strong>Miglioramenti al report delle prestazioni delle e-mail</strong>: sono stati apportati diversi miglioramenti alle metriche di reporting e al tracciamento delle attività e-mail, offrendo ulteriori informazioni e migliorando la precisione.
   <ul>
   <li>Filtrare le persone eliminate e unite dalle metriche delle prestazioni delle e-mail</li>
   <li>Le e-mail sono ora classificate come <i>interrotte</i> dopo tre giorni di attesa per l'attività di risposta</li>
   <li>L’e-mail dell’account viene aperta a livello di campagna</li>
   <li>È stato migliorato il tracciamento delle attività e-mail tramite il perfezionamento della posizione dei pixel di tracciamento</li>
   </td> 
   <td><i>In arrivo</i></td>
   <td><i>In arrivo</i></td>
  </tr>
 </tbody> 
</table>
<br/>

## Annunci {#announcements}

* **Deprecazione del codice QR**: il 4 ottobre 2024 la funzione del codice QR utilizzata nelle notifiche push e nelle risorse di messaggistica in-app diventerà obsoleta. Ciò include l&#39;utilizzo di codici QR per un nuovo dispositivo di test e la creazione di nuove risorse con codici QR. Le funzioni obsolete con un utilizzo inferiore ci consentono di riallocare le loro risorse alla manutenzione complessiva del Marketo Engage.

* **Modifiche Munchkin**

   * **Nuova versione**: il 17 settembre 2024, [Munchkin](/help/marketo/product-docs/administration/setup-administration/munchkin.md){target="_blank"} v.164 inizierà il rollout per le istanze di Marketo Engage in cui l&#39;impostazione &quot;Munchkin Beta&quot; è abilitata in **Admin** > **Treasure Chest**. È pianificato per l’inizio del rollout per tutte le altre istanze il 29 ottobre. Questa versione aggiorna la creazione dei cookie di Munchkin. Nessuna modifica nelle funzionalità.

   * **Caratteri rimossi dall&#39;URL**: le attività &#39;Pagina Web visite&#39; e &#39;Collegamento clic&#39; create da Munchkin JS ora rimuoveranno i caratteri di controllo non codificati dall&#39;URL da tutti i campi URL. Questa modifica è stata progettata per evitare errori relativi alla propagazione di questi tipi di caratteri in sistemi che non li supportano e che non sono utilizzati in modo valido all&#39;interno del Marketo Engage.
