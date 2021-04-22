---
description: Stato di sincronizzazione Salesforce - Documenti Marketo - Documentazione del prodotto
title: Stato di sincronizzazione Salesforce
exl-id: 61197808-7812-4e0a-8ac6-4a60af0f7979
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 0%

---

# Stato di sincronizzazione Salesforce {#salesforce-sync-status}

Utilizza il dashboard Stato sincronizzazione per visualizzare le statistiche di sincronizzazione come parte dei passaggi di sincronizzazione e del relativo stato di successo.

I passaggi di sincronizzazione riflettono le operazioni di push o pull in base a ciascun tipo di oggetto per lo schema dell’oggetto e i dati stessi. Le statistiche coprono nuovi record, aggiornamenti, eliminazioni e conteggi non riusciti durante la sincronizzazione. Gli utenti possono filtrare per data, tipo di operazione o tipo di oggetto. Dashboard di stato sincronizzazione mostra lo stato dei cicli di sincronizzazione per gli ultimi cinque giorni.

>[!NOTE]
>
>Autorizzazioni amministratore richieste

## Visualizza lo stato di sincronizzazione {#view-sync-status}

1. Fai clic su **Amministratore**.

   ![](assets/salesforce-sync-status-1.png)

1. In Integrazione, fai clic su Salesforce, quindi sulla scheda Stato sincronizzazione .

   ![](assets/salesforce-sync-status-2.png)

Per impostazione predefinita, le statistiche vengono ordinate in base all’avvio più recente. Per ordinare in base a Inizia o Termina con (dal più recente al meno recente), fai clic sull’icona di ordinamento.

![](assets/salesforce-sync-status-3.png)

## Stato sincronizzazione filtro {#filter-sync-status}

1. Per filtrare i dati, fai clic sull’icona del filtro posta all’estrema destra della pagina.

   ![](assets/salesforce-sync-status-4.png)

1. Seleziona l’intervallo di date e ore, quindi fai clic sull’elenco a discesa per filtrare in base al tipo di oggetto, al tipo di operazione e/o al tipo di stato.

   ![](assets/salesforce-sync-status-5.png)

1. Fare clic su **Applica**.

   ![](assets/salesforce-sync-status-6.png)

**Passaggio** facoltativo: Per esportare gli errori di sincronizzazione, fai clic su  **Esporta**. I dati verranno esportati come CSV.

![](assets/salesforce-sync-status-7.png)

