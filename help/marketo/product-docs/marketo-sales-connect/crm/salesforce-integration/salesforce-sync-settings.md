---
unique-page-id: 18317669
description: Impostazioni di sincronizzazione Salesforce - Documenti Marketo - Documentazione del prodotto
title: Impostazioni di sincronizzazione Salesforce
exl-id: 024c60ac-569f-4051-9eee-1e8d00f7296c
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 0%

---

# Impostazioni di sincronizzazione Salesforce {#salesforce-sync-settings}

## Registrazione dell’attività e-mail a Salesforce tramite API {#logging-email-activity-to-salesforce-via-api}

Questa funzionalità richiede di essere nell&#39;edizione Enterprise/Unlimited di Salesforce o nell&#39;edizione Professional se hai acquistato Integration tramite API di servizi Web.

>[!PREREQUISITES]
>
>È necessario che Salesforce e Sales Connect siano connessi.

1. In Sales Connect, fai clic sull&#39;icona a forma di ingranaggio in alto a destra e seleziona **Impostazioni**.

   ![](assets/one-2.png)

1. In Il mio account (Impostazioni amministratore se sei un amministratore), fai clic su **Salesforce**.

   ![](assets/two-2.png)

1. Fare clic sulla scheda **Impostazioni sincronizzazione**.

   ![](assets/three-1.png)

1. Fai clic sulla freccia accanto a Registra attività e-mail in Salesforce.

   ![](assets/four-1.png)

1. Fare clic sulla scheda **API Salesforce**. In questa scheda puoi impostare le tue preferenze per la registrazione delle informazioni in Salesforce. Al termine, fai clic su **Salva**.

   ![](assets/five.png)

## Registrazione dell’attività e-mail a Salesforce tramite e-mail a Salesforce (BCC) {#logging-email-activity-to-salesforce-via-email-to-salesforce-bcc}

Dopo aver attivato &quot;E-mail a Salesforce (BCC)&quot;, riceverai un CCN delle e-mail di vendita e le e-mail verranno registrate come attività su opportunità, lead e contatti.

>[!PREREQUISITES]
>
>È necessario che Salesforce e Sales Connect siano connessi.

**Per registrare le e-mail in Salesforce tramite e-mail (CCN)**

1. In Sales Connect, fai clic sull&#39;icona a forma di ingranaggio in alto a destra e seleziona **Impostazioni**.

   ![](assets/one-3.png)

1. In Il mio account (Impostazioni amministratore se sei un amministratore), fai clic su **Salesforce**.

   ![](assets/two-3.png)

1. Fare clic sulla scheda **Impostazioni sincronizzazione**.

   ![](assets/three-1.png)

1. Fai clic sulla scheda **Invia e-mail a Salesforce (BCC)** e fai clic su **Attiva**.

   ![](assets/six-2.png)

Se per qualche motivo il tuo indirizzo e-mail Salesforce non effettua il pull-in, segui questi passaggi per attivare la funzione Ccn nel tuo account Salesforce:

1. Accedi all’istanza Salesforce.
1. Trova il tuo nome utente nell’angolo in alto a destra e seleziona la barra a discesa.
1. Seleziona **Impostazioni personali**.
1. Seleziona **E-mail**.
1. Seleziona **La mia e-mail a Salesforce**.
1. In questa pagina viene visualizzato il campo &quot;E-mail all’indirizzo Salesforce&quot;. Se non è presente alcun elemento popolato accanto a esso, scorri verso il basso fino a &quot;I miei indirizzi e-mail accettabili&quot;.
1. Immettere gli indirizzi e-mail che si desidera impostare come CCN.
1. Fai clic su **Salva modifiche**.

**Impossibile trovare il mio indirizzo e-mail a Salesforce nelle mie impostazioni**

Se nelle tue Impostazioni non trovi La mia e-mail a Salesforce, l’Amministratore potrebbe non averla abilitata. Ciò può accadere se il tuo team non ha mai utilizzato Salesforce o se non hai mai utilizzato l’indirizzo in Ccn fornito da Salesforce.

>[!NOTE]
>
>Per configurare questa impostazione, è necessario disporre dei privilegi di amministratore.

1. Fare clic su **Configurazione**.
1. Fare clic su **Amministrazione e-mail**.
1. Fai clic su **Invia e-mail a Salesforce**.
1. Fai clic su **Modifica**.
1. Seleziona la casella accanto a &quot;Attivo&quot;.
1. Fai clic su **Salva**.

## Sincronizza attività/promemoria vendite con attività Salesforce {#sync-sales-connect-tasks-reminders-to-salesforce-tasks}

1. Fai clic sull&#39;icona ingranaggio in alto a destra e seleziona **Impostazioni**.

   ![](assets/one-3.png)

1. In Il mio account (Impostazioni amministratore se sei un amministratore), fai clic su **Salesforce**.

   ![](assets/two-2.png)

1. Fare clic sulla scheda **Impostazioni sincronizzazione**.

   ![](assets/three-1.png)

1. Fare clic sulla freccia accanto a Sincronizza attività/promemoria di Sales Connect con attività Salesforce.

   ![](assets/seven-2.png)

1. Scegli l’opzione desiderata (l’opzione &quot;Do not sync to Salesforce tasks&quot; (Non sincronizzare con le attività Salesforce) è selezionata per impostazione predefinita).

   ![](assets/eight.png)
