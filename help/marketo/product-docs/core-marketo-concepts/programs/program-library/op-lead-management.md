---
description: Gestione dei lead operativi - Documentazione di Marketo - Documentazione del prodotto
title: Gestione OP-Lead
feature: Programs
exl-id: 28db1a91-a559-4dcb-b2e3-9cb2c0c23f9f
source-git-commit: 38274b4859ae38c018ee73d4f1715fdf6a78e815
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 2%

---

# Gestione OP-Lead {#op-lead-management}

Questo è un esempio di flussi di lavoro basati sulle best practice per la gestione dei lead, che utilizzano un programma predefinito di Marketo Engage, per aiutarti a gestire i record all’interno del database di Marketo Engage al tuo CRM.

>[!NOTE]
>
>In Marketo Engage, i record del database sono denominati persone/persone. La gestione dei lead in questo esempio fa riferimento ai record nel CRM.

Per ulteriore assistenza sulla strategia o per personalizzare un programma, contatta il team dell’account Adobe o visita il [Adobe Professional Services](https://business.adobe.com/customers/consulting-services/main.html) pagina.

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
   <td>01 - Sincronizza nuove persone con CRM</td>
  </tr>
  <tr> 
   <td>Campagna avanzata</td> 
   <td> </td>
   <td>02 - Qualificati per il marketing</td>
  </tr>
  <tr> 
   <td>E-mail</td> 
   <td><a href="/help/marketo/product-docs/core-marketo-concepts/programs/program-library/quick-start-email-template.md" target="_blank">Modello e-mail di avvio rapido</a></td>
   <td>01 - E-mail - AVVISO - MQL</td>
  </tr>
  <tr> 
   <td>Cartella</td> 
   <td> </td>
   <td>Campagne</td>
  </tr>
  <tr> 
   <td>Cartella</td> 
   <td> </td>
   <td>Avviso e-mail</td>
  </tr>
 </tbody> 
</table>

![](assets/op-lead-management-1.png)

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

* Prendi in considerazione l’aggiunta di ulteriori campagne intelligenti per soddisfare ogni esigenza di stato del ciclo di vita che potresti tenere traccia nella tua organizzazione. Ogni campagna creata in questo programma è destinata a essere un esempio della build delle best practice e non è specifica per tutti i casi d’uso. Ricorda di aggiornare le campagne avanzate in base al tuo specifico processo di gestione del ciclo di vita dei lead.

* Prendi in considerazione l’aggiornamento della convenzione di denominazione di questo esempio di programma per allinearla al tuo.
