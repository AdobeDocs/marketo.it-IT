---
description: Note sulla versione - Ottobre 2022 - Documentazione di Marketo - Documentazione del prodotto
title: Note sulla versione - Ottobre 2022
exl-id: 1494b8b9-049c-4969-ab95-a4be41d886b0
feature: Release Information
TQID: https://experienceleague.adobe.com/8d05i8J-yT1oEfPeF8Wn3Ir2Yy9SG6bswhaTA-oRwIw
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b0bb9048-d951-48d8-8232-45cf248a7e27id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45id: d1d0a9cd-295d-4976-8c39-ddae266f240eid: e64968b2-4ee5-47f9-8cae-0588f184b9eb
subfeature_v2: id: efc9a24a-a6a4-449d-a3e6-44f6c74dfd46
topic_v2: id: e1e0219c-f879-479f-8427-888ed2a6e9c2id: eddd9b14-83bd-4ff4-9072-54a4a484abb7id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 619
ht-degree: 21%

---

# Note sulla versione - Ottobre 2022 {#release-notes-oct-22}

Qui sotto trovi tutte le funzioni incluse nella versione di ottobre 2022. Verifica la disponibilità delle funzioni nell‘edizione di Adobe Marketo Engage.

>[!AVAILABILITY]
>
>Le funzionalità contrassegnate da una stella (![star](assets/yellow-star.png)) sono componenti aggiuntivi a pagamento. Per ulteriori informazioni, contatta il rappresentante Marketo Engage.

## Funzioni del ciclo di rilascio standard {#standard-release-cycle-features}

Le seguenti funzioni rientrano nel ciclo di rilascio standard. Inizieranno a essere rilasciate il **sabato 14 ottobre 2022**, con un rollout graduale delle funzioni rimanenti nelle settimane successive. Le funzioni e le date di rilascio sono soggette a modifiche. Di seguito è riportato lo stato di ciascuna funzionalità.

### Ambiente dati di marketing {#marketing-data-environment}

</br>

