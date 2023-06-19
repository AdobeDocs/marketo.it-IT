---
description: Configurare la personalizzazione dei dettagli delle attività di Salesforce - Documenti Marketo - Documentazione del prodotto
title: Configura personalizzazione dettagli attività Salesforce
exl-id: 4b20ca29-18d6-4026-9bf9-77656ad1442d
source-git-commit: 02354356949aef7aa8836d4753ec538b7819a65a
workflow-type: tm+mt
source-wordcount: '707'
ht-degree: 0%

---

# Configura personalizzazione dettagli attività Salesforce {#configure-salesforce-activity-detail-customization}

>[!PREREQUISITES]
>
>* Salesforce e Marketo Sales Connect [deve essere connesso](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/connect-your-sales-connect-account-to-salesforce.md)
>* Registrazione dell’attività e-mail tramite API [deve essere abilitato](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/salesforce-sync-settings.md)

Personalizzazione dettagli attività consente agli amministratori di configurare le informazioni che accederanno al campo Oggetto dell&#39;attività Salesforce quando un&#39;attività/promemoria Sales Connect viene sincronizzato con Salesforce.

>[!NOTE]
>
>* Gli aggiornamenti apportati al campo dell&#39;oggetto in Sales Connect di un&#39;attività promemoria si rifletteranno nel campo dell&#39;oggetto dell&#39;attività Salesforce corrispondente, se si utilizza `{{activity_subject}}` dinamico nella personalizzazione dei dettagli dell’attività.
>* Le interruzioni di riga non sono supportate quando si registrano informazioni nel campo dell’oggetto Salesforce. Eventuali interruzioni di riga nell&#39;editor personalizzazione dettagli attività verranno rimosse quando si aggiorna un oggetto attività di vendita.

![](assets/configure-salesforce-activity-detail-customization-1.png)

![](assets/configure-salesforce-activity-detail-customization-2.png)

<table>
 <tr>
  <td><strong>1</td>
  <td>Attività promemoria InMail</td>
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

La funzione può essere utilizzata per usufruire dei seguenti vantaggi:

* Personalizzando le informazioni visibili sul campo dell’oggetto, i dettagli dell’attività possono essere facilmente analizzati per le vendite in Salesforce.
* Gli amministratori possono assegnare un tag al campo dell’oggetto con un identificatore univoco, ad esempio &quot;Mkto_sales&quot;, in modo che le attività di Sales Connect possano essere facilmente identificate e differenziate da altre attività e-mail, attività di chiamata e attività.
* Riduci la necessità di campi di attività personalizzati. Salesforce impone limiti al numero di campi di attività personalizzati, che possono limitare i dati disponibili per l’utilizzo nei rapporti. Utilizzando i campi dinamici dell’attività per aggiungere dati chiave alla riga dell’oggetto, puoi ridurre il numero di campi attività personalizzati da creare nell’istanza Salesforce.
* Il campo dell&#39;oggetto delle attività e delle attività seguirà un modello coerente definito dall&#39;amministratore Sales Connect.

>[!NOTE]
>
>Se registri le risposte e-mail come attività in Salesforce, non utilizzeranno le impostazioni di Personalizzazione dei dettagli delle attività di Salesforce. Invece, registrerà come &quot;Reply: Email Subject&quot; (Risposta: Oggetto dell’e-mail).

## Campi dinamici attività supportati {#activity-dynamic-fields-supported}

I campi dinamici delle attività contengono informazioni di riferimento sulle attività di vendita per compilare i dati. Oggi possono essere utilizzati con la Personalizzazione dei dettagli delle attività di Salesforce.

>[!NOTE]
>
>Se non è presente alcun valore per compilare il campo dinamico per un&#39;attività/attività specifica, quando il campo Attività - Oggetto Salesforce viene aggiornato non verranno inseriti dati per tale campo dinamico.

