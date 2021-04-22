---
unique-page-id: 4719294
description: Personalizzare la sincronizzazione delle attività - Documenti Marketo - Documentazione del prodotto
title: Personalizzare la sincronizzazione delle attività
exl-id: 938d83dc-b9b1-41d8-bf98-04548b074ec4
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 0%

---

# Personalizzare la sincronizzazione delle attività {#customize-activities-sync}

Se non utilizzi Marketo Sales Insight, Marketo può creare i record della cronologia delle attività di Salesforce per alcuni eventi. Ecco come attivarli.

1. Vai a **Amministratore**.

   ![](assets/admin.png)

1. Fai clic su **Salesforce**, quindi fai clic su **Modifica opzioni di sincronizzazione**.

   ![](assets/two-1.png)

1. Seleziona le caselle accanto alle attività che desideri vengano inviate a Salesforce da Marketo e fai clic su **Salva**.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >Una volta attivato, Marketo invierà una cronologia delle attività per tre mesi. A seconda della quantità di dati, _questo potrebbe richiedere diversi giorni per il completamento_. Gli aggiornamenti che si verificano durante il push delle attività iniziali possono essere ritardati fino al completamento della sincronizzazione iniziale delle attività.

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
   <td>Compilazione di qualsiasi modulo Marketo</td> 
  </tr> 
  <tr> 
   <td>Aggiunto all’elenco</td> 
   <td><p>Passaggio del flusso: È stato aggiunto a un elenco statico</p></td> 
  </tr> 
  <tr> 
   <td>E-mail inviata</td> 
   <td>Passaggio del flusso: È stato inviato un messaggio e-mail</td> 
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
   <td>Rimosso dall’elenco</td> 
   <td>Passaggio del flusso: È stato rimosso da un elenco statico</td> 
  </tr> 
  <tr> 
   <td>Rimuovi dal flusso</td> 
   <td>Passaggio del flusso: Rimuovi dal flusso</td> 
  </tr> 
  <tr> 
   <td>Messaggio e-mail di vendita inviato</td> 
   <td>È stato inviato un messaggio e-mail tramite Marketo Sales Insight</td> 
  </tr> 
  <tr> 
   <td>Messaggio e-mail di vendita aperto</td> 
   <td>È stata aperta un’e-mail inviata tramite Marketo Sales Insight</td> 
  </tr> 
  <tr> 
   <td>Fai clic sul collegamento nell'e-mail di vendita</td> 
   <td>Clic su un collegamento in un messaggio e-mail inviato tramite Marketo Sales Insight</td> 
  </tr> 
  <tr> 
   <td>E-mail di vendita ricevuta</td> 
   <td>Un messaggio e-mail è stato ricevuto e registrato dal rappresentante vendite nel plugin MSI Outlook</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>&quot;E-mail di vendita ricevuta&quot; indica **non** consegnata. Lo stato di consegna non viene acquisito per le e-mail inviate tramite Sales Insight.

>[!TIP]
>
>Per maggiori informazioni su Marketo in Salesforce, consulta il nostro prodotto [Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md) .
