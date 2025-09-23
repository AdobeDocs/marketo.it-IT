---
description: Glossario delle attività di vendita - Documentazione di Marketo - Documentazione del prodotto
title: Glossario dell’attività di vendita
exl-id: c7805642-07b6-4697-9efe-5c673ae9ca53
feature: Marketo Sales Connect
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 8%

---

# Glossario dell’attività di vendita {#sales-activity-glossary}

In Sales Connect, quando un venditore: aggiunge un lead a una cadenza di vendita, invia un’e-mail o effettua una chiamata a un’attività, verrà registrato nella cronologia delle attività di Marketo. Inoltre, quando il lead si relaziona con le e-mail, vengono registrati anche le aperture, i clic e le risposte.

Le attività seguenti verranno registrate in Marketo da [!DNL Sales Connect].

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
  <td>[!UICONTROL Sent By]</td>
 </tr>
 <tr>
  <td>Origine</td>
 </tr>
 <tr>
  <td>[!UICONTROL Template ID]</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Template] URL</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Campaign] URL</td>
 </tr>
 <tr>
  <td>[!UICONTROL Sales Template] Nome</td>
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
  <th rowspan="9"> Apri e-mail vendite</th>
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
  <th rowspan="10">E-mail vendita selezionata</th>
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
  <th rowspan="3">Risposta all'e-mail di vendita</th>
  <td>[!UICONTROL Received By]</td>
 </tr>
 <tr>
  <td>Origine</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Person ID]</td>
 </tr>
 <tr>
  <th rowspan="11">Chiamata di vendita ricevuta</th>
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
  <th rowspan="6">Aggiungi a campagna di vendita</th>
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
  <th rowspan="6">Rimuovi da campagna di vendita</th>
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
   <td>ID univoco del record persona in [!DNL Sales Connect].</td>
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
   <td>ID univoco della risorsa della campagna di vendita in [!DNL Sales Connect].</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sales Campaign Name]</strong></td>
   <td>Nome della campagna di vendita.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sales Campaign URL]</strong></td>
   <td>[!DNL Sales Connect] URL per campagna di vendita.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sales Email Subject]</strong></td>
   <td>Riga dell’oggetto dell’e-mail seguita da un ID univoco (ad esempio, Oggetto (MSC-12345678)</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sales Phone Number Called]</strong></td>
   <td>Numero di telefono chiamato dalle vendite.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sales Template Name]</strong></td>
   <td>Nome del modello e-mail in [!DNL Sales Connect].</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sales Template URL]</strong></td>
   <td>[!DNL Sales Connect] URL per modello e-mail.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Sent By]</strong></td>
   <td>Indirizzo e-mail della persona che ha inviato l’e-mail.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Source]</strong></td>
   <td>Source dell’attività. Verrà impostato come "Tout" per le attività [!DNL Sales Connect] precedenti alla versione di ottobre 2021. Sarà "App di vendita" per le attività [!DNL Sales Connect] dopo la versione di ottobre 2021.</td>
  </tr>
  <tr>
   <td><strong>[!UICONTROL Template ID]</strong></td>
   <td>Quando l'origine è Tout, l'ID modello sarà l'ID modello [!DNL Marketo Sales Connect]. Usare questa opzione per eseguire il targeting di un modello specifico invece della riga dell'oggetto, che potrebbe esistere in più modelli.
</td>
  </tr>
 </tbody>
</table>
