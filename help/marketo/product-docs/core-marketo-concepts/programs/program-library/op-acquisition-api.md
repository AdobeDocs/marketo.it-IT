---
description: OP-Acquisition-API - Documentazione di Marketo - Documentazione del prodotto
title: OP-Acquisition-API
feature: Programs
exl-id: abf7c4a0-c363-4e92-9a1f-197c3953c515
source-git-commit: c16081143588ebc0793f5b6e2630b58348e27124
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 2%

---

# OP-Acquisition-API {#op-acquisition-api}

Questo programma di esempio è destinato ai processi operativi per monitorare l’acquisizione di record da origini API che utilizzano un programma predefinito del Marketo Engage.

## Riepilogo canale {#channel-summary}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Canale</th> 
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

* Nell&#39;ambito delle iniziative di marketing su canali specifici, assicurati di acquisire le immagini quando necessario.
