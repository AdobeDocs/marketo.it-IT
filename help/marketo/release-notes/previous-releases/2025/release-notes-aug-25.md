---
description: Note sulla versione - Agosto 2025 - Documentazione Marketo - Documentazione del prodotto
title: Note sulla versione - Agosto 2025
feature: Release Information
hide: true
hidefromtoc: true
source-git-commit: 07b2e888c31c6e98a3207fad5d277261f7f193af
workflow-type: tm+mt
source-wordcount: '598'
ht-degree: 43%

---

# Note sulla versione - Agosto 2025 {#release-notes-aug-25}

Di seguito sono riportate tutte le funzioni incluse nella versione di agosto 2025. Verifica la disponibilità delle funzioni nell‘edizione di Adobe Marketo Engage.

Le note sulla versione specifiche per Adobe Dynamic Chat [sono disponibili qui](/help/marketo/release-notes/dynamic-chat.md){target="_blank"}.

>[!AVAILABILITY]
>
>Le funzionalità contrassegnate da una stella (![star](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante Marketo Engage.

## Funzioni del ciclo di rilascio standard {#standard-release-cycle-features}

Le seguenti funzionalità rientrano nel ciclo di rilascio standard e inizieranno a essere rilasciate il giorno **sabato 22 agosto 2025** con un rollout graduale delle funzioni rimanenti nelle settimane successive. Le funzioni e le date di rilascio sono soggette a modifiche. Verifica lo stato di ciascuna funzionalità.

<table style="table-layout:auto">
 <tbody>
 <tr>
   <th style="width:65%">Funzione</th>
   <th style="width:10%">Stato</th>
   <th style="width:25%">Documentazione</th>
  </tr>
  <tr>
   <td><strong>E-mail Designer - Generazione rapporti</strong>: i rapporti Prestazioni e collegamenti e-mail e Prestazioni e-mail ora mostrano i dati delle e-mail create utilizzando il nuovo Designer e-mail.</td>
   <td>Spedito</td>
   <td>n/d</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-mail Designer - Rimozione completamento automatico</strong>: l'opzione Completamento automatico nell'editor di personalizzazione dei token indicava oggetti errati ed è stata rimossa. Al momento non è prevista la sua reimplementazione.</td>
   <td>Spedito</td>
   <td>n/d</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Designer e-mail - Ottimizzazione anteprima e-mail</strong>: alcuni utenti hanno riscontrato tempi di caricamento più lenti durante il tentativo di visualizzare l'anteprima del messaggio e-mail nella pagina dei dettagli del modello e-mail/frammento. Questa esperienza è stata ottimizzata per tempi di caricamento fino al 60% più rapidi.</td>
   <td>Spedito</td>
   <td>n/d</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-mail Designer - Correzioni di modelli</strong>: alcuni modelli preconfigurati presentavano problemi di rendering (ad esempio, rendering non corretto in alcuni browser/modalità scura, immagini non allineate, pulsanti di CTA posizionati in modo errato e alcuni altri). Questi problemi sono stati risolti con questa versione.</td>
   <td>Spedito</td>
   <td>n/d</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>E-mail Designer - Correzione blocco contenuto</strong>: in precedenza, se si creava un modello di e-mail con blocco del contenuto e il modello veniva utilizzato per creare un'e-mail, il blocco del contenuto persisteva anche quando l'e-mail veniva reimpostata o veniva selezionata l'opzione "Modifica progettazione". Questo problema è stato risolto con questa versione.</td>
   <td>Spedito</td>
   <td>n/d</td>
  </tr>
  <tr>
   <td> </td>
   <td> </td>
   <td> </td>
  </tr>
  <tr>
   <td><strong>Autorizzazione a modificare i limiti di Smart Campaign</strong>: gli amministratori possono ora limitare la possibilità di modificare i limiti di Smart Campaign solo agli utenti con autorizzazioni.</td>
   <td><i>Disponibile a breve</i></td>
   <td><i>Disponibile a breve</i></td>
  </tr>
  </tbody>
</table>
<br/>

## Annunci {#announcements}

* **Fine del ciclo di vita di Marketo Engage Identity**: ad agosto 2025, Adobe ha iniziato a eliminare gradualmente il supporto per Marketo Engage Identity (accesso tramite `login.marketo.com`). Per evitare l&#39;interruzione dell&#39;accesso a Marketo Engage, devi passare a [Adobe Identity](https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview){target="_blank"} entro il 30 settembre 2025.

   * _Deprecazione restrizioni IP_: supporto per [Limitazione degli accessi a Marketo in base all&#39;IP](https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/administration/settings/restrict-marketo-logins-based-on-ip){target="_blank"} terminato il 30 luglio 2025. La funzione rimarrà operativa fino al completamento della transizione ad Adobe Identity. Presto sarà disponibile una nuova funzione di controllo degli accessi basati sulla posizione per Adobe Identity in Adobe Admin Console.

   * _Obsolescenza Single Sign-On (SSO)_: supporto per [Marketo Identity SSO](https://experienceleague.adobe.com/it/docs/marketo/using/product-docs/administration/additional-integrations/add-single-sign-on-to-a-portal){target="_blank"} terminato il 30 luglio 2025. La funzione rimarrà operativa fino al completamento della transizione ad Adobe Identity. Il Single Sign-On per Adobe Identity in Adobe Admin Console deve essere configurato separatamente. Per i passaggi di configurazione, vedi [Configurare identità e Single Sign-On](https://helpx.adobe.com/it/enterprise/using/set-up-identity.html){target="_blank"}.

* **Obsolescenza di _Inoltra a un amico_ funzionalità**: il 29 settembre 2025 la funzionalità _Inoltra a un amico_ nelle e-mail di Marketo Engage 2.0 (l&#39;editor e-mail legacy) diventerà completamente obsoleta per tutti gli abbonamenti. Questo influisce sul token &quot;Inoltra a un amico&quot; e sui collegamenti &quot;Inoltra a un amico&quot; nelle e-mail che sono già state o saranno inviate utilizzando il token. [Ulteriori informazioni](https://nation.marketo.com/t5/product-blogs/deprecation-of-forward-to-a-friend/ba-p/358045#M2889){target="_blank"}

* **Deprecazione parametro &#39;access_token&#39; API Rest**: il parametro di query `access_token` utilizzato per autenticare le chiamate API REST di Marketo è obsoleto e non sarà disponibile dopo il 31 ottobre 2025. Tutte le integrazioni nuove ed esistenti devono autenticare le chiamate API REST utilizzando l&#39;intestazione &#39;Authorization&#39;, [come descritto qui](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/authentication){target="_blank"}.

* **Deprecazione API SOAP**: il supporto per l&#39;API SOAP di Marketo terminerà il 31 ottobre 2025. I servizi che utilizzano le funzionalità API SOAP devono essere migrati all&#39;[API REST](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.
