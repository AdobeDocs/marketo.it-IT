---
unique-page-id: 4719294
description: Personalizza sincronizzazione attività - Documenti Marketo - Documentazione prodotto
title: Personalizza sincronizzazione attività
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%

---


# Personalizza sincronizzazione attività {#customize-activities-sync}

Se non utilizzi [Sales Insight](http://docs.marketo.com/display/DOCS/Marketo+Sales+Insight), Marketo può creare i record Cronologia attività Salesforce per alcuni eventi. Ecco come attivarli.

1. Vai a **Admin. **

   ![](assets/admin.png)

1. Fate clic su **Salesforce**, quindi fate clic su **Modifica opzioni** sincronizzazione.

   ![](assets/two-1.png)

1. Selezionare le caselle accanto alle attività che si desidera inviare a Salesforce da Marketo e fare clic su **Salva**.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >Una volta attivato, Marketo invierà la cronologia delle attività per tre mesi. A seconda della quantità di dati, *questo potrebbe richiedere diversi giorni per il completamento*. Gli aggiornamenti che si verificano durante il push delle attività iniziali potrebbero essere posticipati fino al completamento della sincronizzazione iniziale delle attività.

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
   <td>Modulo compilato</td> 
   <td>Compilato qualsiasi modulo Marketo</td> 
  </tr> 
  <tr> 
   <td>Aggiunto all'elenco</td> 
   <td><p>Passaggio flusso: È stato aggiunto a un elenco statico</p></td> 
  </tr> 
  <tr> 
   <td>E-mail inviata</td> 
   <td>Passaggio flusso: È stato inviato un messaggio e-mail</td> 
  </tr> 
  <tr> 
   <td>E-mail consegnata</td> 
   <td>Ricevuto un messaggio e-mail (non rimbalzato)</td> 
  </tr> 
  <tr> 
   <td>E-mail aperta</td> 
   <td>È stato aperto un messaggio e-mail (senza bloccare le immagini)</td> 
  </tr> 
  <tr> 
   <td>Collegamento selezionato nell’e-mail</td> 
   <td>Clic su un collegamento in un messaggio e-mail inviato da Marketo</td> 
  </tr> 
  <tr> 
   <td>Rimosso dall'elenco</td> 
   <td>Passaggio flusso: È stato rimosso da un elenco statico</td> 
  </tr> 
  <tr> 
   <td>Rimuovi dal flusso</td> 
   <td>Passaggio flusso: Rimuovi dal flusso</td> 
  </tr> 
  <tr> 
   <td>E-mail di vendita inviata</td> 
   <td>È stato inviato un messaggio e-mail tramite Marketing Sales Insight</td> 
  </tr> 
  <tr> 
   <td>Messaggio e-mail di vendita aperto</td> 
   <td>È stato aperto un messaggio e-mail inviato tramite Marketing Sales Insight</td> 
  </tr> 
  <tr> 
   <td>Fate clic sul collegamento nel messaggio e-mail di vendita</td> 
   <td>Fai clic su un collegamento in un messaggio e-mail inviato tramite Marketing Sales Insight</td> 
  </tr> 
  <tr> 
   <td>E-mail di vendita ricevuta</td> 
   <td>Un messaggio e-mail è stato ricevuto e registrato dal rappresentante delle vendite nel plug-in MSI Outlook</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>**Promemoria**
>
>
>&quot;E-mail di vendita ricevuta&quot; **non** significa consegnata. Lo stato consegnato non viene acquisito per le e-mail inviate tramite Sales Insight.

>[!TIP]
>
>Per maggiori informazioni su Marketo in Salesforce, consulta il nostro prodotto [Marketing Sales Insight](../../../../../product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md) .

