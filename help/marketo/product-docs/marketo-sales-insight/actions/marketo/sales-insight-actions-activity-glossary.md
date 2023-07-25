---
description: Glossario delle attività di approfondimento sulle vendite - Documenti Marketo - Documentazione del prodotto
title: Glossario delle attività Analisi vendite
exl-id: fd0f632c-6f0d-49f9-a805-0730595c81fd
feature: Sales Insight Actions
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 2%

---

# Glossario delle attività Analisi vendite {#sales-insight-actions-activity-glossary}

In Azioni approfondimento vendite, quando un venditore: aggiunge un lead a una campagna di vendita, invia un’e-mail di vendita o effettua una chiamata di vendita in uscita, verrà registrato nella cronologia delle attività di Marketo per quel lead. Inoltre, quando il lead si impegna con e-mail, si apre, fa clic e risponde, viene registrato anche.

Le attività seguenti verranno registrate in Marketo da Sales Insight Actions.

>[!NOTE]
>
>Queste attività e attributi sono disponibili per essere utilizzati dall’API REST e Bulk.

## Attività {#activities}

<table>
 <tr>
  <th>Attività di vendita</th>
  <th>Attributo</th>
 </tr>
 <tr>
  <th rowspan="9">Invia e-mail vendite</th>
  <td>Inviato da</td>
 </tr>
 <tr>
  <td>Origine</td>
 </tr>
 <tr>
  <td>ID Modello</td>
 </tr>
 <tr>
  <td>URL modello vendite</td>
 </tr>
 <tr>
  <td>URL campagna di vendita</td>
 </tr>
 <tr>
  <td>Nome modello di vendita</td>
 </tr>
 <tr>
  <td>Oggetto e-mail</td>
 </tr>
 <tr>
  <td>Nome campagna di vendita</td>
 </tr>
 <tr>
  <td>ID persona di vendita Marketo</td>
 </tr>
 <tr>
  <th rowspan="9">Apri e-mail vendite</th>
  <td>Inviato da</td>
 </tr>
 <tr>
  <td>Origine</td>
 </tr>
 <tr>
  <td>ID Modello</td>
 </tr>
 <tr>
  <td>URL modello vendite</td>
 </tr>
 <tr>
  <td>URL campagna di vendita</td>
 </tr>
 <tr>
  <td>Nome modello di vendita</td>
 </tr>
 <tr>
  <td>Oggetto e-mail</td>
 </tr>
 <tr>
  <td>Nome campagna di vendita</td>
 </tr>
 <tr>
  <td>ID persona di vendita Marketo</td>
 </tr>
 <tr>
  <th rowspan="10">E-mail vendita selezionata</th>
  <td>Collegamento</td>
 </tr>
 <tr>
  <td>Inviato da</td>
 </tr>
 <tr>
  <td>Origine</td>
 </tr>
 <tr>
  <td>ID Modello</td>
 </tr>
 <tr>
  <td>URL modello vendite</td>
 </tr>
 <tr>
  <td>URL campagna di vendita</td>
 </tr>
 <tr>
  <td>Nome modello di vendita</td>
 </tr>
 <tr>
  <td>Oggetto e-mail</td>
 </tr>
 <tr>
  <td>Nome campagna di vendita</td>
 </tr>
 <tr>
  <td>ID persona di vendita Marketo</td>
 </tr>
<tr>
  <th rowspan="3">Risposta all'e-mail di vendita</th>
  <td>Ricevuto da</td>
 </tr>
 <tr>
  <td>Origine</td>
 </tr>
 <tr>
  <td>ID persona di vendita Marketo</td>
 </tr>
 <tr>
  <th rowspan="11">Chiamata di vendita ricevuta</th>
  <td>Chiamata di vendita effettuata da</td>
 </tr>
 <tr>
  <td>Stato della chiamata di vendita</td>
 </tr>
 <tr>
  <td>Oggetto della chiamata di vendita</td>
 </tr>
 <tr>
  <td>Nome campagna di vendita</td>
 </tr>
 <tr>
  <td>URL campagna di vendita</td>
 </tr>
 <tr>
  <td>Numero di telefono vendita chiamato</td>
 </tr>
 <tr>
  <td>Origine</td>
 </tr>
 <tr>
  <td>Durata della chiamata di vendita</td>
 </tr>
 <tr>
  <td>URL registrazione chiamata di vendita</td>
 </tr>
  <tr>
  <td>Chiamata di vendita ricevuta da</td>
 </tr>
 <tr>
  <td>ID persona di vendita Marketo</td>
 </tr>
 <tr>
  <th rowspan="6">Aggiungi a campagna di vendita</th>
  <td>Nome campagna di vendita</td>
 </tr>
 <tr>
  <td>Stato della chiamata di vendita</td>
 </tr>
 <tr>
  <td>URL campagna di vendita</td>
 </tr>
 <tr>
  <td>Inviato da</td>
 </tr>
 <tr>
  <td>Origine</td>
 </tr>
 <tr>
  <td>ID campagna di vendita</td>
 </tr>
 <tr>
  <th rowspan="6">Rimuovi da campagna di vendita</th>
  <td>Nome campagna di vendita</td>
 </tr>
 <tr>
  <td>Stato della chiamata di vendita</td>
 </tr>
 <tr>
  <td>URL campagna di vendita</td>
 </tr>
 <tr>
  <td>Inviato da</td>
 </tr>
 <tr>
  <td>Origine</td>
 </tr>
 <tr>
  <td>ID campagna di vendita</td>
 </tr>
 <tr>
  <th rowspan="5">E-mail di vendita non recapitate</th>
  <td>Dettagli</td>
 </tr>
 <tr>
  <td>E-mail</td>
 </tr>
 <tr>
  <td>Inviato da</td>
 </tr>
 <tr>
  <td>ID persona di vendita Marketo</td>
 </tr>
 <tr>
  <td>ID Modello</td>
 </tr>
