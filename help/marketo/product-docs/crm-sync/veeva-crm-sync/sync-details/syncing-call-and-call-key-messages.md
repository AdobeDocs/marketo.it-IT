---
description: Messaggi chiave di chiamata e chiamata di sincronizzazione - Documenti Marketo - Documentazione del prodotto
title: Sincronizzazione dei messaggi chiave di chiamata e chiamata
exl-id: a8df5b77-e594-4e06-8194-1758a3582cda
source-git-commit: bb020cba0bb0cb65761e15cba05147b6e9fffe50
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 0%

---

# Sincronizzazione dei messaggi chiave di chiamata e chiamata {#syncing-call-and-call-key-messages}

Gli oggetti del messaggio chiave di chiamata e chiamata in Veeva CRM sono sincronizzati per impostazione predefinita in Marketo Engage. Marketo sincronizza i dati con un massimo di 6 mesi, in base alla data di creazione della chiamata.

>[!NOTE]
>
>Marketo conserva i dati delle chiamate fino a sei mesi dalla data della chiamata.

**Quali sono i trigger/filtri correlati al messaggio chiave di chiamata e chiamata?**

Triggers:

* Aggiunto alla chiamata
* Rimosso dalla chiamata
* Aggiunto al messaggio chiave della chiamata
* Rimosso dal messaggio chiave della chiamata
* Chiamata aggiornata
* Messaggio chiave di chiamata aggiornato

Filtri:

* Chiamata
* Con messaggio chiave della chiamata

I campi seguenti nei messaggi di chiamata e chiave di chiamata sono sincronizzati e possono essere utilizzati come vincoli e attivatori.

<table>
  <colgroup>
    <col>
    <col>
    <col>
    <col>
    <col>
  </colgroup>
  <thead>
    <tr>
      <th>
        Oggetto
      </th>
      <th>
        Etichetta campo
      </th>
      <th>
        Descrizione
      </th>
      <th>
        Nome campo
      </th>
      <th>
        Tipo di dati
      </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Chiamata</td>
      <td>Ragioniere</td>
      <td>Cerca l’account a cui è associata la chiamata .</td>
      <td>Account_vod_c</td>
      <td>Ricerca (account)</td>
    </tr>
    <tr>
      <td>Chiamata</td>
      <td>Tipo di chiamata</td>
      <td>Tipo di chiamata gestito dal sistema in base al tipo e al contenuto della chiamata. Questo campo viene utilizzato a scopo di reporting. I valori validi sono: Solo dettaglio, Dettaglio con campione, Dettagli gruppo, Dettagli gruppo con campione, Solo campione. Questi valori non devono essere modificati, ma le traduzioni per queste liste di selezione possono essere modificate. I partecipanti hanno lo stesso tipo di chiamata della chiamata di intestazione. Per una chiamata di Gruppo con 3 professionisti, tutti e 4 i record hanno il tipo di chiamata "Dettagli di gruppo"</td>
      <td>Call_Type_vod_c</td>
      <td>Elenco a discesa</td>
    </tr>
    <tr>
     <td>Chiamata</td>
      <td>Contatto</td>
      <td>Ricercare l’eventuale contatto a cui è associata la chiamata .</td>
      <td>Contact_vod_c</td>
      <td>Ricerca (contatto)</td>
    </tr>
    <tr>
      <td>Chiamata</td>
      <td>Data</td>
      <td>Data della chiamata al primo salvataggio o invio. Questo campo viene impostato tramite un trigger alla data corrente se non viene fornito né il campo data né il campo data/ora.</td>
      <td>Call_Date_vod_c</td>
      <td>Data</td>
    </tr>
    <tr>
      <td>Chiamata</td>
      <td>È La Chiamata Genitore?</td>
      <td>Campo formula per determinare se il record Chiamata è il record Chiamata padre o Chiamata partecipante. 1 indica che il record è la chiamata padre. 0 indica che si tratta di una chiamata partecipante.</td>
      <td>Is_Parent_Call_vod_c</td>
      <td>Formula (numero)</td>
    </tr>
    <tr>
      <td>Chiamata</td>
      <td>Stato</td>
      <td>Stato della chiamata: Pianificato, Salvato o Inviato. Utilizza il workbench di traduzione per modificare i valori di visualizzazione. Gli attivatori durante la chiamata guardano questo campo per vedere se la chiamata è bloccata (inviata). Questo valore viene impostato per l’utente quando si preme il pulsante Salva o Invia.</td>
      <td>Status_vod_c</td>
      <td>Elenco a discesa</td>
    </tr>
    <tr>
      <td>Chiamata</td>
      <td>Tipo di record</td>
      <td> </td>
      <td>RecordTypeId</td>
      <td>Tipo di record</td>
    </tr>
    <tr>
      <td>Messaggio chiave della chiamata</td>
      <td>Chiamata</td>
      <td>Cerca nella chiamata . Ogni messaggio chiave è associato a una chiamata .</td>
      <td>Call2_vod_c</td>
      <td>Master-Detail(Call)</td>
    </tr>
    <tr>
      <td>Messaggio chiave della chiamata</td>
      <td>Categoria</td>
      <td>Registra la categoria del messaggio. Utilizzato principalmente per il reporting.</td>
      <td>Category_vod_c</td>
      <td>Elenco a discesa</td>
    </tr>
    <tr>
      <td>Messaggio chiave della chiamata</td>
      <td>Nome presentazione CLM</td>
      <td>Nome della presentazione CLM con timbro</td>
      <td>Clm_Presentation_Name_vod_c</td>
      <td>Testo (80)</td>
    </tr>
    <tr>
      <td>Messaggio chiave della chiamata</td>
      <td>Nome del messaggio chiave</td>
      <td>Nome del messaggio della chiave con timbro</td>
      <td>Key_Message_Name_vod_c</td>
      <td>Testo (80)</td>
    </tr>
    <tr>
      <td>Messaggio chiave della chiamata</td>
      <td>Nome del prodotto</td>
      <td> </td>
      <td>Nome_Prodotto__c</td>
      <td>Formula (testo)</td>
    </tr>
    <tr>
      <td>Messaggio chiave della chiamata</td>
      <td>Reazione</a>
      </td>
      <td>Elenco delle reazioni al messaggio. Modificate l’elenco di selezione per modificare i valori di reazione.</td>
      <td>Reaction_vod_c</td>
      <td>Elenco a discesa</td>
    </tr>
  </tbody>
</table>
