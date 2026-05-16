---
description: Modello per programma operativo API di acquisizione. Utilizzala per acquisire lead tramite API.
title: OP-Acquisizione da API
feature: Programs
exl-id: abf7c4a0-c363-4e92-9a1f-197c3953c515
TQID: https://experienceleague.adobe.com/a-4w7mJg44cvotVtX2qwx1e4p8SKIbQU1jPWyQ0BzUA
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: a7170d27-32ab-462b-a333-269abc654483id: b13bd2ad-8e65-49e5-9691-2a0d31067b35id: e64968b2-4ee5-47f9-8cae-0588f184b9ebid: f82558ea-6af5-44eb-a424-5b3389abb0a3
topic_v2: id: df401a2a-327d-468c-a5e4-b7b7ccd071a0id: ebde5b41-29c9-4f5e-9ef6-1197e85409e3
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 182
ht-degree: 8%

---

# OP-Acquisizione da API {#op-acquisition-api}

Questo programma di esempio è destinato ai processi operativi per monitorare l’acquisizione di record da origini API che utilizzano un programma predefinito di Marketo Engage.

## Riepilogo canale {#channel-summary}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th>Channel</th>
   <th>Stato iscrizione</th>
   <th>Comportamento di Analytics</th>
   <th>Tipo di programma</th>
  </tr>
  <tr>
   <td>Operativo</td>
   <td>01 membro</td>
   <td>Operativo</td>
   <td>Predefinito</td>
  </tr>
 </tbody>
</table>

## Il programma contiene i seguenti Assets {#program-contains-the-following-assets}

<table style="table-layout:auto">
 <tbody>
  <tr>
   <th>Tipo</th>
   <th>Nome modello</th>
   <th>Nome risorsa</th>
  </tr>
  <tr>
   <td>Campagna avanzata</td>
   <td> </td>
   <td>Imposta acquisizione - Batch</td>
  </tr>
  <tr>
   <td>Campagna avanzata</td>
   <td> </td>
   <td>Imposta acquisizione - Trigger</td>
  </tr>
  <tr>
   <td>Cartella</td>
   <td> </td>
   <td>Campagne (contiene tutte le campagne Smart)</td>
  </tr>
 </tbody>
</table>

![](assets/op-acquisition-api-1.png)

## Regole di conflitto {#conflict-rules}

* **Tag programma**
   * Crea tag in questa sottoscrizione - _Consigliato_
   * Ignora

* **Modello per pagina di destinazione con lo stesso nome**
   * Copia modello originale - _Consigliato_
   * Usa modello di destinazione

* **Immagini con lo stesso nome**
   * Mantieni entrambi i file - _Consigliato_
   * Sostituisci elemento in questa sottoscrizione

* **Modelli e-mail con lo stesso nome**
   * Mantieni entrambi i modelli - _Consigliato_
   * Sostituisci modello esistente

## Best practice {#best-practices}

* Esegui prima la campagna batch se devi recuperare il ritardo nella gestione dei dati.

* Prendi in considerazione l’utilizzo di programmi simili per garantire l’allineamento alle best practice su tutte le origini di input per includere il CRM o le integrazioni di dati.

* Nell&#39;ambito delle iniziative di marketing su canali specifici, assicurati che l&#39;acquisizione venga acquisita quando necessario.
