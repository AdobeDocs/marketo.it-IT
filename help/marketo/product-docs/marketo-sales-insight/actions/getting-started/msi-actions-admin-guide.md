---
description: Guida per l’amministrazione delle azioni MSI - Documenti Marketo - Documentazione del prodotto
title: Guida per l’amministrazione delle azioni MSI
hide: true
hidefromtoc: true
exl-id: 339d518d-445b-4634-ab81-92c9d5541927
source-git-commit: e3d175d9f6131ec9798c4047ccf79858c254c745
workflow-type: tm+mt
source-wordcount: '492'
ht-degree: 0%

---

# Guida per l’amministrazione delle azioni MSI {#msi-actions-admin-guide}

>[!PREREQUISITES]
>
>* Conferma con il tuo Customer Success Manager che le azioni MSI sono state abilitate per il tuo account Marketo (se non hai un CSM, ti preghiamo di [contattare il supporto Marketo](https://nation.marketo.com/t5/support/ct-p/Support)).
>* È necessario configurare la sincronizzazione Marketo/Salesforce.


<table>
 <tr>
  <th>Persona</th>
  <th>Passaggio</th>
 </tr>
 <tr>
  <td>Amministratore Marketo</td>
  <td>Imposta account vendite Marketo</td>
 </tr>
 <tr>
  <td>Amministratore Marketo o <br/>Amministratore Salesforce</td>
  <td>Collegare l'account Marketo Sales a Salesforce</td>
 </tr>
 <tr>
  <td>Amministratore Marketo</td>
  <td>Collegare l'account Marketo Sales a Marketo</td>
 </tr>
 <tr>
  <td>Amministratore Marketo</td>
  <td>Avviare la sincronizzazione dei dati da Marketo all'account di vendita Marketo</td>
 </tr>
 <tr>
  <td>Amministratore Marketo</td>
  <td>Invitare gli utenti su MSI-Actions</td>
 </tr>
 <tr>
  <td>Amministratore Salesforce</td>
  <td>Installa/aggiorna il pacchetto MSI in Salesforce</td>
 </tr>
 <tr>
  <td>Amministratore Salesforce</td>
  <td>Configurare le azioni MSI in Salesforce</td>
 </tr>
</table>

## Imposta account di vendita Marketo {#set-up-marketo-sales-account}

1. In Marketo, fai clic su **Amministratore**.

   ![](assets/msi-actions-admin-guide-1.png)

1. Fai clic su **Approfondimenti vendite**, quindi **Configurazione azioni**. Seleziona da un elenco di amministratori Marketo da invitare e fai clic su **Invia invito**.

   ![](assets/msi-actions-admin-guide-2.png)

L’utente riceverà un’e-mail con i passaggi per accedere all’account.

>[!NOTE]
>
>Gli utenti aggiuntivi non verranno aggiunti tramite Marketo e verranno aggiunti tramite la pagina Gestione utenti dell&#39;account di vendita . [Fai clic qui](/help/marketo/product-docs/marketo-sales-connect/admin/invite-users.md) per ulteriori informazioni sull’aggiunta di utenti aggiuntivi.

## Collegare l&#39;account di vendita Marketo a Salesforce {#connect-marketo-sales-account-to-salesforce}

1. Nel tuo account Marketo Sales, fai clic sull&#39;icona a forma di ingranaggio e seleziona **Impostazioni**.

   ![](assets/msi-actions-admin-guide-3.png)

1. In Impostazioni amministratore, fai clic su **Salesforce**.

   ![](assets/msi-actions-admin-guide-4.png)

1. Nella scheda Connessioni e personalizzazioni fare clic su **Connetti**.

   ![](assets/msi-actions-admin-guide-5.png)

1. Fai clic su **OK**.

   ![](assets/msi-actions-admin-guide-6.png)

Se hai già effettuato l’accesso a Salesforce, verrai connesso. In caso contrario, ti verrà chiesto di effettuare l’accesso.

## Collega Marketo al tuo account App di vendita {#connect-marketo-to-your-sales-apps-account}

1. Nel tuo account Marketo Sales, fai clic sull&#39;icona a forma di ingranaggio e seleziona **Impostazioni**.

   ![](assets/msi-actions-admin-guide-7.png)

1. In Impostazioni amministratore, fai clic su **Marketo**.

   ![](assets/msi-actions-admin-guide-8.png)

1. Fai clic su **connect**. Il tuo account verrà quindi connesso.

   ![](assets/msi-actions-admin-guide-9.png)

>[!NOTE]
>
>Se non si collega, copia le credenziali dalla scheda &quot;Configurazione azioni&quot; di Marketo Sales Insight e incollale nella scheda Configurazione.

## Avvia sincronizzazione dati {#initiate-data-sync}

1. In Marketo, fai clic su **Amministratore**.

   ![](assets/msi-actions-admin-guide-10.png)

1. Fare clic su Insight vendite.

   ![](assets/msi-actions-admin-guide-11.png)

1. Fare clic sulla scheda Configurazione azioni. Nella scheda Sincronizzazione campo azione, fai clic su **Sincronizzazione**.

   ![](assets/msi-actions-admin-guide-12.png)

1. Verrà visualizzata un’anteprima dei campi che verranno sincronizzati. Fai clic su **Avvia sincronizzazione**.

   ![](assets/msi-actions-admin-guide-13.png)

I record personali esistenti in Marketo e Salesforce verranno sincronizzati nel tuo account App vendite Marketo.

## Invitare singoli utenti alle azioni MSI {#invite-individual-users-to-msi-actions}

1. Nel tuo account Marketo Sales, fai clic sull&#39;icona a forma di ingranaggio e seleziona **Impostazioni**.

   ![](assets/msi-actions-admin-guide-14.png)

1. In Impostazioni amministratore, seleziona **Gestione utente**.

   ![](assets/msi-actions-admin-guide-15.png)

1. Fai clic su **Azioni** e seleziona **Invitare gli utenti**.

   ![](assets/msi-actions-admin-guide-16.png)

1. Inserisci gli indirizzi e-mail e fai clic su **Invito**.

   ![](assets/msi-actions-admin-guide-17.png)

>[!NOTE]
>
>Per impostazione predefinita, tutti i nuovi membri verranno aggiunti al team Everyone.

Riceverai un messaggio di conferma.

## Invitare gli utenti tramite CSV nelle azioni MSI {#invite-users-via-csv-to-msi-actions}

1. Nel tuo account Marketo Sales, fai clic sull&#39;icona a forma di ingranaggio e seleziona **Impostazioni**.

   ![](assets/msi-actions-admin-guide-18.png)

1. In Impostazioni amministratore, seleziona **Gestione utente**.

   ![](assets/msi-actions-admin-guide-19.png)

1. Fai clic su **Azioni** e seleziona **Invitare utenti tramite CSV**.

   ![](assets/msi-actions-admin-guide-20.png)

1. Cerca il CSV sul computer, selezionalo e fai clic su **Successivo**.

   ![](assets/msi-actions-admin-guide-21.png)

1. Conferma che i campi siano mappati correttamente e fai clic su **Invito**.

   ![](assets/msi-actions-admin-guide-22.png)

Riceverai un messaggio di conferma dopo l’invio degli inviti.

>[!NOTE]
>
>Una volta fatto questo, puoi aggiornare il pacchetto MSI esistente o installarne uno nuovo e passare a [configurazione delle azioni MSI in Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/salesforce-configuration/msi-actions-configuration-in-salesforce.md).
