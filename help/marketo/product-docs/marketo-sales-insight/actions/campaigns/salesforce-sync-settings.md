---
description: Impostazioni di sincronizzazione Salesforce - Documenti Marketo - Documentazione del prodotto
title: Impostazioni di sincronizzazione Salesforce
exl-id: fa13ced2-6184-485f-a0ef-813ccab4f0fe
feature: Sales Insight Actions
source-git-commit: 350490c93d8f2bcc278f9f3e82018a1db91a1146
workflow-type: tm+mt
source-wordcount: '709'
ht-degree: 0%

---

# Impostazioni di sincronizzazione Salesforce {#salesforce-sync-settings}

## Registrazione dell’attività e-mail a Salesforce tramite API {#logging-email-activity-to-salesforce-via-api}

Questa funzionalità richiede di essere nell&#39;edizione Enterprise/Unlimited di Salesforce o nell&#39;edizione Professional se hai acquistato Integration tramite API di servizi Web.

>[!PREREQUISITES]
>
>Le azioni Salesforce e Sales Insight devono essere collegate.

1. In Azioni approfondimento vendite, fai clic sull’icona a forma di ingranaggio e seleziona **Impostazioni**.

   ![](assets/salesforce-sync-settings-1.png)

1. In Impostazioni amministratore (o &quot;Il mio account&quot; se non sei un amministratore), fai clic su **Salesforce**.

   ![](assets/salesforce-sync-settings-2.png)

1. Fai clic su **Impostazioni di sincronizzazione** scheda.

   ![](assets/salesforce-sync-settings-3.png)

1. Fai clic sulla freccia accanto a Registra attività e-mail in Salesforce.

   ![](assets/salesforce-sync-settings-4.png)

1. Fai clic su **API Salesforce** scheda. In questa scheda puoi impostare le tue preferenze per la registrazione delle informazioni in Salesforce. Clic **Salva** al termine.

   ![](assets/salesforce-sync-settings-5.png)

## Registrazione dell’attività e-mail a Salesforce tramite e-mail a Salesforce (BCC) {#logging-email-activity-to-salesforce-via-email-to-salesforce-bcc}

Dopo aver attivato &quot;E-mail a Salesforce (BCC)&quot;, riceverai un CCN delle e-mail di vendita e le e-mail verranno registrate come attività su opportunità, lead e contatti.

>[!PREREQUISITES]
>
>Le azioni Salesforce e Sales Insight devono essere collegate.

**Per registrare le e-mail in Salesforce tramite e-mail (CCN)**

1. In Marketo Sales, fai clic sull’icona a forma di ingranaggio e seleziona **Impostazioni**.

   ![](assets/salesforce-sync-settings-6.png)

1. In Impostazioni amministratore (o &quot;Il mio account&quot; se non sei un amministratore), fai clic su **Salesforce**.

   ![](assets/salesforce-sync-settings-7.png)

1. Fai clic su **Impostazioni di sincronizzazione** scheda.

   ![](assets/salesforce-sync-settings-8.png)

1. Fai clic su **E-mail a Salesforce (BCC)** e fai clic su **Attiva**.

   ![](assets/salesforce-sync-settings-9.png)

Se per qualche motivo il tuo indirizzo e-mail Salesforce non effettua il pull-in, segui questi passaggi per attivare la funzione Ccn nel tuo account Salesforce:

1. Accedi all’istanza Salesforce.
1. Trova il tuo nome utente nell’angolo in alto a destra e seleziona la barra a discesa.
1. Seleziona **Le mie impostazioni**.
1. Seleziona **E-mail**.
1. Seleziona **E-mail a Salesforce**.
1. In questa pagina viene visualizzato il campo &quot;E-mail all’indirizzo Salesforce&quot;. Se non è presente alcun elemento popolato accanto a esso, scorri verso il basso fino a &quot;I miei indirizzi e-mail accettabili&quot;.
1. Immettere gli indirizzi e-mail che si desidera impostare come CCN.
1. Clic **Salva modifiche**.

