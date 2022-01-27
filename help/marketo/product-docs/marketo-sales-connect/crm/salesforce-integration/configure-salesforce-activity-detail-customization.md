---
description: Configurare la personalizzazione dei dettagli dell’attività Salesforce - Documenti Marketo - Documentazione del prodotto
title: Configurare la personalizzazione dei dettagli dell’attività Salesforce
hide: true
hidefromtoc: true
exl-id: 4b20ca29-18d6-4026-9bf9-77656ad1442d
source-git-commit: 8574a4373ec778b6127905bb3f5057153bec88a5
workflow-type: tm+mt
source-wordcount: '614'
ht-degree: 0%

---

# Configurare la personalizzazione dei dettagli dell’attività Salesforce {#configure-salesforce-activity-detail-customization}

>[!PREREQUISITES]
>
>* Salesforce e Marketo Sales Connect [deve essere collegato](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/connect-your-sales-connect-account-to-salesforce.md)
>* Registrazione di attività e-mail tramite API [deve essere abilitato](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/salesforce-sync-settings.md)


La personalizzazione dei dettagli dell&#39;attività consente agli amministratori di configurare le informazioni che verranno registrate nel campo Attività Salesforce - Oggetto, quando un&#39;attività/attività promemoria di Sales Connect viene sincronizzata in Salesforce.

![](assets/configure-salesforce-activity-detail-customization-1.png)

![](assets/configure-salesforce-activity-detail-customization-2.png)

<table>
 <tr>
  <td><strong>1</td>
  <td>Attività Promemoria InMail</td>
 </tr>
 <tr>
  <td><strong>2</td>
  <td>Attività e-mail</td>
 </tr>
 <tr>
  <td><strong>3</td>
  <td>Attività di chiamata</td>
 </tr>
</table>

La funzione può essere utilizzata per sbloccare i seguenti vantaggi:

* Personalizzando le informazioni visibili sul campo dell&#39;oggetto, i dettagli dell&#39;attività possono essere facilmente scannerizzati per le vendite in Salesforce.
* Gli amministratori possono assegnare un tag al campo oggetto con un identificatore univoco, ad esempio &quot;Mkto_sales&quot;, in modo che le attività di Sales Connect possano essere facilmente identificate e differenziate da altre attività e-mail, attività di chiamata e attività.
* Riduci la necessità di campi di attività personalizzati. Salesforce impone dei limiti al numero di campi di attività personalizzati, che possono limitare i dati disponibili da utilizzare nei rapporti. Utilizzando i campi dinamici dell’attività per aggiungere dati chiave alla riga dell’oggetto, puoi ridurre il numero di campi di attività personalizzati da creare nell’istanza Salesforce.
* Il campo oggetto delle attività e delle attività seguirà un pattern coerente definito dall’amministratore di Sales Connect.

## Campi dinamici dell’attività supportati {#activity-dynamic-fields-supported}

I campi dinamici dell’attività fanno riferimento a informazioni sulle attività di vendita per popolare i dati. Oggi, possono essere utilizzati con Personalizzazione dei dettagli dell&#39;attività Salesforce.

>[!NOTE]
>
>Se non è presente alcun valore per compilare il campo dinamico per un’attività o un’attività specifica, non verrà compilato alcun dato per quel campo dinamico quando il campo Attività Salesforce - Oggetto viene aggiornato.

<table>
 <tr>
  <th>Campo</th>
  <th>Descrizione</th>
 </tr>
 <tr>
  <td>{{activity_type}}</td>
  <td>Compilerà il tipo di attività come E-mail, Chiamata, InMail o Personalizzato.</td>
 </tr>
 <tr>
  <td>{{activity_subject}}</td>
  <td><p>Compilerà l'oggetto dell'attività.</p>
      <p>Nel caso di un’e-mail, compila la riga dell’oggetto dell’e-mail.</p>
      <p>In caso di chiamata, inMail o personalizzata, verrà compilato un valore se è stata creata un'attività promemoria con un valore nel campo nome/oggetto dell'attività.</p></td>
 </tr>
 <tr>
  <td>{{sales_campaign_name}}</td>
  <td>Se l'attività è stata avviata da una campagna di vendita, verrà compilato il nome della campagna di vendita.</td>
 </tr>
 <tr>
  <td>{{sales_campaign_day}}</td>
  <td>Se l'attività è stata avviata da una campagna di vendita, verrà compilato il numero del giorno della campagna di vendita in cui si è verificata questa attività.</td>
 </tr>
 <tr>
  <td>{{sales_campaign_step}}</td>
  <td>Se l'attività è stata avviata da una campagna di vendita, il numero di passaggio verrà compilato entro il giorno della campagna di vendita in cui si è verificata questa attività.</td>
 </tr>
 <tr>
  <td>{{call_result}}</td>
  <td>Se l’attività è una chiamata e è selezionato un risultato della chiamata, questo popolerà il valore del risultato della chiamata.</td>
 </tr>
 <tr>
  <td>{{call_reason}}</td>
  <td>Se l’attività è una chiamata e è selezionato un motivo di chiamata, verrà popolato il valore del motivo della chiamata.</td>
 </tr>
</table>

## Configurazione della personalizzazione dei dettagli dell’attività Salesforce {#configuring-salesforce-activity-detail-customization}

>[!NOTE]
>
>**Autorizzazioni di amministrazione richieste.**

Durante la configurazione dei dettagli dell’attività, considera quali dati sarebbero più rilevanti per le vendite durante la revisione della cronologia delle attività in Salesforce.

1. Fai clic sull’icona a forma di ingranaggio e seleziona **Impostazioni**.

   ![](assets/configure-salesforce-activity-detail-customization-3.png)

1. Fai clic su **Salesforce**.

   ![](assets/configure-salesforce-activity-detail-customization-4.png)

1. Fai clic su **Impostazioni di sincronizzazione**.

   ![](assets/configure-salesforce-activity-detail-customization-5.png)

1. Nell’editor di personalizzazione dei dettagli dell’attività, aggiungi eventuale testo libero desiderato. Il testo aggiunto non è dinamico e rimarrà invariato per il campo oggetto di tutte le attività sincronizzate con Salesforce.

   ![](assets/configure-salesforce-activity-detail-customization-6.png)

   >[!TIP]
   >
   >Anche se non obbligatorio, il wrapping di testo aggiunto tra parentesi graffe può facilitare la discernimento tra i dati quando vengono compilati in un campo oggetto in Salesforce. Esempio: `[Sales Connect] - {{Activity_type}}`

1. Aggiungi eventuali campi dinamici aggiuntivi desiderati facendo clic sul pulsante **Aggiungi campo dinamico** pulsante .

   ![](assets/configure-salesforce-activity-detail-customization-7.png)

1. Seleziona i campi dinamici desiderati.

   ![](assets/configure-salesforce-activity-detail-customization-8.png)

1. Fai clic su **Salva**.

   ![](assets/configure-salesforce-activity-detail-customization-9.png)

>[!NOTE]
>
>Salesforce applica un limite di 255 caratteri. Se i dettagli dell’attività superano tale limite, verranno troncati per assicurarsi che le informazioni vengano memorizzate nel campo oggetto Salesforce.

>[!MORELIKETHIS]
>
>* [Impostazioni di sincronizzazione](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/salesforce-sync-settings.md)
>* [Sincronizzazione attività promemoria con Salesforce](/help/marketo/product-docs/marketo-sales-connect/tasks/reminder-task-sync-with-salesforce.md)
>* [Personalizzazione di Sales Connect per CRM](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/sales-connect-customizations-for-crm.md)

