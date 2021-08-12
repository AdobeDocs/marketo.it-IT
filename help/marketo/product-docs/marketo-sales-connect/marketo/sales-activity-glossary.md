---
description: Glossario delle attività di vendita - Documenti Marketo - Documentazione del prodotto
title: Glossario delle attività di vendita
hide: true
hidefromtoc: true
source-git-commit: 70f17106efe52ee742c8e31013e533fc36ce9835
workflow-type: tm+mt
source-wordcount: '275'
ht-degree: 3%

---

# Glossario delle attività di vendita {#sales-activity-glossary}

In Sales Connect, quando un venditore: aggiunge un lead a una cadenza di vendita, invia loro un’e-mail o effettua una chiamata a un’attività, che verrà registrata nella cronologia delle attività di Marketo. Inoltre, quando il lead si occupa di e-mail, aperture, clic e risposte, viene registrato anche.

Le attività seguenti verranno registrate in Marketo da Sales Connect.

>[!NOTE]
>
>Queste attività e questi attributi sono disponibili per essere utilizzati dalla nostra API REST e Bulk.

## Attività {#activities}

<table>
 <tr>
  <th>Attività di vendita</th>
  <th>Attributo</th>
 </tr>
 <tr>
  <th rowspan="3">Invia e-mail di vendita</th>
  <td>Inviato da</td>
 </tr>
 <tr>
  <td>Fonte</td>
 </tr>
 <tr>
  <td>ID modello</td>
 </tr>
 <tr>
  <th rowspan="3">Apri e-mail di vendita</th>
  <td>Inviato da</td>
 </tr>
 <tr>
  <td>Fonte</td>
 </tr>
 <tr>
  <td>ID modello</td>
 </tr>
 <tr>
  <th rowspan="4">E-mail di vendita selezionata</th>
  <td>Collegamento</td>
 </tr>
 <tr>
  <td>Inviato da</td>
 </tr>
 <tr>
  <td>Fonte</td>
 </tr>
 <tr>
  <td>ID modello</td>
 </tr>
 <tr>
  <th rowspan="2">Email di vendita ricevute</th>
  <td>Ricevuto da</td>
 </tr>
 <tr>
  <td>Fonte</td>
 </tr>
 <tr>
  <th rowspan="4">E-mail di vendita rimbalzata</th>
  <td>Dettagli</td>
 </tr>
 <tr>
  <td>ID modello</td>
 </tr>
 <tr>
  <td>E-mail</td>
 </tr>
 <tr>
  <td>Inviato da</td>
 </tr>
 <tr>
  <th rowspan="7">Chiamata alle vendite ricevute</th>
  <td>Chiamata Di Vendita Effettuata Da</td>
 </tr>
 <tr>
  <td>Stato della chiamata di vendita</td>
 </tr>
 <tr>
  <td>Oggetto della chiamata di vendita</td>
 </tr>
 <tr>
  <td>Nome della campagna di vendita</td>
 </tr>
 <tr>
  <td>URL della campagna di vendita</td>
 </tr>
 <tr>
  <td>Numero di telefono di vendita chiamato</td>
 </tr>
 <tr>
  <td>Fonte</td>
 </tr>
 <tr>
  <th rowspan="6">Aggiungi alla campagna di vendita</th>
  <td>Nome della campagna di vendita</td>
 </tr>
 <tr>
  <td>Stato della chiamata di vendita</td>
 </tr>
 <tr>
  <td>URL della campagna di vendita</td>
 </tr>
 <tr>
  <td>Inviato da</td>
 </tr>
 <tr>
  <td>Fonte</td>
 </tr>
 <tr>
  <td>ID campagna di vendita</td>
 </tr>
 <tr>
  <th rowspan="6">Rimuovi dalla campagna di vendita</th>
  <td>Nome della campagna di vendita</td>
 </tr>
 <tr>
  <td>Stato della chiamata di vendita</td>
 </tr>
 <tr>
  <td>URL della campagna di vendita</td>
 </tr>
 <tr>
  <td>Inviato da</td>
 </tr>
 <tr>
  <td>Fonte</td>
 </tr>
 <tr>
  <td>ID campagna di vendita</td>
 </tr>
</table>

## Descrizioni {#descriptions}

<table> 
 <tr>
  <th>Attributo</th>
  <th>Descrizione</th>
 </tr>
 <tbody> 
  <tr> 
   <td><strong>Inviato da</strong></td>
   <td>Indirizzo e-mail della persona che ha inviato l’e-mail.</td> 
  </tr> 
  <tr> 
   <td><strong>Fonte</strong></td> 
   <td>Origine dell’attività. Sarà impostato come "Tout" per le attività di vendita Connect.</td> 
  </tr> 
  <tr> 
   <td><strong>ID modello</strong></td> 
   <td>Quando l'origine è Tout, l'ID modello sarà l'ID modello di Marketo Sales Connect. Utilizza questa opzione per eseguire il targeting di un modello specifico invece della riga dell’oggetto, che potrebbe essere presente in più modelli.
</td> 
  </tr> 
  <tr> 
   <td><strong>Ricevuto da</strong></td> 
   <td>Indirizzo e-mail della persona che ha inviato l’e-mail.</td> 
  </tr> 
  <tr> 
   <td><strong>Dettagli</strong></td> 
   <td>Dettagli del messaggio di errore non recapitato.</td> 
  </tr> 
  <tr> 
   <td><strong>E-mail</strong></td> 
   <td>Indirizzo e-mail rimbalzato.</td> 
  </tr> 
 </tbody> 
</table>