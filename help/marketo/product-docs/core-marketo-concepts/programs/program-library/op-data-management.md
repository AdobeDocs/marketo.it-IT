---
description: Gestione dei dati operativi - Documentazione di Marketo - Documentazione del prodotto
title: Gestione dei dati operativi
feature: Programs
exl-id: 21cd86b2-e924-4326-bbf7-32a03a3eb224
source-git-commit: 38274b4859ae38c018ee73d4f1715fdf6a78e815
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 2%

---

# Gestione dei dati operativi {#op-data-management}

Questo è un esempio di semplici flussi di lavoro basati sulle best practice per la gestione dei dati operativi che utilizzano un programma predefinito, per aiutarti a gestire la coerenza dei dati per i record nel database di Marketo Engage.

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
   <td>Normalizza paese - Stati Uniti</td>
  </tr>
  <tr> 
   <td>Campagna avanzata</td> 
   <td> </td>
   <td>Normalizza paese - Regno Unito</td>
  </tr>
  <tr> 
   <td>Campagna avanzata</td> 
   <td> </td>
   <td>Inserire nell'elenco Bloccati Imposta l'su True</td>
  </tr>
  <tr> 
   <td>Campagna avanzata</td> 
   <td> </td>
   <td>Imposta partner IS su True</td>
  </tr>
  <tr> 
   <td>Campagna avanzata</td> 
   <td> </td>
   <td>Importazione elenco</td>
  </tr>
  <tr> 
   <td>Campagna avanzata</td> 
   <td> </td>
   <td>Evento live</td>
  </tr>
  <tr> 
   <td>Campagna avanzata</td> 
   <td> </td>
   <td>Pubblicità online</td>
  </tr>
  <tr> 
   <td>Campagna avanzata</td> 
   <td> </td>
   <td>Fiera</td>
  </tr>
  <tr> 
   <td>Campagna avanzata</td> 
   <td> </td>
   <td>Contenuto web</td>
  </tr>
  <tr> 
   <td>Campagna avanzata</td> 
   <td> </td>
   <td>Richiesta Web</td>
  </tr>
  <tr> 
   <td>Campagna avanzata</td> 
   <td> </td>
   <td>Webinar</td>
  </tr>
  <tr> 
   <td>Campagna avanzata</td> 
   <td> </td>
   <td>Nuova persona da importazione elenco</td>
  </tr>
  <tr> 
   <td>Campagna avanzata</td> 
   <td> </td>
   <td>Nuova persona da evento live</td>
  </tr>
  <tr> 
   <td>Campagna avanzata</td> 
   <td> </td>
   <td>Nuova persona dalla pubblicità online</td>
  </tr>
  <tr> 
   <td>Campagna avanzata</td> 
   <td> </td>
   <td>Nuova persona da fiera</td>
  </tr>
   <tr> 
   <td>Campagna avanzata</td> 
   <td> </td>
   <td>Nuova persona dal contenuto web</td>
  </tr>
   <tr> 
   <td>Campagna avanzata</td> 
   <td> </td>
   <td>Nuova persona da richiesta web</td>
  </tr>
   <tr> 
   <td>Campagna avanzata</td> 
   <td> </td>
   <td>Nuova persona dal webinar</td>
  </tr>
  <tr> 
   <td>Cartella</td> 
   <td> </td>
   <td>Batch notturno sorgente persona (per le istanze con traffico elevato)</td>
  </tr>
  <tr> 
   <td>Cartella</td> 
   <td> </td>
   <td>Sorgente della persona attivata (per istanze a traffico ridotto)</td>
  </tr>
  <tr> 
   <td>Cartella</td> 
   <td> </td>
   <td>Acquisire l’origine della persona</td>
  </tr>
  <tr> 
   <td>Cartella</td> 
   <td> </td>
   <td>Normalizzazione</td>
  </tr>
  <tr> 
   <td>Cartella</td> 
   <td> </td>
   <td>Gestione record</td>
  </tr>
  <tr> 
   <td>Cartella</td> 
   <td> </td>
   <td>INSERISCO NELL'ELENCO BLOCCATI DI</td>
  </tr>
 </tbody> 
</table>

![](assets/op-data-management-1.png)

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
