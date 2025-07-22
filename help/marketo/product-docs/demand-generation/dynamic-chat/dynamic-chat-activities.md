---
description: '[!DNL Dynamic Chat] attività - Documentazione di Marketo - Documentazione del prodotto'
title: '[!DNL Dynamic Chat] attività'
exl-id: ef3bb1a3-6758-4798-92eb-fef28a5ff9c7
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# [!DNL Dynamic Chat] attività {#dynamic-chat-activities}

[!DNL Dynamic Chat] offre diversi filtri e trigger da utilizzare negli elenchi smart.

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
    <td>Un coinvolgimento si verifica la prima volta che un visitatore web fa clic su un prompt in una finestra di dialogo o in un flusso conversazionale (facendo clic su un’opzione a scelta multipla, inviando informazioni, prenotando una riunione, aprendo un documento, ecc). Se un visitatore apre una finestra di dialogo o un flusso conversazionale, ma non fa clic su un prompt, viene registrato un coinvolgimento <b>non</b>. 
    <br>Un evento di coinvolgimento per visitatore, per sessione.</td>
  </tr>
   <tr>
    <td style="width:25%"><b>Coinvolto con un agente</b></td>
    <td>Si verifica quando un visitatore è connesso correttamente a un agente di chat in tempo reale.
    <br>Un evento di agente per visitatore, per sessione.</td>
  </tr>
  <tr>
    <td style="width:25%"><b>Interazione con il documento</b></td>
    <td>Si verifica quando un visitatore fa clic su un documento in una scheda del documento.
    <br>È possibile che esistano più interazioni documento per visitatore, per sessione.</td>
  </tr>
  <tr>
    <td style="width:25%"><b>Obiettivo/i raggiunto</b></td>
    <td>Si verifica quando un visitatore raggiunge un obiettivo. <br>Possono esserci più eventi per obiettivo per visitatore, per sessione.</td>
  </tr>
  <tr>
    <td style="width:25%"><b>Riunione pianificata</b></td>
    <td>Si verifica quando un visitatore registra una riunione con un agente Dynamic Chat.
    <br>Possono essere presenti più eventi prenotati per la riunione per visitatore, per sessione.</td>
  </tr>
</tbody>
</table>

## Aspetti da considerare {#things-to-note}

* Le condizioni sono supportate in [!DNL Dynamic Chat] passaggi di flusso
* È possibile sincronizzare [!DNL Dynamic Chat] attività in [[!DNL Marketo Sales Insight]](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/features/dynamic-chat-integration.md){target="_blank"}
* È possibile visualizzare singole [!DNL Dynamic Chat] attività nel registro attività di un record Persona
