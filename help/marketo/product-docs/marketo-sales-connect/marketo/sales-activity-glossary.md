---
description: Glossario delle attività di vendita - Documenti Marketo - Documentazione del prodotto
title: Glossario delle attività di vendita
exl-id: c7805642-07b6-4697-9efe-5c673ae9ca53
source-git-commit: 9677c26004a567bb53fef452304665eb73855568
workflow-type: tm+mt
source-wordcount: '480'
ht-degree: 1%

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
  <th rowspan="9">Invia e-mail di vendita</th>
  <td>Inviato da</td>
 </tr>
 <tr>
  <td>Fonte</td>
 </tr>
 <tr>
  <td>ID modello</td>
 </tr>
 <tr>
  <td>URL del modello di vendita</td>
 </tr>
 <tr>
  <td>URL della campagna di vendita</td>
 </tr>
 <tr>
  <td>Nome del modello di vendita</td>
 </tr>
 <tr>
  <td>Oggetto e-mail</td>
 </tr>
 <tr>
  <td>Nome della campagna di vendita</td>
 </tr>
 <tr>
  <td>ID persona di vendita Marketo</td>
 </tr>
 <tr>
  <th rowspan="9">Apri e-mail di vendita</th>
  <td>Inviato da</td>
 </tr>
 <tr>
  <td>Fonte</td>
 </tr>
 <tr>
  <td>ID modello</td>
 </tr>
 <tr>
  <td>URL del modello di vendita</td>
 </tr>
 <tr>
  <td>URL della campagna di vendita</td>
 </tr>
 <tr>
  <td>Nome del modello di vendita</td>
 </tr>
 <tr>
  <td>Oggetto e-mail</td>
 </tr>
 <tr>
  <td>Nome della campagna di vendita</td>
 </tr>
 <tr>
  <td>ID persona di vendita Marketo</td>
 </tr>
 <tr>
  <th rowspan="10">E-mail di vendita selezionata</th>
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
  <td>URL del modello di vendita</td>
 </tr>
 <tr>
  <td>URL della campagna di vendita</td>
 </tr>
 <tr>
  <td>Nome del modello di vendita</td>
 </tr>
 <tr>
  <td>Oggetto e-mail</td>
 </tr>
 <tr>
  <td>Nome della campagna di vendita</td>
 </tr>
 <tr>
  <td>ID persona di vendita Marketo</td>
 </tr>
<tr>
  <th rowspan="3">Email di vendita ricevute</th>
  <td>Ricevuto da</td>
 </tr>
 <tr>
  <td>Fonte</td>
 </tr>
 <tr>
  <td>ID persona (MSC)</td>
 </tr>
 <tr>
  <th rowspan="11">Chiamata alle vendite ricevute</th>
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
  <td>Durata chiamata vendite</td>
 </tr>
 <tr>
  <td>URL registrazione chiamata vendita</td>
 </tr>
  <tr>
  <td>Risposta alla chiamata di vendita da</td>
 </tr>
 <tr>
  <td>ID persona di vendita Marketo (MSC)</td>
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
   <td><strong>Dettagli</strong></td> 
   <td>Dettagli del messaggio di errore non recapitato.</td> 
  </tr> 
  <tr> 
   <td><strong>E-mail</strong></td> 
   <td>Indirizzo e-mail rimbalzato.</td> 
  </tr> 
  <tr> 
   <td><strong>Collegamento</strong></td> 
   <td>URL su cui è stato fatto clic.</td> 
  </tr> 
  <tr> 
   <td><strong>Ricevuto da</strong></td> 
   <td>Indirizzo e-mail della persona che ha inviato l’e-mail.</td> 
  </tr>
  <tr> 
   <td><strong>Risposta alla chiamata di vendita da</strong></td> 
   <td>Nome della persona che ha risposto alla chiamata.</td> 
  </tr>
  <tr> 
   <td><strong>Durata chiamata vendite</strong></td> 
   <td>Durata della chiamata in secondi.</td> 
  </tr>
  <tr> 
   <td><strong>Chiamata Di Vendita Effettuata Da</strong></td> 
   <td>Indirizzo e-mail del venditore che ha effettuato la chiamata.</td> 
  </tr>
  <tr> 
   <td><strong>URL registrazione chiamata vendita</strong></td> 
   <td>URL della registrazione della chiamata.</td> 
  </tr>
  <tr> 
   <td><strong>Stato della chiamata di vendita</strong></td> 
   <td>Salva lo stato della chiamata finale, che include: completato, nessuna risposta, annullato, non riuscito.</td> 
  </tr>
  <tr> 
   <td><strong>Oggetto della chiamata di vendita</strong></td> 
   <td>Chiama il risultato selezionato da un utente di vendita nel dialer.</td> 
  </tr>
  <tr> 
   <td><strong>ID campagna di vendita</strong></td> 
   <td>ID univoco per la risorsa della campagna di vendita in Sales Connect.</td> 
  </tr>
  <tr> 
   <td><strong>Nome della campagna di vendita</strong></td> 
   <td>Nome della campagna di vendita.</td> 
  </tr>
  <tr> 
   <td><strong>URL della campagna di vendita</strong></td> 
   <td>URL di connessione alle vendite per la campagna di vendita.</td> 
  </tr>
  <tr> 
   <td><strong>Oggetto e-mail vendite</strong></td> 
   <td>Oggetto dell'e-mail.</td> 
  </tr>
  <tr> 
   <td><strong>Numero di telefono di vendita chiamato</strong></td> 
   <td>Numero di telefono chiamato dalle vendite.</td> 
  </tr>
  <tr> 
   <td><strong>Nome del modello di vendita</strong></td> 
   <td>Nome del modello e-mail in Sales Connect.</td> 
  </tr>
  <tr> 
   <td><strong>URL del modello di vendita</strong></td> 
   <td>URL di connessione alle vendite per il modello e-mail.</td> 
  </tr>
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
 </tbody> 
</table>
