---
description: Glossario delle attività di vendita Insight Actions - Documentazione di Marketo - Documentazione del prodotto
title: Glossario attività azioni Insight vendite
exl-id: fd0f632c-6f0d-49f9-a805-0730595c81fd
feature: Sales Insight Actions
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 5%

---

# Glossario attività [!DNL Sales Insight Actions] {#sales-insight-actions-activity-glossary}

In [!DNL Sales Insight Actions], quando un venditore: aggiunge un lead a una campagna di vendita, invia un&#39;e-mail di vendita o effettua una chiamata di vendita in uscita, verrà registrato nella cronologia delle attività di Marketo per tale lead. Inoltre, quando il lead si impegna con e-mail, si apre, fa clic e risponde, viene registrato anche.

Le attività seguenti verranno registrate in Marketo da [!DNL Sales Insight Actions].

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
  <th rowspan="9">[!UICONTROL Send Sales Email]</th>
  <td>[!UICONTROL Sent By]</td>
 </tr>
 <tr>
  <td>Origine</td>
 </tr>
 <tr>
  <td>[!UICONTROL Template ID]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Template URL]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign URL]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Template Name]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Email Subject]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign Name]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Person ID]</td>
 </tr>
 <tr>
  <th rowspan="9">[!UICONTROL Open Sales Email]</th>
  <td>[!UICONTROL Sent By]</td>
 </tr>
 <tr>
  <td>Origine</td>
 </tr>
 <tr>
  <td>[!UICONTROL Template ID]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Template URL]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign URL]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Template Name]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Email Subject]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign Name]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Person ID]</td>
 </tr>
 <tr>
  <th rowspan="10">[!UICONTROL Clicked Sales Email]</th>
  <td>[!UICONTROL Link]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sent By]</td>
 </tr>
 <tr>
  <td>Origine</td>
 </tr>
 <tr>
  <td>[!UICONTROL Template ID]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Template URL]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign URL]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Template Name]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Email Subject]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign Name]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Person ID]</td>
 </tr>
<tr>
  <th rowspan="3">[!UICONTROL Replied to Sales Email]</th>
  <td>[!UICONTROL Received By]</td>
 </tr>
 <tr>
  <td>Origine</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Person ID]</td>
 </tr>
 <tr>
  <th rowspan="11">[!UICONTROL Received Sales Call]</th>
  <td>[!UICONTROL Sales Call Made By]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Call Status]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Call Subject]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign Name]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign URL]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Phone Number Called]</td>
 </tr>
 <tr>
  <td>Origine</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Call Duration]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Call Recording URL]</td>
 </tr>
  <tr>
  <td>[!UICONTROL Sales Call Answered By]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Person ID]</td>
 </tr>
 <tr>
  <th rowspan="6">[!UICONTROL Add to Sales Campaign]</th>
  <td>[!UICONTROL Sales Campaign Name]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Call Status]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign URL]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sent By]</td>
 </tr>
 <tr>
  <td>Origine</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign ID]</td>
 </tr>
 <tr>
  <th rowspan="6">[!UICONTROL Remove from Sales Campaign]</th>
  <td>[!UICONTROL Sales Campaign Name]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Call Status]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign URL]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sent By]</td>
 </tr>
 <tr>
  <td>Origine</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign ID]</td>
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
  <td>ID modello</td>
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
   <td><strong>[!UICONTROL Details]</strong></td> 
   <td>Dettagli del messaggio di errore di mancato recapito.</td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Email]</strong></td> 
   <td>Indirizzo e-mail non recapitato.</td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Link]</strong></td> 
   <td>URL su cui è stato fatto clic.</td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Marketo Sales Person ID]</strong></td> 
   <td>ID univoco del record persona in [!DNL Sales Insight Actions].</td> 
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Received By]</strong></td> 
   <td>Indirizzo e-mail della persona che ha inviato l’e-mail.</td> 
  </tr>
  <tr> 
   <td><strong>[!UICONTROL Sales Call Answered By]</strong></td> 
   <td>Nome della persona che ha risposto alla chiamata.</td> 
  </tr>
  <tr> 
   <td><strong>[!UICONTROL Sales Call Duration]</strong></td> 
   <td>Durata della chiamata in secondi.</td> 
  </tr>
  <tr> 
   <td><strong>[!UICONTROL Sales Call Made By]</strong></td> 
   <td>Indirizzo e-mail del venditore che ha effettuato la chiamata.</td> 
  </tr>
  <tr> 
   <td><strong>[!UICONTROL Sales Call Recording URL]</strong></td> 
   <td>URL della registrazione delle chiamate.</td> 
  </tr>
  <tr> 
   <td><strong>[!UICONTROL Sales Call Status]</strong></td> 
   <td>Salva lo stato finale della chiamata, che include: completato, nessuna risposta, annullato, non riuscito.</td> 
  </tr>
  <tr> 
   <td><strong>[!UICONTROL Sales Call Subject]</strong></td> 
   <td>Risultato della chiamata selezionato da un utente di vendita nella composizione.</td> 
  </tr>
  <tr> 
   <td><strong>[!UICONTROL Sales Campaign ID]</strong></td> 
   <td>ID univoco della risorsa della campagna di vendita in [!DNL Sales Insight Actions].</td> 
  </tr>
  <tr> 
   <td><strong>[!UICONTROL Sales Campaign Name]</strong></td> 
   <td>Nome della campagna di vendita.</td> 
  </tr>
  <tr> 
   <td><strong>[!UICONTROL Sales Campaign URL]</strong></td> 
   <td>[!DNL Sales Insight Actions] URL per campagna di vendita.</td> 
  </tr>
  <tr> 
   <td><strong>[!UICONTROL Sales Email Subject]</strong></td> 
   <td>Riga dell'oggetto dell'e-mail seguita da un ID univoco (ad es., Oggetto (SIA-12345678)</td> 
  </tr>
  <tr> 
   <td><strong>[!UICONTROL Sales Phone Number Called]</strong></td> 
   <td>Numero di telefono chiamato dalle vendite.</td> 
  </tr>
  <tr> 
   <td><strong>[!UICONTROL Sales Template Name]</strong></td> 
   <td>Nome del modello e-mail in [!DNL Sales Insight Actions].</td> 
  </tr>
  <tr> 
   <td><strong>[!UICONTROL Sales Template URL]</strong></td> 
   <td>[!DNL Sales Insight Actions] URL per modello e-mail.</td> 
  </tr>
  <tr> 
   <td><strong>[!UICONTROL Sent By]</strong></td>
   <td>Indirizzo e-mail della persona che ha inviato l’e-mail.</td> 
  </tr> 
  <tr> 
   <td><strong>Origine</strong></td> 
   <td>Source dell’attività. Verrà impostato come "Tout" per le attività [!DNL Sales Insight Actions] precedenti alla versione di ottobre 2021. Sarà "App di vendita" per le attività [!DNL Sales Insight Actions] dopo la versione di ottobre 2021.</td>
  </tr> 
  <tr> 
   <td><strong>[!UICONTROL Template ID]</strong></td> 
   <td>Quando l'origine è Tout, l'ID modello sarà l'ID modello [!DNL Marketo Sales Insight Actions]. Usare questa opzione per eseguire il targeting di un modello specifico invece della riga dell'oggetto, che potrebbe esistere in più modelli.
</td> 
  </tr> 
 </tbody> 
</table>
