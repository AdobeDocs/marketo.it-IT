---
description: Guida alla configurazione dell’amministratore delle azioni di Sales Insight - Documentazione di Marketo - Documentazione del prodotto
title: Guida alla configurazione dell'amministratore delle azioni di Sales Insight
exl-id: 339d518d-445b-4634-ab81-92c9d5541927
feature: Sales Insight Actions
source-git-commit: 1f228323c18204149630a7cb77d6ae0a88b425e3
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 0%

---

# Guida alla configurazione dell&#39;amministratore delle azioni di Sales Insight {#sales-insight-actions-admin-setup-guide}

>[!NOTE]
>
>Marketo Sales Insight Actions è un&#39;applicazione basata su Web che si integra esclusivamente con il sistema CRM Salesforce tramite il [pacchetto Marketo Sales Insight](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}. A volte viene chiamato &quot;Vendite Marketo&quot; o semplicemente &quot;Azioni&quot;.

>[!PREREQUISITES]
>
>* Conferma con il team dell&#39;account Adobe (il tuo Account Manager) che le azioni MSI sono state abilitate per l&#39;account di Marketo Engage (se non disponi di un Account Manager, contatta il [supporto Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}).
>* È necessario configurare la sincronizzazione Marketo/Salesforce.

<table>
 <tr>
  <th>Persona</th>
  <th>Passaggio</th>
 </tr>
 <tr>
  <td>Amministratore Marketo</td>
  <td>Configura account di vendita Marketo</td>
 </tr>
 <tr>
  <td>Amministratore Marketo o amministratore <br/>Salesforce</td>
  <td>Connetti account Marketo Sales a Salesforce</td>
 </tr>
 <tr>
  <td>Amministratore Marketo</td>
  <td>Connetti account di vendita Marketo a Marketo</td>
 </tr>
 <tr>
  <td>Amministratore Marketo</td>
  <td>Avvia sincronizzazione dati da Marketo all'account di vendita Marketo</td>
 </tr>
 <tr>
  <td>Amministratore Marketo</td>
  <td>Invita utenti alle azioni MSI</td>
 </tr>
 <tr>
  <td>Amministratore Salesforce</td>
  <td>Installare/aggiornare il pacchetto MSI in Salesforce</td>
 </tr>
 <tr>
  <td>Amministratore Salesforce</td>
  <td>Configurare azioni MSI in Salesforce</td>
 </tr>
</table>

## Configura account di vendita Marketo {#set-up-marketo-sales-account}

1. In Marketo, fai clic su **Amministratore**.

   ![](assets/msi-actions-admin-guide-1.png)

   >[!NOTE]
   >
   >Se non visualizzi un ID client e un segreto client nella scheda Informazioni integrazione, attiva l’istanza Azioni invitando il primo utente; verranno visualizzati l’ID client e il segreto client.

1. Fai clic su **Insight vendite**, quindi su **Configurazione azioni**. Selezionare da un elenco di amministratori di Marketo da invitare e fare clic su **Invia invito**.

   ![](assets/msi-actions-admin-guide-2.png)

L’utente riceverà un’e-mail con i passaggi per accedere all’account.

>[!NOTE]
>
>Gli utenti aggiuntivi non verranno aggiunti tramite Marketo, ma tramite la pagina Gestione utente dell&#39;account di vendita. [Fai clic qui](/help/marketo/product-docs/marketo-sales-connect/admin/invite-users.md){target="_blank"} per ulteriori informazioni sull&#39;aggiunta di altri utenti.

## Connetti account vendite Marketo a Salesforce {#connect-marketo-sales-account-to-salesforce}

1. Nel tuo account Marketo Sales, fai clic sull&#39;icona ingranaggio e seleziona **Impostazioni**.

   ![](assets/msi-actions-admin-guide-3.png)

1. In Impostazioni amministrazione fare clic su **Salesforce**.

   ![](assets/msi-actions-admin-guide-4.png)

1. Nella scheda Connessioni e personalizzazioni fare clic su **Connetti**.

   ![](assets/msi-actions-admin-guide-5.png)

1. Fai clic su **OK**.

   ![](assets/msi-actions-admin-guide-6.png)

Se hai già effettuato l’accesso a Salesforce, sarai connesso. In caso contrario, ti verrà chiesto di effettuare l&#39;accesso.

## Collegare Marketo all&#39;account App vendite {#connect-marketo-to-your-sales-apps-account}

