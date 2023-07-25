---
description: Sincronizzazione dei messaggi chiave di chiamata e chiamata - Documenti Marketo - Documentazione del prodotto
title: Sincronizzazione dei messaggi chiave di chiamata e chiamata
exl-id: a8df5b77-e594-4e06-8194-1758a3582cda
feature: Veeva CRM
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '503'
ht-degree: 2%

---

# Sincronizzazione dei messaggi chiave di chiamata e chiamata {#syncing-call-and-call-key-messages}

Gli oggetti messaggio chiave di chiamata e chiamata in Veeva CRM vengono sincronizzati per impostazione predefinita nel Marketo Engage. Marketo sincronizza i dati che risalgono a un massimo di 6 mesi fa, in base alla data di creazione della chiamata.

>[!NOTE]
>
>Marketo conserva i dati della chiamata fino a sei mesi dalla data della chiamata.

**Quali sono i trigger/filtri relativi alla chiamata e al messaggio chiave di chiamata?**

Trigger:

* Aggiunto alla chiamata
* Rimosso dalla chiamata
* Aggiunto al messaggio della chiave di chiamata
* Rimosso dal messaggio chiave di chiamata
* Chiamata aggiornata
* Messaggio Chiave Chiamata Aggiornato

Filtri:

* Ha una chiamata
* Ha un messaggio di chiave di chiamata

I seguenti campi nei messaggi Chiave chiamata e Chiave chiamata sono sincronizzati e possono essere utilizzati come vincoli e attivatori.

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
      <td>Contabile</td>
      <td>Ricercare l’account a cui è associata la chiamata.</td>
      <td>Account_vod__c</td>
      <td>Ricerca (account)</td>
    </tr>
    <tr>
      <td>Chiamata</td>
      <td>Tipo di chiamata</td>
      <td>Tipo di chiamata gestito dal sistema in base al tipo e al contenuto della chiamata. Questo campo viene utilizzato a scopo di reporting. I valori validi sono: Solo dettaglio, Dettaglio con campione, Dettaglio gruppo, Dettaglio gruppo con campione, Solo campione. Questi valori non devono essere modificati, ma le traduzioni per questi elenchi a discesa possono essere modificate. I partecipanti hanno lo stesso tipo di chiamata della chiamata di intestazione. Per una chiamata di gruppo con 3 professionisti, tutti e 4 i record hanno il tipo di chiamata "Dettagli gruppo"</td>
      <td>Tipo_chiamata_vod__c</td>
      <td>Elenco a discesa</td>
    </tr>
    <tr>
     <td>Chiamata</td>
      <td>Contatto</td>
      <td>Ricercare il contatto (se presente) a cui è associata la chiamata.</td>
      <td>Contact_vod__c</td>
      <td>Lookup(Contact)</td>
    </tr>
    <tr>
      <td>Chiamata</td>
      <td>Data</td>
      <td>Data della chiamata in cui è stata salvata o inviata per la prima volta. Questo campo viene impostato tramite un trigger alla data corrente se non viene fornito né il campo data né il campo data e ora.</td>
      <td>Data_chiamata__c</td>
      <td>Data</td>
    </tr>
    <tr>
      <td>Chiamata</td>
      <td>È Una Chiamata Genitore?</td>
      <td>Campo formula per determinare se il record Chiamata è il record Chiamata padre o Chiamata partecipante. 1 indica che il record è la chiamata padre. 0 indica che si tratta di una chiamata Partecipante.</td>
      <td>Is_Parent_Call_vod__c</td>
      <td>Formula (numero)</td>
    </tr>
    <tr>
      <td>Chiamata</td>
      <td>Stato</td>
      <td>Stato della chiamata: Pianificato, Salvato o Inviato. Utilizza il workbench di traduzione per modificare i valori di visualizzazione. I trigger durante la chiamata esaminano questo campo per verificare se la chiamata è bloccata (inviata). Questo valore viene impostato per l’utente quando viene premuto il pulsante Salva o Invia.</td>
      <td>Status_vod__c</td>
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
      <td>Chiama messaggio chiave</td>
      <td>Chiamata</td>
      <td>Ricerca nella chiamata. Ogni messaggio chiave è associato a una chiamata.</td>
      <td>Chiama2_vod__c</td>
      <td>Master-Detail(Call)</td>
    </tr>
    <tr>
      <td>Chiama messaggio chiave</td>
      <td>Categoria</td>
      <td>Registra la categoria del messaggio. Utilizzato principalmente per il reporting.</td>
      <td>Categoria_vod__c</td>
      <td>Elenco a discesa</td>
    </tr>
    <tr>
      <td>Chiama messaggio chiave</td>
      <td>Nome presentazione CLM</td>
      <td>Nome presentazione CLM con timbro</td>
      <td>Clm_Presentation_Name_vod__c</td>
      <td>Testo (80)</td>
    </tr>
    <tr>
      <td>Chiama messaggio chiave</td>
      <td>Nome messaggio chiave</td>
      <td>Nome messaggio chiave timbrata</td>
      <td>Nome_messaggio_chiave_vod__c</td>
      <td>Testo (80)</td>
    </tr>
    <tr>
      <td>Chiama messaggio chiave</td>
      <td>Nome prodotto</td>
      <td> </td>
      <td>Product_Name__c</td>
      <td>Formula (testo)</td>
    </tr>
    <tr>
      <td>Chiama messaggio chiave</td>
      <td>Reazione</a>
      </td>
      <td>Elenco a discesa delle reazioni al messaggio. Modificate l'elenco a discesa per modificare i valori di reazione.</td>
      <td>Reaction_vod__c</td>
      <td>Elenco a discesa</td>
    </tr>
  </tbody>
</table>
