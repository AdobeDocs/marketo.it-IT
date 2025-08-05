---
description: Sincronizzazione attività promemoria con Salesforce - Documentazione Marketo - Documentazione del prodotto
title: Sincronizzazione attività promemoria con Salesforce
exl-id: 11aa6ab5-5489-4c20-a64d-2fd6fe29506f
feature: Sales Insight Actions
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 0%

---

# Sincronizzazione attività promemoria con [!DNL Salesforce] {#reminder-task-sync-with-salesforce}

>[!NOTE]
>
>Per informazioni su come abilitare l&#39;opzione Sincronizzazione attività, estrarre [Sincronizza attività/promemoria azioni di Insight Sales alle attività di Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/sync-sales-activities-to-salesforce.md#sync-sales-insight-actions-tasks-reminders-to-salesforce-tasks).

Una volta abilitate le impostazioni di sincronizzazione delle attività, gli utenti visualizzeranno le attività promemoria sincronizzate bidirezionalmente con [!DNL Salesforce]. Ciò significa che gli utenti possono gestire le attività da [!DNL Salesforce] o [!DNL Sales Insight Actions] e che i sistemi rimarranno allineati.

## Sincronizzazione campi attività promemoria {#reminder-task-field-sync}

![](assets/reminder-task-sync-with-salesforce-1.png)

Di seguito è riportato un elenco dei campi dell&#39;attività promemoria in [!DNL Sales Insight Actions] e dei campi corrispondenti di [!DNL Salesforce] supportati tramite la sincronizzazione bidirezionale delle attività.

<table>
 <tr>
  <th>[!DNL Sales Insight Actions] Campo attività</th>
  <th>[!DNL Salesforce] Campo attività</th>
  <th>[!DNL Salesforce] Attività</th>
 </tr>
 <tr>
  <td>[!UICONTROL Task Name]</td>
  <td>[!UICONTROL Subject Field]</td>
  <td>Un breve campo di riepilogo destinato a mostrare il titolo dell’attività.</td>
 </tr>
 <tr>
  <td>[!UICONTROL Status]</td>
  <td>[!UICONTROL Task Status]</td>
  <td><p>Mostra lo stato dell'attività. [!DNL Sales Insight Actions] attività hanno due stati mappati a due dei valori nella lista di selezione dello stato dell'attività [!DNL Salesforce].</p>
  <p>Apertura tra [!DNL Sales Insight Actions] = Non avviato tra [!DNL Salesforce].</p>
  <p>Completato in [!DNL Sales Insight Actions] = Completato in [!DNL Salesforce].</p>
  <p>Gli altri valori di stato in [!DNL Salesforce] non verranno sincronizzati con [!DNL Sales Insight Actions].</p></td>
 </tr>
 <tr>
  <td>[!UICONTROL Priority]</td>
  <td>[!UICONTROL Priority]</td>
  <td><p>[!DNL Sales Insight Actions] La priorità può essere Normale o Alta, che corrisponde ai valori di priorità Normale e Alta in [!DNL Salesforce].</p>
  <p>Il valore con priorità bassa in [!DNL Salesforce] non verrà sincronizzato con [!DNL Sales Insight Actions].</p></td>
 </tr>
 <tr>
  <td>[!UICONTROL Due Date]</td>
  <td>[!UICONTROL Due Date]</td>
  <td>Data di scadenza dell'attività.</td>
 </tr>
 <tr>
  <td>[!UICONTROL Details]</td>
  <td>[!UICONTROL Comments]</td>
  <td>Mostra informazioni più dettagliate su ciò che doveva essere completato con l'attività promemoria.</td>
 </tr>
</table>

## È in corso la prima sincronizzazione di [!DNL Sales Insight Actions] attività con [!DNL Salesforce] {#syncing-sales-insight-actions-tasks-with-salesforce-for-the-first-time}

Quando si attiva la sincronizzazione tra [!DNL Sales Insight Actions] e [!DNL Salesforce] attività, le attività [!DNL Salesforce] vengono importate. **non** eseguirà il push delle attività correnti in [!DNL Sales Insight Actions] a [!DNL Salesforce]. Per ridurre l&#39;ingombro e i duplicati, le uniche attività sincronizzate da [!DNL Sales Insight Actions] in [!DNL Salesforce] sono le attività create *dopo* la sincronizzazione di [!DNL Sales Insight Actions] con SFDC.

Ecco cosa accade quando si sincronizzano [!DNL Sales Insight Actions] e le attività di SFDC:

* Non appena si fa clic su Salva durante la sincronizzazione delle attività, queste vengono sincronizzate. Inizialmente questo richiederà del tempo.

* Tutti i promemoria aggiornati o creati nelle ultime 24 ore verranno inseriti da SFDC a [!DNL Sales Insight Actions]. La sincronizzazione è basata sulla data di scadenza e tutte queste attività verranno sincronizzate nel back-end, ma in Centro comandi verranno visualizzate solo le attività in scadenza oggi e domani.

* Se la sincronizzazione è stata attivata in precedenza ed è stata eliminata qualsiasi attività in SFDC, qualsiasi elemento eliminato negli ultimi 15 giorni verrà eliminato da Centro comandi.

* Le attività verranno sincronizzate costantemente tra [!DNL Sales Insight Actions] e SFDC, purché la sincronizzazione sia abilitata.

Dopo la sincronizzazione iniziale, tutte le attività create, modificate, completate o eliminate in [!DNL Sales Insight Actions] verranno sincronizzate con l&#39;elenco delle attività in [!DNL Salesforce]. E qualsiasi elemento creato, modificato, completato o eliminato in [!DNL Salesforce] aggiornerà l&#39;elenco delle attività in [!DNL Sales Insight Actions].

Per attivare questa sincronizzazione, seleziona la casella di sincronizzazione nella [pagina Impostazioni](https://toutapp.com/login) dell&#39;applicazione Web.

>[!NOTE]
>
>Il campo dell&#39;oggetto di un&#39;attività può essere aggiornato in [!DNL Sales Insight Actions] e tale aggiornamento verrà sincronizzato nel campo dell&#39;oggetto [!DNL Salesforce] per l&#39;attività sincronizzata corrispondente, se si utilizza il campo dinamico `{{activity_subject}}` nelle impostazioni [Personalizzazione dettagli attività](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-integration/configure-salesforce-activity-detail-customization.md). Al contrario, eventuali aggiornamenti apportati al campo dell&#39;oggetto in [!DNL Salesforce] *non* verranno sincronizzati con il campo dell&#39;oggetto attività promemoria [!DNL Sales Insight Actions].
