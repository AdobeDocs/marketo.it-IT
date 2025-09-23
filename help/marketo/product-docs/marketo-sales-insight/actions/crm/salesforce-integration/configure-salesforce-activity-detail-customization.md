---
description: Configurare la personalizzazione dei dettagli delle attività di Salesforce - Documentazione di Marketo - Documentazione del prodotto
title: Configurare la personalizzazione dei dettagli delle attività di Salesforce
exl-id: 534ebdb5-7a5b-48eb-98f7-2d05a9eae8e8
feature: Sales Insight Actions
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 2%

---

# Configura personalizzazione dettagli attività [!DNL Salesforce] {#configure-salesforce-activity-detail-customization}

>[!PREREQUISITES]
>
>* Le azioni Salesforce e Sales Insight [ devono essere connesse](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/connect-your-sales-insight-actions-account-to-salesforce.md)
>* La registrazione dell&#39;attività e-mail tramite API [ deve essere abilitata](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md)

Personalizzazione dettagli attività consente agli amministratori di configurare le informazioni che accederanno al campo Oggetto dell&#39;attività [!DNL Salesforce] quando un&#39;attività di attività/promemoria [!DNL Sales Insight Actions] viene sincronizzata in [!DNL Salesforce].

>[!NOTE]
>
>* Gli aggiornamenti apportati al campo dell&#39;oggetto in [!DNL Sales Insight Actions] di un&#39;attività promemoria verranno rispecchiati nel campo dell&#39;oggetto dell&#39;attività [!DNL Salesforce] corrispondente, se si utilizza il campo dinamico `{{activity_subject}}` nella personalizzazione dei dettagli attività.
>* Le interruzioni di riga non sono supportate quando si registrano informazioni nel campo dell&#39;oggetto [!DNL Salesforce]. Eventuali interruzioni di riga nell&#39;editor personalizzazione dettagli attività verranno rimosse quando si aggiorna un oggetto attività di vendita.

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

* Personalizzando le informazioni visibili nel campo dell’oggetto, i dettagli dell’attività possono essere facilmente analizzati per le vendite in Salesforce.
* Gli amministratori possono assegnare un tag al campo dell’oggetto con un identificatore univoco, ad esempio &quot;Mkto_sales&quot;, in modo che le attività delle azioni di Insight per le vendite possano essere facilmente identificate e differenziate dalle altre attività e-mail, attività di chiamata e attività.
* Riduci la necessità di campi di attività personalizzati. Salesforce impone limiti al numero di campi di attività personalizzati, che possono limitare i dati disponibili per l’utilizzo nei rapporti. Utilizzando i campi dinamici dell’attività per aggiungere dati chiave alla riga dell’oggetto, puoi ridurre il numero di campi attività personalizzati da creare nell’istanza di Salesforce.
* Il campo dell&#39;oggetto delle attività e delle attività seguirà un modello coerente definito dall&#39;amministratore delle azioni di Sales Insight.

>[!NOTE]
>
>Se si registrano le risposte e-mail come attività in [!DNL Salesforce], non verranno utilizzate le impostazioni di personalizzazione dei dettagli attività di [!DNL Salesforce]. Invece, registrerà come &quot;Reply: Email Subject&quot; (Risposta: Oggetto dell’e-mail).

## Campi dinamici attività supportati {#activity-dynamic-fields-supported}

I campi dinamici delle attività contengono informazioni di riferimento sulle attività di vendita per compilare i dati. Oggi possono essere utilizzati con la personalizzazione dei dettagli di attività [!DNL Salesforce].

>[!NOTE]
>
>Se non è disponibile alcun valore per compilare il campo dinamico per un&#39;attività o un&#39;attività specifica, quando il campo Attività - Oggetto di Salesforce viene aggiornato non verranno inseriti dati per tale campo dinamico.

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

## Configurazione della personalizzazione dei dettagli dell&#39;attività [!DNL Salesforce] {#configuring-salesforce-activity-detail-customization}

>[!NOTE]
>
>**Autorizzazioni amministratore richieste.**

Quando configuri i dettagli dell&#39;attività, considera quali dati sarebbero più rilevanti per le vendite quando esamini la cronologia delle attività in [!DNL Salesforce].

1. Fare clic sull&#39;icona ingranaggio e selezionare **[!UICONTROL Settings]**.

   ![](assets/configure-salesforce-activity-detail-customization-3.png)

1. Fai clic su **[!UICONTROL Salesforce]**.

   ![](assets/configure-salesforce-activity-detail-customization-4.png)

1. Fai clic su **[!UICONTROL Sync Settings]**.

   ![](assets/configure-salesforce-activity-detail-customization-5.png)

1. Nell’editor di personalizzazione dei dettagli dell’attività aggiungi eventuale testo libero. Il testo aggiunto non è dinamico e rimarrà invariato per il campo dell&#39;oggetto di tutte le attività sincronizzate con [!DNL Salesforce].

   ![](assets/configure-salesforce-activity-detail-customization-6.png)

   >[!TIP]
   >
   >Anche se non obbligatorio, la disposizione del testo aggiunto tra parentesi quadre può facilitare la distinzione tra i dati quando vengono inseriti in un campo dell&#39;oggetto in [!DNL Salesforce]. Esempio: `[Sales Insight Actions] - {{Activity_type}}`

1. Per aggiungere altri campi dinamici, fare clic sul pulsante **[!UICONTROL Add Dynamic Field]**.

   ![](assets/configure-salesforce-activity-detail-customization-7.png)

1. Seleziona i campi dinamici desiderati.

   ![](assets/configure-salesforce-activity-detail-customization-8.png)

1. Fai clic su **[!UICONTROL Save]**.

   ![](assets/configure-salesforce-activity-detail-customization-9.png)

>[!NOTE]
>
>[!DNL Salesforce] applica un limite di 255 caratteri. Se i dettagli dell&#39;attività superano questo limite, verranno troncati per garantire che le informazioni vengano memorizzate nel campo dell&#39;oggetto [!DNL Salesforce].

>[!MORELIKETHIS]
>
>* [Sincronizza attività di vendita con Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md)
>* [Sincronizzazione attività promemoria con Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/tasks/reminder-task-sync-with-salesforce.md)
