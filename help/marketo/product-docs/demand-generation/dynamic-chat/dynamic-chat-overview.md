---
description: Panoramica della chat dinamica - Documenti Marketo - Documentazione del prodotto
title: Panoramica della chat dinamica
exl-id: 73ab651e-bb11-459d-aa6a-39d9e208d512
source-git-commit: f08c85f59113a91d3ce020a11199b7fc4ed58857
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Panoramica della chat dinamica {#dynamic-chat-overview}

La chat dinamica consente di sfruttare un&#39;interfaccia di facile utilizzo per eseguire il targeting sia per le persone che per gli account che visitano il tuo sito web. Raccogli contenuti pertinenti quali nome, informazioni di contatto e testo libero. I visitatori del sito possono anche prenotare riunioni con il team di vendita. I dati di attività e coinvolgimento della chat dinamica possono essere utilizzati per aggiungere membri ai programmi Marketo e attivare attività cross-channel.

>[!NOTE]
>
>La chat dinamica sta per essere implementata gradualmente ed è attualmente a disponibilità limitata. Questa pagina verrà aggiornata con i dettagli di disponibilità generale (GA) man mano che diventano disponibili.

>[!TIP]
>
>Visita [questa pagina](https://experienceleague.adobe.com/docs/marketo-learn/tutorials/dynamic-chat/dynamic-chat-overview.html) per visualizzare i video tutorial della chat dinamica.

## Integrazioni {#integrations}

Un componente chiave della chat dinamica è la sua capacità di interfaccia nativa con il tuo abbonamento Marketo. Per sfruttare appieno la funzionalità di questa integrazione, è innanzitutto necessario avviare la sincronizzazione dei dati. A seconda delle dimensioni del database Marketo, potrebbero essere necessarie fino a 24 ore per i dati iniziali, [sincronizzazione una tantum](/help/marketo/product-docs/demand-generation/dynamic-chat/connect-dynamic-chat-to-marketo.md) da completare.

Viene sincronizzato quanto segue:

* Dati del campo Persona
* Dati sul campo dell&#39;azienda
* Dati attività

## Finestre di dialogo {#dialogues}

Le finestre di dialogo rappresentano un singolo coinvolgimento di chat. Immaginalo come un contenitore con tutte le cose necessarie per avere un dialogo chat coinvolgente con i visitatori del tuo sito web. In ciascuna finestra di dialogo è possibile specificare le pagine sulle quali si desidera visualizzare la finestra di dialogo, le relative pagine e il contenuto e il flusso della finestra stessa. Inoltre, puoi trovare le metriche per vedere le prestazioni della finestra di dialogo. [Ulteriori informazioni sulle finestre di dialogo](/help/marketo/product-docs/demand-generation/dynamic-chat/dialogues.md).

## Configurazione {#configuration}

Nella scheda Configurazione, personalizzare l&#39;aspetto delle varie finestre di dialogo. Cambia font, colori, tempo di risposta e altro ancora! [Ulteriori informazioni sulla configurazione](/help/marketo/product-docs/demand-generation/dynamic-chat/configuration.md).

## Calendario {#calendar}

Nella scheda Calendario, collegare il calendario (Outlook o Gmail) per l&#39;utilizzo nella pianificazione degli appuntamenti nel chatbot. Una volta che il calendario di un utente è connesso a Dynamic Chat, tale utente verrà aggiunto alla coda e il suo calendario sarà disponibile per i visitatori del sito web a pianificare gli appuntamenti in.

Puoi anche personalizzare il corpo dell’invito inviato al visitatore quando questo pianifica un appuntamento sul calendario dell’utente.

## Riunioni {#meetings}

Qui puoi vedere tutti gli appuntamenti pianificati dai visitatori del sito web attraverso le varie finestre di dialogo. Qui trovi l&#39;indirizzo e-mail della persona che ha prenotato l&#39;appuntamento, con quale agente ha prenotato l&#39;appuntamento, quando l&#39;appuntamento è programmato e se la riunione è avvenuta o meno.

## Indirizzamento {#routing}

Qui puoi vedere un elenco di tutti gli agenti che hanno collegato i loro calendari e l&#39;ordine in cui verranno presentati ai visitatori del sito web. Le riunioni vanno in stile robin, quindi se avete cinque agenti e l&#39;agente tre ha preso l&#39;ultima riunione, l&#39;agente quattro avrà quello successivo, seguito dall&#39;agente cinque, poi di nuovo all&#39;agente uno.

## Domande frequenti {#faq}

**Per quanto tempo vengono memorizzati i dati per il reporting?**

90 giorni (vedi l&#39;elenco completo dei limiti) [di seguito](#limits-in-dynamic-chat)).

**La chat dinamica consente la chat dal vivo?**

No, utilizza solo risposte predeterminate.

**Come posso indirizzare le persone anonime?**

Nella finestra di dialogo, devi utilizzare il _L&#39;e-mail della persona è vuota_ attributo.

**Supporta la funzionalità AI/NLP?**

Non è supportata la funzionalità AI/NLP.

**Dynamic Chat offre altre lingue oltre all&#39;inglese?**

Non in questo momento.

## Limiti della chat dinamica {#limits-in-dynamic-chat}

<table>
  <th>Parametro</th>
  <th>Descrizione</th>
  <th>Limite</th>
 <tr>
  <td>Finestre di dialogo totali</td>
  <td>Numero totale di finestre di dialogo (pubblicate e bozza)</td>
  <td>500</td>
 </tr>
 <tr>
  <td>Finestre di dialogo pubblicate</td>
  <td>Numero di finestre di dialogo pubblicate salvate</td>
  <td>100</td>
 </tr>
 <tr>
  <td>URL di destinazione per finestra di dialogo</td>
  <td>Numero di URL di destinazione che possono essere aggiunti a un’unica finestra di dialogo</td>
  <td>20</td>
 </tr>
 <tr>
  <td>Attributi per finestra di dialogo</td>
  <td>Numero di attributi che possono essere aggiunti ai criteri del pubblico per una singola finestra di dialogo</td>
  <td>100</td>
 </tr>
 <tr>
  <td>Gruppi</td>
  <td>Numero di gruppi che possono essere aggiunti a una singola finestra di dialogo</td>
  <td>10</td>
 </tr>
 <tr>
  <td>Attributi per gruppo</td>
  <td>Numero di attributi che possono essere aggiunti a un gruppo</td>
  <td>10</td>
 </tr>
 <tr>
  <td>Schede</td>
  <td>Numero di schede che possono essere aggiunte all’area di lavoro per finestra di dialogo</td>
  <td>500</td>
 </tr>
 <tr>
  <td>Periodo di conservazione dei dati lead anonimi</td>
  <td>Durata per quanto tempo verranno mantenute le informazioni di un lead anonimo senza alcun coinvolgimento</td>
  <td>90 giorni</td>
 </tr>
 <tr>
  <td>Periodo di conservazione dell’attività dell’obiettivo</td>
  <td>Quantità di dati dell’attività dell’obiettivo temporale conservati</td>
  <td>24 mesi</td>
 </tr>
 <tr>
  <td>Periodo di conservazione dell’attività del documento</td>
  <td>Quantità di dati di attività del documento a tempo determinato conservati</td>
  <td>24 mesi</td>
 </tr>
 <tr>
  <td>Interagito con il periodo di conservazione dell’attività della finestra di dialogo</td>
  <td>Il tempo interagito con i dati dell’attività Dialogo viene mantenuto</td>
  <td>90 giorni</td>
 </tr>
 <tr>
  <td>Periodo di conservazione dell'attività di prenotazione riunioni</td>
  <td>Quantità di tempo durante la prenotazione delle riunioni verrà memorizzata in Chat dinamico</td>
  <td>24 mesi</td>
 </tr>
</table>
