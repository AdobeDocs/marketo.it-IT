---
description: Glossario delle attività di analisi delle vendite - Documenti Marketo - Documentazione del prodotto
title: Glossario delle attività di Sales Insight
exl-id: fd0f632c-6f0d-49f9-a805-0730595c81fd
source-git-commit: d9b8b92ac5f051178b8eb9b450c4949b56d50b99
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 2%

---

# Glossario delle attività di Sales Insight {#sales-insight-actions-activity-glossary}

In azioni di Insight sulle vendite, quando un venditore: aggiunge un lead a una campagna di vendita, invia loro un messaggio e-mail di vendita o effettua una chiamata di vendita in uscita, verrà registrato nella cronologia delle attività di Marketo per quel lead. Inoltre, quando il lead si occupa di e-mail, aperture, clic e risposte, viene registrato.

Le attività seguenti saranno registrate in Marketo da Sales Insight Actions.

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
  <th rowspan="3">Risposta all'e-mail di vendita</th>
  <td>Ricevuto da</td>
 </tr>
 <tr>
  <td>Fonte</td>
 </tr>
 <tr>
  <td>ID persona di vendita Marketo</td>
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
  <td>ID persona di vendita Marketo</td>
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
   <td><strong>ID persona di vendita Marketo</strong></td> 
   <td>ID univoco per il record della persona nelle azioni Approfondimenti vendite.</td> 
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
   <td>ID univoco per la risorsa della campagna di vendita nelle azioni Approfondimenti vendite.</td> 
  </tr>
  <tr> 
   <td><strong>Nome della campagna di vendita</strong></td> 
   <td>Nome della campagna di vendita.</td> 
  </tr>
  <tr> 
   <td><strong>URL della campagna di vendita</strong></td> 
   <td>URL delle azioni Approfondimenti vendite per la campagna di vendita.</td> 
  </tr>
  <tr> 
   <td><strong>Oggetto e-mail vendite</strong></td> 
   <td>Oggetto dell’e-mail seguito da un ID univoco (ad esempio: Linea oggetto (SIA-12345678)</td> 
  </tr>
  <tr> 
   <td><strong>Numero di telefono di vendita chiamato</strong></td> 
   <td>Numero di telefono chiamato dalle vendite.</td> 
  </tr>
  <tr> 
   <td><strong>Nome del modello di vendita</strong></td> 
   <td>Nome del modello e-mail in Azioni Approfondimenti vendite.</td> 
  </tr>
  <tr> 
   <td><strong>URL del modello di vendita</strong></td> 
   <td>URL delle azioni Approfondimenti vendite per il modello e-mail.</td> 
  </tr>
  <tr> 
   <td><strong>Inviato da</strong></td>
   <td>Indirizzo e-mail della persona che ha inviato l’e-mail.</td> 
  </tr> 
  <tr> 
   <td><strong>Fonte</strong></td> 
   <td>Origine dell’attività. Sarà impostato come "Tout" per le attività di Sales Insight prima del rilascio del 21 ottobre. Sarà "App di vendita" per le attività Approfondimenti vendite dopo il rilascio del 21 ottobre.</td>
  </tr> 
  <tr> 
   <td><strong>ID modello</strong></td> 
   <td>Quando l’origine è Tout, l’ID modello sarà l’ID modello per le azioni Marketo Sales Insight. Utilizza questa opzione per eseguire il targeting di un modello specifico invece della riga dell’oggetto, che potrebbe essere presente in più modelli.
</td> 
  </tr> 
 </tbody> 
</table>
