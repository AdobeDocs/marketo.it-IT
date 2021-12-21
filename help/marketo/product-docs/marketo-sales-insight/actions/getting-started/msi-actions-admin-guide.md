---
description: Guida per l’amministrazione delle azioni MSI - Documenti Marketo - Documentazione del prodotto
title: Guida per l’amministrazione delle azioni MSI
hide: true
hidefromtoc: true
source-git-commit: 9ee07611ffae25fea4bffa3124927083bf187ddd
workflow-type: tm+mt
source-wordcount: '509'
ht-degree: 0%

---

# Guida per l’amministrazione delle azioni MSI {#msi-actions-admin-guide}

>[!PREREQUISITES]
>
>* Conferma con il tuo Customer Success Manager che le azioni MSI sono state abilitate per il tuo account Marketo (se non hai un CSM, ti preghiamo di [contattare il supporto](https://nation.marketo.com/t5/support/ct-p/Support)).
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

PICC

1. Fai clic su **Approfondimenti vendite**, quindi **Configurazione azioni**. Seleziona da un elenco di amministratori Marketo da invitare e fai clic su **Invia invito**.

PICC

L’utente riceverà un’e-mail con i passaggi per accedere all’account.

>[!NOTE]
>
>Gli utenti aggiuntivi non verranno aggiunti tramite Marketo e verranno aggiunti tramite la pagina Gestione utenti dell&#39;account di vendita . [Fai clic qui](/help/marketo/product-docs/marketo-sales-connect/admin/invite-users.md) per ulteriori informazioni sull’aggiunta di utenti aggiuntivi.

## Collegare l&#39;account di vendita Marketo a Salesforce {#connect-marketo-sales-account-to-salesforce}

1. Nel tuo account Marketo Sales, fai clic sull&#39;icona a forma di ingranaggio e seleziona **Impostazioni**.

PICC

1. In Impostazioni amministratore, fai clic su **Salesforce**.

PICC

1. Nella scheda Connessioni e personalizzazioni fare clic su **Connetti**.

PICC

1. Fai clic su **OK**.

PICC

Se hai già effettuato l’accesso a Salesforce, verrai connesso. In caso contrario, ti verrà chiesto di effettuare l’accesso.

## Collega Marketo al tuo account App di vendita {#connect-marketo-to-your-sales-apps-account}

1. Nel tuo account Marketo Sales, fai clic sull&#39;icona a forma di ingranaggio e seleziona **Impostazioni**.

PICC

1. In Impostazioni amministratore, fai clic su **Marketo**.

PICC

1. Fai clic su **connect**. Il tuo account verrà quindi connesso.

>[!NOTE]
>
>Se non si collega, copia le credenziali dalla scheda &quot;Configurazione azioni&quot; di Marketo Sales Insight e incollale nella scheda Configurazione.

## Avvia sincronizzazione dati {#initiate-data-sync}

1. In Marketo, fai clic su Amministratore.

PICC

1. Fare clic su Insight vendite, quindi su Configurazione azioni.

PICC

1. Nella scheda Sincronizzazione campo azione, fai clic su **Sincronizzazione**.

PICC

1. Verrà visualizzata un’anteprima dei campi che verranno sincronizzati. Fai clic su **Avvia sincronizzazione**.

PICC

I record personali esistenti in Marketo e Salesforce verranno sincronizzati nel tuo account App vendite Marketo.

## Invitare singoli utenti alle azioni MSI {#invite-individual-users-to-msi-actions}

1. Nel tuo account Marketo Sales, fai clic sull&#39;icona a forma di ingranaggio e seleziona **Impostazioni**.

PICC

1. In Impostazioni amministratore, seleziona **Gestione utente**.

PICC

1. Fai clic su **Azioni** e seleziona **Invitare gli utenti**.

PICC

1. Inserisci gli indirizzi e-mail e fai clic su **Invito**.

>[!NOTE]
>
>Per impostazione predefinita, tutti i nuovi membri verranno aggiunti al team Everyone.

Riceverai un messaggio di conferma.

## Invitare gli utenti tramite CSV nelle azioni MSI {#invite-users-via-csv-to-msi-actions}

1. Nel tuo account Marketo Sales, fai clic sull&#39;icona a forma di ingranaggio e seleziona **Impostazioni**.

PICC

1. In Impostazioni amministratore, seleziona **Gestione utente**.

PICC

1. Fai clic su **Azioni** e seleziona **Invitare utenti tramite CSV**.

PICC

1. Cerca il CSV sul computer, selezionalo e fai clic su **Successivo**.

PICC

1. Conferma che i campi siano mappati correttamente e fai clic su **Invito**.

PICC

Riceverai un messaggio di conferma dopo l’invio degli inviti.

>[!NOTE]
>
>Una volta fatto questo, puoi aggiornare il pacchetto MSI esistente o installarne uno nuovo e passare a [configurazione delle azioni MSI in Salesforce](/help/marketo/product-docs/marketo-sales-insight/actions/salesforce-configuration/msi-actions-configuration-in-salesforce.md).
