---
description: Attività di Dynamic Chat - Documentazione Marketo - Documentazione del prodotto
title: Attività Dynamic Chat
feature: Dynamic Chat
exl-id: ef3bb1a3-6758-4798-92eb-fef28a5ff9c7
source-git-commit: 79b439a9bb3d3cd130eb5a7b52cea13988e7b88e
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 0%

---

# Attività Dynamic Chat {#dynamic-chat-activities}

Il Dynamic Chat offre diversi filtri e attivatori da utilizzare negli elenchi avanzati.

![](assets/dynamic-chat-activities-1.png)

## Definizioni {#definitions}

<table>
<thead>
<tbody>
  <tr>
    <td style="width:25%"><b>Attivato</b></td>
    <td>Un evento trigger si verifica quando un visitatore soddisfa i criteri di targeting per un dialogo o un flusso conversazionale e viene visualizzato nel dialogo.
    <br>Un evento trigger per visitatore, per sessione.</td>
  </tr>
  <tr>
    <td style="width:25%"><b>Coinvolto con un flusso/finestra di dialogo per conversazione</b></td>
    <td>Un coinvolgimento si verifica la prima volta che un visitatore web fa clic su un prompt in una finestra di dialogo o in un flusso conversazionale (facendo clic su un’opzione a scelta multipla, inviando informazioni, prenotando una riunione, aprendo un documento, ecc). Se un visitatore apre una finestra di dialogo o un flusso conversazionale, ma non fa clic su un prompt, il coinvolgimento è <b>non</b> registrato. 
    <br>Un evento di coinvolgimento per visitatore, per sessione.</td>
  </tr>
   <tr>
    <td style="width:25%"><b>Coinvolto con un agente</b></td>
    <td>Si verifica quando un visitatore è connesso correttamente a un agente di chat in tempo reale.
    <br>Uno impegnato con un evento agente per visitatore, per sessione.</td>
  </tr>
  <tr>
    <td style="width:25%"><b>Interazione con il documento</b></td>
    <td>Si verifica quando un visitatore fa clic su un documento in una scheda del documento.
    <br>È possibile che esistano più interazioni con i documenti per visitatore e per sessione.</td>
  </tr>
  <tr>
    <td style="width:25%"><b>Obiettivo/i raggiunto</b></td>
    <td>Si verifica quando un visitatore raggiunge un obiettivo. <br>Possono essere presenti più eventi con obiettivo per visitatore, per sessione.</td>
  </tr>
  <tr>
    <td style="width:25%"><b>Riunione pianificata</b></td>
    <td>Si verifica quando un visitatore registra una riunione con un agente di Dynamic Chat.
    <br>Possono esserci più eventi prenotati per la riunione per visitatore, per sessione.</td>
  </tr>
</tbody>
</table>

## Aspetti da considerare {#things-to-note}

* Le condizioni sono supportate nei passaggi del flusso di Dynamic Chat
* Le attività di Dynamic Chat possono essere sincronizzate con [Insight sulla vendita di Marketo](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/dynamic-chat-integration.md){target="_blank"}
* È possibile visualizzare singole attività di Dynamic Chat nel registro attività di un record Persona
