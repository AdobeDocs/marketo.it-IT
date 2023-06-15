---
description: Registrazione degli attributi dell'attività di vendita in Salesforce - Documenti Marketo - Documentazione del prodotto
title: Registrazione degli attributi dell'attività di vendita in Salesforce
exl-id: fdefe53b-eb99-48ce-a04e-3666be33fea4
source-git-commit: 544dfc0892016223c1e5976bd8c9d108ade7c984
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 5%

---

# Registrazione degli attributi dell&#39;attività di vendita in Salesforce {#logging-sales-activity-attributes-to-salesforce}

L’amministratore di Salesforce può aggiungere manualmente campi di attività personalizzati a Salesforce.

1. Nel tuo account Salesforce, fai clic su **Configurazione**.

1. Cerca &quot;Campi personalizzati attività&quot; nel campo di ricerca rapida e fai clic su di esso.

1. Clic **Nuovo**.

1. Seleziona il Tipo di dati corrispondente al campo da aggiungere in base alla tabella seguente e fai clic su **Successivo**.

1. Immettere il nome e l&#39;etichetta del campo corrispondenti al campo che si desidera aggiungere.

Descrizione di ciascuna colonna della tabella seguente:

* **Etichetta campo**: nome del campo visualizzato nell’interfaccia utente (può essere personalizzato dal team per migliorarne la leggibilità)
* **Nome campo**: nome tecnico del campo (assicurati che il nome del campo immesso corrisponda al nome del campo nella tabella seguente)
* **Nome API**: nome tecnico del campo per API (assicurati che il nome API immesso corrisponda al nome API nella tabella seguente)
* **Tipo di dati**: tipo di campo
* **Dimensione**: dimensione del campo di testo

<table>
 <tr>
  <th>Etichetta campo</th>
  <th>Nome campo</th>
  <th>Nome API</th>
  <th>Tipo di dati</th>
  <th>Dimensione</th>
 </tr>
  <tr>
  <td>Risultati della chiamata</td>
  <td>mktosales_call_result</td>
  <td>mktosales_call_result__c</td>
  <td>Testo</td>
  <td>50</td>
 </tr>
 <tr>
  <td>Motivi della chiamata</td>
  <td>mktosales_call_reason</td>
  <td>mktosales_call_reason__c</td>
  <td>Testo</td>
  <td>50</td>
 </tr>
 <tr>
  <td>ID presenza locale per chiamata di vendita Marketo</td>
  <td>MSE_Call_Local_Presence_ID</td>
  <td>ID_presenza_locale_chiamata__MSE</td>
  <td>Testo</td>
  <td>255</td>
 </tr>
 <tr>
  <td>URL di registrazione di Marketo Sales Call</td>
  <td>MSE_Call_Recording</td>
  <td>MSE_Call_Recording__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>Campagna di vendita Marketo</td>
  <td>MSE_Campaign</td>
  <td>MSE_Campaign__c</td>
  <td>Testo</td>
  <td>255</td>
 </tr>
 <tr>
  <td>Passaggio corrente della campagna di vendita Marketo</td>
  <td>MSE_Current_Campaign_Step</td>
  <td>MSE_Current_Campaign_Step__c</td>
  <td>Testo</td>
  <td>255</td>
 </tr>
 <tr>
  <td>URL campagna di vendita Marketo</td>
  <td>MSE_Campaign_Details_Link</td>
  <td>MSE_Campaign_Details_Link__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>Allegato e-mail vendita Marketo visualizzato</td>
  <td>MSE_Presentation_Viewed</td>
  <td>MSE_Presentation_Viewed__c</td>
  <td>Casella di controllo</td>
  <td></td>
 </tr>
 <tr>
  <td>E-mail vendita Marketo selezionata</td>
  <td>MSE_Clicked</td>
  <td>MSE_Clicked__c</td>
  <td>Casella di controllo</td>
  <td></td>
 </tr>
 <tr>
  <td>E-mail Marketo Sales - Risposta</td>
  <td>MSE_Risposta</td>
  <td>MSE_Risposta__c</td>
  <td>Casella di controllo</td>
  <td></td>
 </tr>
 <tr>
  <td>Stato e-mail vendita Marketo</td>
  <td>MSE_Email_Status</td>
  <td>MSE_Email_Status__c</td>
  <td>Testo</td>
  <td></td>
 </tr>
 <tr>
  <td>Modello e-mail vendite Marketo</td>
  <td>MSE_Template</td>
  <td>MSE_Template__c</td>
  <td>Testo</td>
  <td>255</td>
 </tr>
 <tr>
  <td>URL modello e-mail vendita Marketo</td>
  <td>MSE_Template_Details</td>
  <td>MSE_Template_Details__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>URL e-mail vendita Marketo</td>
  <td>MSE_Details</td>
  <td>MSE_Details__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>E-mail vendita Marketo visualizzata</td>
  <td>MSE_Visualizzato</td>
  <td>MSE_Visualizzato__c</td>
  <td>Casella di controllo</td>
  <td></td>
 </tr>
</table>