1. Nel tuo account Marketo Sales, fai clic sull&#39;icona ingranaggio e seleziona **Impostazioni**.

   ![](assets/msi-actions-admin-guide-7.png)

1. In Impostazioni amministrazione fare clic su **Marketo**.

   ![](assets/msi-actions-admin-guide-8.png)

1. Fai clic su **connetti**. Il tuo account verrà quindi connesso.

   ![](assets/msi-actions-admin-guide-9.png)

>[!NOTE]
>
>Se non si connette, copiare le credenziali dalla scheda &quot;Configurazione azioni&quot; di Marketo Sales Insight e incollarle nella scheda Configurazione.

## Avvia sincronizzazione dati {#initiate-data-sync}

La sincronizzazione dei campi di unificazione dei dati per le azioni di Sales Insight consente al sistema di richiamare le informazioni sulle persone dal database del Marketo Engage nel database delle azioni di Sales Insight, mantenendo aggiornati i dati sulle persone e garantendo che le attività vengano registrate nei record corretti in Marketo e Salesforce.

>[!CAUTION]
>
>Una volta avviata la sincronizzazione dei dati, **non** rimuovere l&#39;utente originale nell&#39;istanza Azioni approfondimento vendite. Questo è l’utente a cui è stato inviato il primo invito.

1. In Marketo, fai clic su **Amministratore**.

   ![](assets/msi-actions-admin-guide-10.png)

1. Fare clic su **Informazioni sulle vendite**.

   ![](assets/msi-actions-admin-guide-11.png)

1. Fare clic sulla scheda **Configurazione azioni**. Nella scheda Sincronizzazione campi azione, fai clic su **Sincronizza**.

   ![](assets/msi-actions-admin-guide-12.png)

1. Verrà visualizzata un&#39;anteprima dei campi che verranno sincronizzati. Fare clic su **Avvia sincronizzazione**.

   ![](assets/msi-actions-admin-guide-13.png)

I record di persone esistenti in Marketo e Salesforce verranno sincronizzati con il tuo account Marketo Sales Apps.

>[!NOTE]
>
>Per ulteriori informazioni sulla sincronizzazione dei dati relativi a persone e attività tra Sales Insight Actions, Marketo e Salesforce, [fai clic qui](/help/marketo/product-docs/marketo-sales-insight/actions/admin/sync-sales-action-data-with-marketo-and-salesforce.md){target="_blank"}.

## Invita singoli utenti alle azioni MSI {#invite-individual-users-to-msi-actions}

1. Nel tuo account Marketo Sales, fai clic sull&#39;icona ingranaggio e seleziona **Impostazioni**.

   ![](assets/msi-actions-admin-guide-14.png)

1. In Impostazioni amministrazione selezionare **Gestione utente**.

   ![](assets/msi-actions-admin-guide-15.png)

1. Fai clic su **Azioni** e seleziona **Invita utenti**.

   ![](assets/msi-actions-admin-guide-16.png)

1. Immetti gli indirizzi e-mail e fai clic su **Invita**.

   ![](assets/msi-actions-admin-guide-17.png)

>[!NOTE]
>
>Per impostazione predefinita, tutti i nuovi membri vengono aggiunti al team Everyone.

Riceverai un messaggio di conferma.

## Invitare utenti tramite CSV ad azioni MSI {#invite-users-via-csv-to-msi-actions}

1. Nel tuo account Marketo Sales, fai clic sull&#39;icona ingranaggio e seleziona **Impostazioni**.

   ![](assets/msi-actions-admin-guide-18.png)

1. In Impostazioni amministrazione selezionare **Gestione utente**.

   ![](assets/msi-actions-admin-guide-19.png)

1. Fai clic su **Azioni** e seleziona **Invita utenti tramite CSV**.

   ![](assets/msi-actions-admin-guide-20.png)

1. Cerca il file CSV nel computer, selezionalo e fai clic su **Avanti**.

   ![](assets/msi-actions-admin-guide-21.png)

1. Verificare che i campi siano mappati correttamente e fare clic su **Invita**.

   ![](assets/msi-actions-admin-guide-22.png)

Riceverai un messaggio di conferma una volta inviati gli inviti.

>[!NOTE]
>
>Al termine, puoi aggiornare il pacchetto MSI esistente o installarne uno nuovo e passare alla [configurazione delle azioni MSI in Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/crm/salesforce-package-configuration/sales-insight-actions-configuration-in-salesforce.md){target="_blank"}.