<table>
 <tr>
  <th>Campo</th>
  <th>Descrizione</th>
 </tr>
 <tr>
  <td>{{activity_type}}</td>
  <td>Popola il tipo di attività come E-mail, Chiamata, InMail o Personalizzato.</td>
 </tr>
 <tr>
  <td>{{activity_subject}}</td>
  <td><p>Compilerà l'oggetto dell'attività.</p>
      <p>Nel caso di un’e-mail, verrà compilata la riga dell’oggetto dell’e-mail.</p>
      <p>In caso di chiamata, inMail o personalizzata, verrà compilato un valore se è stata creata un'attività promemoria con un valore nel campo nome attività/oggetto.</p></td>
 </tr>
 <tr>
  <td>{{sales_campaign_name}}</td>
  <td>Se l’attività è stata avviata da una campagna di vendita, popolerà il nome della campagna di vendita.</td>
 </tr>
 <tr>
  <td>{{sales_campaign_day}}</td>
  <td>Se l'attività è stata avviata da una campagna di vendita, verrà compilato il numero del giorno della campagna di vendita in cui si è verificata l'attività.</td>
 </tr>
 <tr>
  <td>{{sales_campaign_step}}</td>
  <td>Se l'attività è stata avviata da una campagna di vendita, popolerà il numero della fase entro il giorno della campagna di vendita in cui si è verificata l'attività.</td>
 </tr>
 <tr>
  <td>{{call_outcome}}</td>
  <td>Se l’attività è una chiamata e viene selezionato un risultato della chiamata, questo popolerà il valore del risultato della chiamata.</td>
 </tr>
 <tr>
  <td>{{call_reason}}</td>
  <td>Se l’attività è una chiamata e viene selezionato un motivo di chiamata, questo popolerà il valore del motivo della chiamata.</td>
 </tr>
</table>

## Configurazione della personalizzazione dei dettagli dell’attività Salesforce {#configuring-salesforce-activity-detail-customization}

>[!NOTE]
>
>**Autorizzazioni di amministrazione richieste.**

Quando configuri i dettagli dell’attività, considera quali dati sarebbero più rilevanti per le vendite quando esamini la cronologia delle attività in Salesforce.

1. Fai clic sull’icona a forma di ingranaggio e seleziona **Impostazioni**.

   ![](assets/configure-salesforce-activity-detail-customization-3.png)

1. Clic **Salesforce**.

   ![](assets/configure-salesforce-activity-detail-customization-4.png)

1. Clic **Impostazioni di sincronizzazione**.

   ![](assets/configure-salesforce-activity-detail-customization-5.png)

1. Nell’editor di personalizzazione dei dettagli dell’attività aggiungi eventuale testo libero. Il testo aggiunto non è dinamico e rimarrà invariato per il campo dell&#39;oggetto di tutte le attività sincronizzate con Salesforce.

   ![](assets/configure-salesforce-activity-detail-customization-6.png)

   >[!TIP]
   >
   >Anche se non obbligatorio, racchiudere il testo aggiunto tra parentesi quadre può facilitare la distinzione tra i dati quando vengono inseriti in un campo dell’oggetto in Salesforce. Esempio: `[Sales Connect] - {{Activity_type}}`

1. Aggiungi eventuali campi dinamici aggiuntivi facendo clic sul pulsante **Aggiungi campo dinamico** pulsante.

   ![](assets/configure-salesforce-activity-detail-customization-7.png)

1. Seleziona i campi dinamici desiderati.

   ![](assets/configure-salesforce-activity-detail-customization-8.png)

1. Clic **Salva**.

   ![](assets/configure-salesforce-activity-detail-customization-9.png)

>[!NOTE]
>
>Salesforce applica un limite di 255 caratteri. Se i dettagli dell’attività superano questo limite, verranno troncati per garantire che le informazioni vengano memorizzate nel campo dell’oggetto Salesforce.

>[!MORELIKETHIS]
>
>* [Impostazioni di sincronizzazione](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-integration/salesforce-sync-settings.md)
>* [Sincronizzazione attività promemoria con Salesforce](/help/marketo/product-docs/marketo-sales-connect/tasks/reminder-task-sync-with-salesforce.md)
>* [Personalizzazione di Sales Connect per CRM](/help/marketo/product-docs/marketo-sales-connect/crm/salesforce-customization/sales-connect-customizations-for-crm.md)
