---
unique-page-id: 18317669
description: Impostazioni di sincronizzazione Salesforce - Documenti Marketo - Documentazione del prodotto
title: Impostazioni di sincronizzazione Salesforce
exl-id: 024c60ac-569f-4051-9eee-1e8d00f7296c
source-git-commit: 56db82ef98d774f8ac56c1401ef7ef275862d1dc
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# Impostazioni di sincronizzazione Salesforce {#salesforce-sync-settings}

## Registrazione dell’attività e-mail su Salesforce tramite API {#logging-email-activity-to-salesforce-via-api}

Questa funzionalità richiede l’utilizzo dell’edizione Enterprise/Unlimited di Salesforce o dell’edizione Professional se hai acquistato l’integrazione tramite API di Web Services.

>[!PREREQUISITES]
>
>È necessario collegare Salesforce e Sales Connect.

1. In Sales Connect, fai clic sull&#39;icona dell&#39;ingranaggio in alto a destra e seleziona **Impostazioni**.

   ![](assets/one-2.png)

1. In My Account (Admin Settings (Impostazioni amministratore), fai clic su **Salesforce**.

   ![](assets/two-2.png)

1. Fai clic sul pulsante **Impostazioni di sincronizzazione** scheda .

   ![](assets/three-1.png)

1. Fai clic sulla freccia accanto a Registra attività e-mail su Salesforce.

   ![](assets/four-1.png)

1. Fai clic sul pulsante **API Salesforce** scheda . In questa scheda puoi impostare la tua preferenza per la registrazione delle informazioni su Salesforce. Fai clic su **Salva** al termine.

   ![](assets/five.png)

## Registrazione dell’attività e-mail a Salesforce tramite e-mail a Salesforce (CCN) {#logging-email-activity-to-salesforce-via-email-to-salesforce-bcc}

Una volta attivato &quot;Email to Salesforce (CCN)&quot;, riceverai un CCN delle tue e-mail di vendita e le tue verranno registrate come attività su opportunità, lead e contatti.

>[!PREREQUISITES]
>
>È necessario collegare Salesforce e Sales Connect.

**Per registrare le e-mail in Salesforce tramite E-mail (CCN)**

1. In Sales Connect, fai clic sull&#39;icona dell&#39;ingranaggio in alto a destra e seleziona **Impostazioni**.

   ![](assets/one-3.png)

1. In My Account (Admin Settings (Impostazioni amministratore), fai clic su **Salesforce**.

   ![](assets/two-3.png)

1. Fai clic sul pulsante **Impostazioni di sincronizzazione** scheda .

   ![](assets/three-1.png)

1. Fai clic sul pulsante **E-mail a Salesforce (CCN)** e fai clic su **Attiva**.

   ![](assets/six-2.png)

Se per qualche motivo l&#39;indirizzo Email to Salesforce non effettua il pull in, segui questi passaggi per attivare la funzione CCN nel tuo account Salesforce:

1. Accedi alla tua istanza Salesforce.
1. Trova il nome utente nell’angolo in alto a destra e seleziona la barra a discesa.
1. Seleziona **Impostazioni personali**.
1. Seleziona **E-mail**.
1. Seleziona **E-mail a Salesforce**.
1. In questa pagina verrà visualizzato un campo con l’etichetta &quot;Email to Salesforce Address&quot;. Se accanto a esso non è presente nulla di popolato, scorri verso il basso fino a &quot;I miei indirizzi e-mail accettabili&quot;.
1. Inserisci gli indirizzi e-mail che desideri ricevere da Ccn.
1. Fai clic su **Salva modifiche**.

**Impossibile trovare l&#39;e-mail a Salesforce nelle impostazioni**

Se in Impostazioni non trovi My Email to Salesforce , il tuo amministratore potrebbe non averlo abilitato. Questo può accadere se il tuo team è nuovo di Salesforce o se il tuo team non ha mai utilizzato l’indirizzo CCN fornito da Salesforce.

>[!NOTE]
>
>Per configurarlo, dovrai disporre dei privilegi di amministratore.

1. Fai clic su **Configurazione**.
1. Fai clic su **Amministrazione e-mail**.
1. Fai clic su **Invia e-mail a Salesforce**.
1. Fai clic su **Modifica**.
1. Seleziona la casella accanto a &quot;Attivo&quot;.
1. Fai clic su **Salva**.

## Sincronizza attività di vendita/promemoria in attività Salesforce {#sync-sales-connect-tasks-reminders-to-salesforce-tasks}

1. Fai clic sull’icona a forma di ingranaggio in alto a destra e seleziona **Impostazioni**.

   ![](assets/one-3.png)

1. In My Account (Admin Settings (Impostazioni amministratore), fai clic su **Salesforce**.

   ![](assets/two-2.png)

1. Fai clic sul pulsante **Impostazioni di sincronizzazione** scheda .

   ![](assets/three-1.png)

1. Fare clic sulla freccia accanto a Sincronizza attività/promemoria di connessione vendite alle attività Salesforce.

   ![](assets/seven-2.png)

1. Scegli l’opzione desiderata (&quot;Non sincronizzare con le attività Salesforce&quot; è selezionata per impostazione predefinita).

   ![](assets/eight.png)