</table>

## Descrizione {#descriptions}

<table> 
 <tr>
  <th>Attributo</th>
  <th>Descrizione</th>
 </tr>
 <tbody> 
 <tr> 
   <td><strong>Dettagli</strong></td> 
   <td>Dettagli del messaggio di errore di mancato recapito.</td> 
  </tr> 
  <tr> 
   <td><strong>E-mail</strong></td> 
   <td>Indirizzo e-mail non recapitato.</td> 
  </tr> 
  <tr> 
   <td><strong>Collegamento</strong></td> 
   <td>URL su cui è stato fatto clic.</td> 
  </tr> 
  <tr> 
   <td><strong>ID persona di vendita Marketo</strong></td> 
   <td>ID univoco per il record della persona nelle azioni di approfondimento sulle vendite.</td> 
  </tr> 
  <tr> 
   <td><strong>Ricevuto da</strong></td> 
   <td>Indirizzo e-mail della persona che ha inviato l’e-mail.</td> 
  </tr>
  <tr> 
   <td><strong>Chiamata di vendita ricevuta da</strong></td> 
   <td>Nome della persona che ha risposto alla chiamata.</td> 
  </tr>
  <tr> 
   <td><strong>Durata della chiamata di vendita</strong></td> 
   <td>Durata della chiamata in secondi.</td> 
  </tr>
  <tr> 
   <td><strong>Chiamata di vendita effettuata da</strong></td> 
   <td>Indirizzo e-mail del venditore che ha effettuato la chiamata.</td> 
  </tr>
  <tr> 
   <td><strong>URL registrazione chiamata di vendita</strong></td> 
   <td>URL della registrazione delle chiamate.</td> 
  </tr>
  <tr> 
   <td><strong>Stato della chiamata di vendita</strong></td> 
   <td>Salva lo stato finale della chiamata, che include: completato, nessuna risposta, annullato, non riuscito.</td> 
  </tr>
  <tr> 
   <td><strong>Oggetto della chiamata di vendita</strong></td> 
   <td>Risultato della chiamata selezionato da un utente di vendita nella composizione.</td> 
  </tr>
  <tr> 
   <td><strong>ID campagna di vendita</strong></td> 
   <td>ID univoco della risorsa della campagna di vendita nelle azioni di approfondimento sulle vendite.</td> 
  </tr>
  <tr> 
   <td><strong>Nome campagna di vendita</strong></td> 
   <td>Nome della campagna di vendita.</td> 
  </tr>
  <tr> 
   <td><strong>URL campagna di vendita</strong></td> 
   <td>URL azioni approfondimento vendite per campagna di vendita.</td> 
  </tr>
  <tr> 
   <td><strong>Oggetto e-mail vendita</strong></td> 
   <td>Riga dell'oggetto dell'e-mail seguita da un ID univoco (ad es., Oggetto (SIA-12345678)</td> 
  </tr>
  <tr> 
   <td><strong>Numero di telefono vendita chiamato</strong></td> 
   <td>Numero di telefono chiamato dalle vendite.</td> 
  </tr>
  <tr> 
   <td><strong>Nome modello di vendita</strong></td> 
   <td>Nome del modello e-mail in Azioni approfondimento vendite.</td> 
  </tr>
  <tr> 
   <td><strong>URL modello vendite</strong></td> 
   <td>URL azioni approfondimento vendite per modello e-mail.</td> 
  </tr>
  <tr> 
   <td><strong>Inviato da</strong></td>
   <td>Indirizzo e-mail della persona che ha inviato l’e-mail.</td> 
  </tr> 
  <tr> 
   <td><strong>Origine</strong></td> 
   <td>Origine dell’attività. Verrà impostato come "Tout" per le attività di approfondimento sulle vendite precedenti alla versione di ottobre 2021. Sarà "App di vendita" per le attività di approfondimento sulle vendite dopo la versione di ottobre 2021.</td>
  </tr> 
  <tr> 
   <td><strong>ID Modello</strong></td> 
   <td>Quando l’origine è Tout, l’ID modello sarà l’ID modello Marketo Sales Insight Actions. Usare questa opzione per eseguire il targeting di un modello specifico invece della riga dell'oggetto, che potrebbe esistere in più modelli.
</td> 
  </tr> 
 </tbody> 
</table>