## Campi di stato di sincronizzazione {#sync-status-fields}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th>Campo</th> 
   <th>Descrizione</th> 
   <th>Valori Enum</th> 
  </tr> 
  <tr> 
   <td colspan="1">Inizia a</td> 
   <td colspan="1">Data/ora di inizio del ciclo di sincronizzazione (fuso orario dell'utente)</td> 
   <td colspan="1"></td> 
  </tr>  
  <tr> 
   <td colspan="1">Terminato a</td> 
   <td colspan="1">Data/ora di fine del ciclo di sincronizzazione (fuso orario dell’utente)</td> 
   <td colspan="1"></td> 
  </tr> 
  <tr> 
   <td colspan="1">Oggetto</td> 
   <td colspan="1">Tipo di oggetto</td> 
   <td colspan="1">Contatto, Persona, Attività, Opportunità, Lead, Altri come di seguito</td> 
  </tr>  
  <tr> 
   <td colspan="1">Funzionamento</td> 
   <td colspan="1">Tipo di operazione</td> 
   <td colspan="1">Tipi di operazioni come sotto</td> 
  </tr>  
  <tr> 
   <td colspan="1">Stato</td> 
   <td colspan="1">Stato del batch</td> 
   <td colspan="1">Riuscito, Non riuscito, Incompleto, In corso, Pulito*</td> 
  </tr>
  <tr> 
   <td colspan="1">Nuovo</td> 
   <td colspan="1">Conteggio dei nuovi record</td> 
   <td colspan="1"></td> 
  </tr>  
  <tr> 
   <td colspan="1">Aggiornato</td> 
   <td colspan="1">Conteggio dei record aggiornati</td> 
   <td colspan="1"></td> 
  </tr>  
  <tr> 
   <td colspan="1">Eliminato</td> 
   <td colspan="1">Conteggio dei record eliminati</td> 
   <td colspan="1"></td> 
  </tr> 
  <tr> 
   <td colspan="1">Elemento non riuscito</td> 
   <td colspan="1">Numero di record con sincronizzazione non riuscita</td> 
   <td colspan="1"><br></td> 
  </tr>  
  <tr> 
   <td colspan="1">Saltato</td> 
   <td colspan="1">Numero di record saltati perché non vi sono state modifiche ai campi di interesse per la sincronizzazione</td> 
   <td colspan="1"></td> 
  </tr>  
 </tbody> 
</table>

*I dati sono stati ripristinati allo stato precedente di integrità dopo un errore del passo di sincronizzazione.

## Tipo di oggetto {#object-type}

<table> 
 <colgroup> 
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <td colspan="1">Account</td> 
  </tr>  
  <tr> 
   <td colspan="1">Tipo di conto</td> 
  </tr> 
  <tr> 
   <td colspan="1">Oggetti personalizzati</td> 
  </tr>  
  <tr> 
   <td colspan="1">Campaign</td> 
  </tr>  
  <tr> 
   <td colspan="1">Stato membro campagna</td> 
  </tr>
  <tr> 
   <td colspan="1">Contatto</td> 
  </tr>  
  <tr> 
   <td colspan="1">Modello e-mail</td> 
  </tr>  
  <tr> 
   <td colspan="1">Evento</td> 
  </tr> 
  <tr> 
   <td colspan="1">Persona (lead)</td> 
  </tr>  
  <tr> 
   <td colspan="1">Opportunità</td> 
  </tr>  
  <tr> 
   <td colspan="1">Ruolo contatto opportunità</td> 
  </tr>  
  <tr> 
   <td colspan="1">Attività</td> 
  </tr>  
  <tr> 
   <td colspan="1">Utente</td> 
  </tr>  
 </tbody> 
</table>

## Tipo di operazione {#operation-type}

<table> 
 <colgroup> 
  <col> 
  <col> 
  <col>
  <col> 
 </colgroup> 
 <tbody> 
  <tr> 
   <th>Tipo di operazione</th> 
   <th>Trovato in questi oggetti</th> 
   <th>Osservazioni</th> 
   <th>Tipo di operazione</th>
  </tr> 
  <tr> 
   <td colspan="1">Collegamento Init con il programma</td> 
   <td colspan="1">Campaign</td> 
   <td colspan="1">Collegamento di campagne a programmi</td> 
   <td colspan="1">Aggiorna</td>
  </tr>  
  <tr> 
   <td colspan="1">Conversioni di pull</td> 
   <td colspan="1">Persona (lead)*</td> 
   <td colspan="1">Recupera le azioni di conversione da SFDC a Marketo. Unità (numeri): lead che si convertono in contatti</td> 
   <td colspan="1">Aggiornamento, elemento non riuscito o ignorato</td>
  </tr> 
  <tr> 
   <td colspan="1">Elimina pull</td> 
   <td colspan="1">Contatto, Persona (lead), Opportunità, Campagna, Membri campagna, Contatto opportunità, Oggetti personalizzati, Campagne, Stato membro campagna, Ruolo contatto opportunità</td> 
   <td colspan="1">Record eliminati di SFDC sincronizzati con Marketo</td> 
   <td colspan="1">Eliminato, non riuscito o ignorato</td>
  </tr>  
  <tr> 
   <td colspan="1">Aggiornamenti pull</td> 
   <td colspan="1">Attività, Persona (Lead), Coda Persona (Lead), Contatto, Evento, Opportunità, Account, Tipo di account, Membri campagna, Oggetti Personalizzati, Campagne, Stato Membro campagna, Eventi, Stato Persona, Opportunità, Ruolo Contatto opportunità</td> 
   <td colspan="1">Aggiornamenti o nuovi record in SFDC sincronizzati con Marketo, Recupera eventi come attività</td> 
   <td colspan="1">Nuovo, aggiornato, elemento non riuscito o ignorato</td>
  </tr>  
  <tr> 
   <td colspan="1">Invia nuovo</td> 
   <td colspan="1">Attività, modelli e-mail</td> 
   <td colspan="1">Attività push (attività)</td> 
   <td colspan="1"></td>
  </tr>
  <tr> 
   <td colspan="1">Aggiornamenti push</td> 
   <td colspan="1">Attività, Modelli E-Mail, Persona, Contatto, Campagne</td> 
   <td colspan="1">Invio di aggiornamenti a SFDC ed eliminazione</td> 
   <td colspan="1">Aggiornamento, elemento non riuscito o ignorato</td>
  </tr>  
  <tr> 
   <td colspan="1">Schema di sincronizzazione</td> 
   <td colspan="1">Membri della campagna, oggetti personalizzati, campagne, stato membro campagna, attività, persona, opportunità, ruolo contatto opportunità, utenti</td> 
   <td colspan="1">Sincronizza metadati per oggetti diversi, per decidere quali nuovi campi sincronizzare nel ciclo successivo</td> 
   <td colspan="1"></td>
  </tr>  
  <tr> 
   <td colspan="1">Sincronizza con il programma</td> 
   <td colspan="1">Campagne</td> 
   <td colspan="1">Sincronizza il programma Marketo con le campagne SFDC</td> 
   <td colspan="1">Nuovo, Aggiornamenti, Non riuscito o ignorato</td>
  </tr> 
  <tr> 
   <td colspan="1">Aggiornare le attività</td> 
   <td colspan="1">Attività</td> 
   <td colspan="1">Recupera attività da Salesforce</td> 
   <td colspan="1"></td>
  </tr>  
  <tr> 
   <td colspan="1">Aggiorna FKS</td> 
   <td colspan="1">Tutto</td> 
   <td colspan="1">Aggiorna la chiave esterna di tutti gli oggetti</td> 
   <td colspan="1">N/D</td>
  </tr>  
 </tbody> 
</table>

*La configurazione del branding a livello di abbonamento determina l&#39;etichetta: &quot;Lead&quot; o &quot;Persona&quot; nel rapporto.