**Non riesco a trovare la mia e-mail a Salesforce nelle mie impostazioni**

Se nelle tue Impostazioni non trovi La mia e-mail a Salesforce, l’Amministratore potrebbe non averla abilitata. Ciò può accadere se il tuo team non ha mai utilizzato Salesforce o se non hai mai utilizzato l’indirizzo in Ccn fornito da Salesforce.

>[!NOTE]
>
>Per configurare questa impostazione, è necessario disporre dei privilegi di amministratore.

1. Clic **Configurazione**.
1. Clic **Amministrazione e-mail**.
1. Clic **E-mail a Salesforce**.
1. Clic **Modifica**.
1. Seleziona la casella accanto a &quot;Attivo&quot;.
1. Clic **Salva**.

## Sincronizza attività/promemoria di Sales Insight con le attività Salesforce {#sync-sales-insight-actions-tasks-reminders-to-salesforce-tasks}

1. In Azioni approfondimento vendite, fai clic sull’icona a forma di ingranaggio e seleziona **Impostazioni**.

   ![](assets/salesforce-sync-settings-10.png)

1. In Impostazioni amministratore (o &quot;Il mio account&quot; se non sei un amministratore), fai clic su **Salesforce**.

   ![](assets/salesforce-sync-settings-11.png)

1. Fai clic su **Impostazioni di sincronizzazione** scheda.

   ![](assets/salesforce-sync-settings-12.png)

1. Fare clic sulla freccia accanto a Sincronizza attività/promemoria vendite Marketo con attività Salesforce.

   ![](assets/salesforce-sync-settings-13.png)

1. Scegli l’opzione desiderata (l’opzione &quot;Do not sync to Salesforce tasks&quot; (Non sincronizzare con le attività Salesforce) è selezionata per impostazione predefinita).

   ![](assets/salesforce-sync-settings-14.png)

## Sincronizzazione delle attività di Sales Insight con Salesforce per la prima volta {#syncing-sales-insight-ations-tasks-with-salesforce-for-the-first-time}

Quando attivi per la prima volta la sincronizzazione tra le azioni di approfondimento sulle vendite e le attività di Salesforce, importiamo le attività di Salesforce. Non trasferiremo a Salesforce nessuna delle attività attuali che hai in Azioni approfondimenti vendite. Per ridurre l&#39;ingombro e i duplicati, le uniche attività sincronizzate da Sales Insight Actions in Salesforce sono quelle create dopo la sincronizzazione di Sales Insight Actions con SFDC.

Ecco cosa accade quando si sincronizzano le azioni Sales Insight e le attività SFDC:

Non appena si fa clic su Salva durante la sincronizzazione delle attività, queste vengono sincronizzate. Inizialmente questo richiederà del tempo.

Tutti i promemoria aggiornati o creati nelle ultime 24 ore verranno inseriti da SFDC in Sales Insight Actions. La sincronizzazione è basata sulla data di scadenza e tutte queste attività verranno sincronizzate nel back-end, ma in Centro comandi verranno visualizzate solo le attività in scadenza oggi e domani.

Se la sincronizzazione è stata attivata in precedenza ed è stata eliminata qualsiasi attività in SFDC, qualsiasi elemento eliminato negli ultimi 15 giorni verrà eliminato da Centro comandi.

Finché la sincronizzazione è abilitata, sincronizzeremo costantemente le attività tra le azioni Sales Insight e SFDC.

Dopo la sincronizzazione iniziale, tutte le attività create, modificate, completate o eliminate in Azioni approfondimenti vendite verranno sincronizzate con l’elenco delle attività in Salesforce. E qualsiasi cosa creata, modificata, completata o eliminata in Salesforce aggiornerà l’elenco delle attività in Azioni approfondimento vendite.

Per attivare questa sincronizzazione, seleziona la casella di sincronizzazione nella pagina Impostazioni dell’applicazione web.
