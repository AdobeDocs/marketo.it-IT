---
unique-page-id: 4719294
description: Personalizzare la sincronizzazione delle attività - Documentazione di Marketo - Documentazione del prodotto
title: Personalizza sincronizzazione attività
exl-id: 938d83dc-b9b1-41d8-bf98-04548b074ec4
feature: Salesforce Integration
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 1%

---

# Personalizza sincronizzazione attività {#customize-activities-sync}

Se non si utilizza Marketo Sales Insight, Marketo Engage può creare record della cronologia attività di Salesforce per determinati eventi. Ecco come abilitarli.

>[!NOTE]
>
>La sincronizzazione Salesforce/Marketo Engage non invierà a Salesforce alcuna attività che si è verificata prima del push della persona a Salesforce.

1. Vai a **[!UICONTROL Admin]**.

   ![](assets/customize-activities-sync-1.png)

1. Fai clic su **[!DNL Salesforce]**, quindi su **[!UICONTROL Edit Sync Options]**.

   ![](assets/two-1.png)

1. Selezionare le caselle accanto alle attività che si desidera inviare da Marketo a Salesforce e fare clic su **[!UICONTROL Save]**.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >Una volta abilitato, Marketo invierà tre mesi di cronologia delle attività. A seconda della quantità di dati, _il completamento potrebbe richiedere alcuni giorni_. Gli aggiornamenti che si verificano durante il push iniziale delle attività possono essere ritardati fino al completamento della sincronizzazione iniziale delle attività.

<table> 
 <colgroup> 
  <col> 
  <col> 
 </colgroup> 
 <thead> 
  <tr> 
   <th>Tipo di attività</th> 
   <th>Descrizione</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Filled out form]</td> 
   <td>Compilato qualsiasi modulo Marketo</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Added to list]</td> 
   <td><p>Passaggio di flusso: aggiunto a un elenco statico</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Email sent]</td> 
   <td>Passaggio di flusso: è stata inviata un’e-mail</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Email delivered]</td> 
   <td>Ricevuto un messaggio e-mail (non inviato)</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Email opened]</td> 
   <td>Aperta un’e-mail (senza bloccare le immagini)</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Clicked link in email]</td> 
   <td>Clic su un collegamento in un messaggio e-mail inviato da Marketo</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Removed from list]</td> 
   <td>Passaggio di flusso: rimosso da un elenco statico</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Remove from flow]</td> 
   <td>Passaggio di flusso: Rimuovi dal flusso</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sales email sent]</td> 
   <td>È stato inviato un messaggio e-mail tramite Marketo Sales Insight</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sales email opened]</td> 
   <td>Apertura di un'e-mail inviata tramite Marketo Sales Insight</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Click link in sales email]</td> 
   <td>Clic su un collegamento in un’e-mail inviata tramite Marketo Sales Insight</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sales email received]</td> 
   <td>Un messaggio e-mail è stato ricevuto e registrato dal rappresentante commerciale nel plug-in di Outlook MSI</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>&quot;E-mail di vendita ricevuta&quot; significa _non_ recapitata. Lo stato di consegna non viene acquisito per le e-mail inviate tramite Sales Insight.

>[!TIP]
>
>Se sei interessato a ottenere ulteriori informazioni su Marketo in Salesforce, consulta il nostro prodotto [Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}.
