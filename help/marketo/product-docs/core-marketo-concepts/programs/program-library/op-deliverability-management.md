---
description: Gestione della consegna dei messaggi - Documentazione di Marketo - Documentazione del prodotto
title: Gestione recapito messaggi OP
feature: Programs
exl-id: 2c831c7a-f9c9-4308-9610-0e98eeb14288
source-git-commit: 38274b4859ae38c018ee73d4f1715fdf6a78e815
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 4%

---

# Gestione recapito messaggi OP {#op-deliverability-management}

Questo è un esempio di flussi di lavoro basati sulle best practice per la gestione del recapito dei messaggi che utilizzano un programma predefinito di Marketo Engage, per rivedere lo stato attuale del recapito dei messaggi e-mail e gestire i messaggi non recapitati cronici e i non-responder.

>[!NOTE]
>
>Richiede il campo stringa personalizzato &quot;Motivo di sospensione del marketing&quot; per importare. [Ulteriori informazioni](https://nation.marketo.com/community/product_and_support/support_solutions/blog/2016/04/18/how-to-monitor-deliverability-using-marketo){target="_blank"}.

Per ulteriore assistenza sulla strategia o per personalizzare un programma, contatta il team dell’account Adobe o visita il [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html){target="_blank"} pagina.

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

## Campi prerequisiti {#prerequisite-fields}

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <th>Tipo</th> 
   <th>Nome intuitivo</th>
   <th>Nome API</th>
  </tr>
  <tr> 
   <td>Stringa</td> 
   <td>Motivo della sospensione del marketing</td>
   <td>MarketingSuspendedReason</td>
  </tr>
 </tbody> 
</table>

## Il programma contiene le seguenti risorse {#program-contains-the-following-assets}

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
   <td>Non-responder cronici alla sospensione del marketing</td>
  </tr>
  <tr> 
   <td>Campagna avanzata</td> 
   <td> </td>
   <td>E-Mail Con Mancato Recapito Cronico Da Parte Del Marketing</td>
  </tr>
  <tr> 
   <td>Campagna avanzata</td> 
   <td> </td>
   <td>Ripristina "E-mail non valida" dopo l’aggiornamento e-mail</td>
  </tr>
  <tr> 
   <td>Campagna avanzata</td> 
   <td> </td>
   <td>Ripristina "Marketing sospeso" dopo l’aggiornamento dell’e-mail</td>
  </tr>
  <tr> 
   <td>Cartella</td> 
   <td> </td>
   <td>Gestisci</td>
  </tr>
  <tr> 
   <td>Cartella</td> 
   <td> </td>
   <td>Controlla</td>
  </tr>
 </tbody> 
</table>

![](assets/op-deliverability-management-1.png)

## Regole di conflitto {#conflict-rules}

* **Tag del programma**
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

* Ogni campagna creata deve essere un esempio sulla build della best practice e non specifica per i casi d’uso. Ricorda di aggiornare le campagne intelligenti per risolvere problemi specifici e problemi relativi ai dati.

* Prendi in considerazione l’aggiornamento della convenzione di denominazione di questo esempio di programma per allinearla alla convenzione di denominazione.
