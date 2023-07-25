---
unique-page-id: 4719294
description: Personalizzare la sincronizzazione delle attività - Documentazione di Marketo - Documentazione del prodotto
title: Personalizza sincronizzazione attività
exl-id: 938d83dc-b9b1-41d8-bf98-04548b074ec4
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 0%

---

# Personalizza sincronizzazione attività {#customize-activities-sync}

Se non utilizzi Marketo Sales Insight, Marketo può creare record di cronologia attività Salesforce per determinati eventi. Ecco come abilitarli.

1. Vai a **Amministratore**.

   ![](assets/admin.png)

1. Clic **Salesforce**, quindi fai clic su **Modifica opzioni di sincronizzazione**.

   ![](assets/two-1.png)

1. Seleziona le caselle accanto alle attività che desideri che Marketo invii a Salesforce e fai clic su **Salva**.

   ![](assets/three-1.png)

   >[!NOTE]
   >
   >Una volta abilitato, Marketo invierà tre mesi di cronologia delle attività. A seconda della quantità di dati, _il completamento di questa operazione potrebbe richiedere alcuni giorni_. Gli aggiornamenti che si verificano durante il push iniziale delle attività possono essere ritardati fino al completamento della sincronizzazione iniziale delle attività.

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
   <td><p>Passaggio di flusso: aggiunto a un elenco statico</p></td> 
  </tr> 
  <tr> 
   <td>E-mail inviata</td> 
   <td>Passaggio di flusso: è stata inviata un’e-mail</td> 
  </tr> 
  <tr> 
   <td>E-mail consegnata</td> 
   <td>Ricevuto un messaggio e-mail (non inviato)</td> 
  </tr> 
  <tr> 
   <td>E-mail aperta</td> 
   <td>Aperta un’e-mail (senza bloccare le immagini)</td> 
  </tr> 
  <tr> 
   <td>Collegamento selezionato nell’e-mail</td> 
   <td>Clic su un collegamento in un messaggio e-mail inviato da Marketo</td> 
  </tr> 
  <tr> 
   <td>Rimosso dall’elenco</td> 
   <td>Passaggio di flusso: rimosso da un elenco statico</td> 
  </tr> 
  <tr> 
   <td>Rimuovi dal flusso</td> 
   <td>Passaggio di flusso: Rimuovi dal flusso</td> 
  </tr> 
  <tr> 
   <td>E-mail di vendita inviata</td> 
   <td>È stato inviato un messaggio e-mail tramite Marketo Sales Insight</td> 
  </tr> 
  <tr> 
   <td>E-mail di vendita aperta</td> 
   <td>Apertura di un'e-mail inviata tramite Marketo Sales Insight</td> 
  </tr> 
  <tr> 
   <td>Fai clic sul collegamento nell’e-mail di vendita</td> 
   <td>Clic su un collegamento in un'e-mail inviata tramite Marketo Sales Insight</td> 
  </tr> 
  <tr> 
   <td>E-mail di vendita ricevuta</td> 
   <td>Un messaggio e-mail è stato ricevuto e registrato dal rappresentante commerciale nel plug-in di Outlook MSI</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>&quot;E-mail di vendita ricevuta&quot; non **non** media consegnata. Lo stato di consegna non viene acquisito per le e-mail inviate tramite Sales Insight.

>[!TIP]
>
>Per maggiori informazioni su Marketo in Salesforce, consulta la sezione [Insight sulla vendita di Marketo](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md) prodotto.
