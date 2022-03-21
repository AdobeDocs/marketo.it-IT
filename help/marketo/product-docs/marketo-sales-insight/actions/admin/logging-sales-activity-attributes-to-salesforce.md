---
description: Registrazione degli attributi delle attività di vendita su Salesforce - Documenti Marketo - Documentazione del prodotto
title: Registrazione degli attributi delle attività di vendita a Salesforce
exl-id: fdefe53b-eb99-48ce-a04e-3666be33fea4
source-git-commit: f2f81167066c2f170f81308b2deec52d19efafb3
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 1%

---

# Registrazione degli attributi delle attività di vendita a Salesforce {#logging-sales-activity-attributes-to-salesforce}

L’amministratore Salesforce può aggiungere manualmente campi di attività personalizzati a Salesforce.

1. Nel tuo account Salesforce, fai clic su **Configurazione**.

1. Cerca &quot;Campi personalizzati attività&quot; nel campo di ricerca rapida e fai clic su di esso.

1. Fai clic su **Nuovo**.

1. Seleziona Tipo di dati corrispondente al campo da aggiungere in base alla tabella seguente e fai clic su **Successivo**.

1. Immetti il nome del campo e l’etichetta corrispondenti al campo da aggiungere.

Descrizione di ciascuna colonna della tabella seguente:

* **Etichetta campo**: Nome del campo visualizzato nell’interfaccia utente (questo nome può essere personalizzato per migliorare la leggibilità da parte del team)
* **Nome campo**: Nome tecnico del campo (assicurati che il Nome campo immesso corrisponda al Nome campo nella tabella seguente)
* **Nome API**: Nome tecnico del campo API (assicurati che il nome API immesso corrisponda al nome API nella tabella seguente)
* **Tipo di dati**: Tipo di campo
* **Dimensione**: Dimensioni del campo di testo

<table>
 <tr>
  <th>Etichetta campo</th>
  <th>Nome campo</th>
  <th>Nome API</th>
  <th>Tipo di dati</th>
  <th>Dimensione</th>
 </tr>
 <tr>
  <td>ID presenza locale chiamata vendita Marketo</td>
  <td>MSE_Call_Local_Presence_ID</td>
  <td>MSE_Call_Local_Presence_ID_c</td>
  <td>Testo</td>
  <td>255</td>
 </tr>
 <tr>
  <td>URL di registrazione della chiamata di vendita Marketo</td>
  <td>MSE_Call_Recording</td>
  <td>MSE_Call_Recording_c</td>
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
  <td>MSE_Current_Campaign_Step_c</td>
  <td>Testo</td>
  <td>255</td>
 </tr>
 <tr>
  <td>URL della campagna di vendita Marketo</td>
  <td>MSE_Campaign_Details_Link</td>
  <td>MSE_Campaign_Details_Link_c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>Allegato e-mail di vendita Marketo visualizzato</td>
  <td>MSE_Presentation_Viewed</td>
  <td>MSE_Presentation_Viewed_c</td>
  <td>Casella di controllo</td>
  <td></td>
 </tr>
 <tr>
  <td>E-mail di vendita Marketo selezionata</td>
  <td>MSE_Clic</td>
  <td>MSE_Clic_c</td>
  <td>Casella di controllo</td>
  <td></td>
 </tr>
 <tr>
  <td>Risposte e-mail di vendita Marketo</td>
  <td>MSE_Risposta</td>
  <td>MSE_Replied_c</td>
  <td>Casella di controllo</td>
  <td></td>
 </tr>
 <tr>
  <td>Stato e-mail vendite Marketo</td>
  <td>MSE_Email_Status</td>
  <td>MSE_Email_Status__c</td>
  <td>Testo</td>
  <td></td>
 </tr>
 <tr>
  <td>Modello e-mail vendite Marketo</td>
  <td>MSE_Template</td>
  <td>MSE_Template_c</td>
  <td>Testo</td>
  <td>255</td>
 </tr>
 <tr>
  <td>URL modello e-mail vendita Marketo</td>
  <td>MSE_Template_Details</td>
  <td>MSE_Template_Details_c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>URL e-mail vendita Marketo</td>
  <td>MSE_Details</td>
  <td>MSE_Details_c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>E-mail di vendita Marketo visualizzata</td>
  <td>MSE_Visualizzato</td>
  <td>MSE_Viewed_c</td>
  <td>Casella di controllo</td>
  <td></td>
 </tr>
</table>