* **Sincronizzazione campo personalizzato membro del programma**: possibilità di sincronizzare in modo bidirezionale i campi estensibili acquisiti per un membro del programma (ad esempio, le preferenze del partecipante durante la registrazione dell&#39;evento come cibo, sessioni, brani, ecc.) con Campi membro della campagna in Salesforce.

<table>
  <tr>
   <td><b>Stato</b></td>
   <td><b>Aggiornamenti alla documentazione</b></td>
  </tr>
  <tr>
   <td>Rilasciato</td>
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-field-sync.md">Sincronizzazione campo personalizzato del membro del programma</a></td>
  </tr>
  </tbody>
</table>

* **Integrazione di Adobe Privacy Service**: esegui l&#39;armonizzazione con Privacy Service per automatizzare la conformità alle normative sulla privacy dei dati nei prodotti Experience Cloud. Attualmente, questo servizio è disponibile solo per i clienti Marketo Engage che hanno effettuato l’onboarding in Adobe Identity Management System.

<table>
  <tr>
   <td><b>Stato</b></td>
   <td><b>Aggiornamenti alla documentazione</b></td>
  </tr>
  <tr>
   <td>Rilasciato</td>
   <td><a href="/help/marketo/product-docs/administration/marketo-with-adobe-identity/adobe-identity-management-overview.md">Adobe Identity Management</a></td>
  </tr>
  </tbody>
</table>

### Esperienza di nuova generazione {#modern-ux}

</br>

* **Screens aggiornato nell&#39;esperienza di nuova generazione**: verranno forniti schermi aggiuntivi e aggiornati nell&#39;esperienza di nuova generazione che offrono una progettazione aggiornata e miglioramenti a livello di usabilità accessibili tramite l&#39;interruttore:

   * Dettagli modello pagina di destinazione
   * Elenco modelli e-mail

<table>
  <tr>
   <td><b>Stato</b></td>
   <td><b>Aggiornamenti alla documentazione</b></td>
  </tr>
  <tr>
   <td>Rilasciato</td>
   <td><a href="/help/marketo/product-docs/marketo-engage-modern-ux/toggle-switch.md">Attiva/Disattiva</a></td>
  </tr>
  </tbody>
</table>

* **Utilizzo ottimizzato da scheda in Dettagli modello e-mail**: nella nuova esperienza verranno visualizzate informazioni aggiuntive relative alle risorse che utilizzano il modello e-mail, inclusi Stato risorsa, Ultima modifica e Ultima modifica di. Puoi anche cercare, ordinare e filtrare l’elenco delle risorse utilizzate.

<table>
  <tr>
   <td><b>Stato</b></td>
   <td><b>Aggiornamenti alla documentazione</b></td>
  </tr>
  <tr>
   <td>Rilasciato</td>
   <td>n/d</td>
  </tr>
  </tbody>
</table>

* **Modali filtro risorse report**: nuova progettazione per i moduli di configurazione dei report con una nuova struttura di risorse nel menu di configurazione e un filtro per Data di creazione e Modifica.

<table>
  <tr>
   <td><b>Stato</b></td>
   <td><b>Aggiornamenti alla documentazione</b></td>
  </tr>
  <tr>
   <td>Rilasciato</td>
   <td>n/d</td>
  </tr>
  </tbody>
</table>

### Miglioramenti API {#api-enhancements}

</br>

* **Importazione lead in blocco: associazione venditore**: parità con API REST lead per associare i lead ai venditori durante il processo di importazione dei lead in blocco, riducendo la complessità e il numero di chiamate API richieste.

<table>
  <tr>
   <td><b>Stato</b></td>
   <td><b>Aggiornamenti alla documentazione</b></td>
  </tr>
  <tr>
   <td>Rilasciato</td>
   <td><a href="https://developer.adobe.com/marketo-apis/api/mapi/#tag/Bulk-Import-Leads">Importazione lead in blocco</a></td>
  </tr>
  </tbody>
</table>

### Insight di vendita {#sales-insight}

</br>

![(stella)](assets/yellow-star.png)

* **Integrazione di Sales Insight con Dynamic Chat**: il dashboard approfondimenti ora include le attività Dynamic Chat in Smart Grid insieme a un riepilogo settimanale e schede di dettagli.

<table>
  <tr>
   <td><b>Stato</b></td>
   <td><b>Aggiornamenti alla documentazione</b></td>
  </tr>
  <tr>
   <td>Rilasciato</td>
   <td><a href="/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/dynamic-chat-integration.md">Integrazione Dynamic Chat</a></td>
  </tr>
  </tbody>
</table>

## Funzioni di rilascio Agile

Le seguenti funzioni seguono un formato Agile e vengono rilasciate in varie date prima o dopo la data di rilascio standard. Di seguito è riportato lo stato di ciascuna funzionalità.

* **Flussi per finestre di dialogo di disposizione automatica per Dynamic Chat**: migliora l&#39;area di lavoro della finestra di dialogo di gruppo organizzando tutto ciò che si trova nell&#39;area di lavoro in un formato pulito e di facile lettura con la pressione di un pulsante tramite Disponi automaticamente.

<table>
  <tr>
   <td><b>Stato</b></td>
   <td><b>Aggiornamenti alla documentazione</b></td>
  </tr>
  <tr>
   <td>Rilasciato</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/stream-designer.md#stream-designer-icons">Icone Streaming Designer</a></td>
  </tr>
  </tbody>
</table>

* **Collegamenti riunione per Dynamic Chat**: opzione per includere automaticamente un collegamento Team o Incontro per Google e Outlook in ogni invito del calendario inviato ai visitatori.

<table>
  <tr>
   <td><b>Stato</b></td>
   <td><b>Aggiornamenti alla documentazione</b></td>
  </tr>
  <tr>
   <td>Rilasciato</td>
   <td><a href="/help/marketo/product-docs/demand-generation/dynamic-chat/setup-and-configuration/agent-settings.md">Calendario</a></td>
  </tr>
  </tbody>
</table>

* **Supporta tipi di dati aggiuntivi per Dynamic Chat**: tre nuovi tipi di dati (booleano, intero, in virgola mobile) consentono di sfruttare più campi Marketo Engage esistenti in Dynamic Chat per elementi quali il targeting in base a punteggi o la richiesta ai visitatori di domande sì/no.

<table>
  <tr>
   <td><b>Stato</b></td>
   <td><b>Aggiornamenti alla documentazione</b></td>
  </tr>
  <tr>
   <td>Rilasciato</td>
   <td>n/d</td>
  </tr>
  </tbody>
</table>

## Annunci {#announcements}

* **Forms 1.0**: la versione obsoleta di Forms 1.0 verrà completata con la versione di ottobre. Le risorse di Forms 1.0 non saranno più in grado di inviare dati a Marketo Engage e, se tentate, restituiranno errori.

* **Forms senza script**: Forms non funzionerà più se JavaScript è disabilitato nel browser. Per l’invio di un modulo è necessario abilitare JavaScript.
