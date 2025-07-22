---
description: Registrazione degli attributi dell'attività di vendita su Salesforce - Documentazione Marketo - Documentazione del prodotto
title: Registrazione degli attributi dell'attività di vendita in Salesforce
exl-id: fdefe53b-eb99-48ce-a04e-3666be33fea4
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 12%

---

# Registrazione attributi attività di vendita in [!DNL Salesforce] {#logging-sales-activity-attributes-to-salesforce}

L&#39;amministratore di Salesforce può aggiungere manualmente campi attività personalizzati a [!DNL Salesforce].

1. Nel tuo account [!DNL Salesforce], fai clic su **[!UICONTROL Setup]**.

1. Cerca &quot;Campi personalizzati attività&quot; nel campo di ricerca rapida e fai clic su di esso.

1. Fai clic su **[!UICONTROL New]**.

1. Selezionare il tipo di dati corrispondente al campo che si desidera aggiungere in base alla tabella seguente e fare clic su **[!UICONTROL Next]**.

1. Immettere il nome e l&#39;etichetta del campo corrispondenti al campo che si desidera aggiungere.

Descrizione di ciascuna colonna della tabella seguente:

* **Etichetta campo**: nome del campo visualizzato nell&#39;interfaccia utente (può essere personalizzato dal team per migliorarne la leggibilità)
* **Nome campo**: nome tecnico del campo (verificare che il nome del campo immesso corrisponda al nome del campo nella tabella seguente)
* **Nome API**: nome tecnico del campo per API (verificare che il nome API immesso corrisponda al nome API nella tabella seguente)
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
  <td>[!UICONTROL Call Outcomes]</td>
  <td>mktosales_call_result</td>
  <td>mktosales_call_result__c</td>
  <td>Testo</td>
  <td>50</td>
 </tr>
 <tr>
  <td>[!UICONTROL Call Reasons]</td>
  <td>mktosales_call_reason</td>
  <td>mktosales_call_reason__c</td>
  <td>Testo</td>
  <td>50</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Call Local Presence ID]</td>
  <td>MSE_Call_Local_Presence_ID</td>
  <td>ID_presenza_locale_chiamata__MSE</td>
  <td>Testo</td>
  <td>255</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Call Recording URL]</td>
  <td>MSE_Call_Recording</td>
  <td>MSE_Call_Recording__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Campaign]</td>
  <td>MSE_Campaign</td>
  <td>MSE_Campaign__c</td>
  <td>Testo</td>
  <td>255</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Campaign Current Step]</td>
  <td>MSE_Current_Campaign_Step</td>
  <td>MSE_Current_Campaign_Step__c</td>
  <td>Testo</td>
  <td>255</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Campaign URL]</td>
  <td>MSE_Campaign_Details_Link</td>
  <td>MSE_Campaign_Details_Link__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Email Attachment Viewed]</td>
  <td>MSE_Presentation_Viewed</td>
  <td>MSE_Presentation_Viewed__c</td>
  <td>Casella di controllo</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Email Clicked]</td>
  <td>MSE_Clicked</td>
  <td>MSE_Clicked__c</td>
  <td>Casella di controllo</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Email Replied]</td>
  <td>MSE_Risposta</td>
  <td>MSE_Risposta__c</td>
  <td>Casella di controllo</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Email Status]</td>
  <td>MSE_Email_Status</td>
  <td>MSE_Email_Status__c</td>
  <td>Testo</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Email Template]</td>
  <td>MSE_Template</td>
  <td>MSE_Template__c</td>
  <td>Testo</td>
  <td>255</td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Email Template URL]</td>
  <td>MSE_Template_Details</td>
  <td>MSE_Template_Details__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Email URL]</td>
  <td>MSE_Details</td>
  <td>MSE_Details__c</td>
  <td>URL</td>
  <td></td>
 </tr>
 <tr>
  <td>[!UICONTROL Marketo Sales Email Viewed]</td>
  <td>MSE_Visualizzato</td>
  <td>MSE_Visualizzato__c</td>
  <td>Casella di controllo</td>
  <td></td>
 </tr>
</table>
