---
description: Impostazioni di sincronizzazione Salesforce - Documentazione Marketo - Documentazione del prodotto
title: Impostazioni sincronizzazione Salesforce
exl-id: fa13ced2-6184-485f-a0ef-813ccab4f0fe
feature: Sales Insight Actions
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '574'
ht-degree: 1%

---

# Impostazioni di sincronizzazione [!DNL Salesforce] {#salesforce-sync-settings}

## Registrazione dell&#39;attività e-mail in [!DNL Salesforce] tramite API {#logging-email-activity-to-salesforce-via-api}

Questa funzionalità richiede l&#39;iscrizione all&#39;edizione Enterprise/Unlimited di [!DNL Salesforce] o all&#39;edizione Professional se è stata acquistata l&#39;integrazione tramite API dei servizi Web.

>[!PREREQUISITES]
>
>[!DNL Salesforce] e [!DNL Sales Insight Actions] devono essere connessi.

1. In [!DNL Sales Insight Actions], fare clic sull&#39;icona a forma di ingranaggio e selezionare **[!UICONTROL Settings]**.

   ![](assets/salesforce-sync-settings-1.png)

1. In [!UICONTROL Admin Settings] (o &quot;[!UICONTROL My Account]&quot; se non sei un amministratore), fai clic su **[!UICONTROL Salesforce]**.

   ![](assets/salesforce-sync-settings-2.png)

1. Fare clic sulla scheda **[!UICONTROL Sync Settings]**.

   ![](assets/salesforce-sync-settings-3.png)

1. Fare clic sulla freccia accanto a [!UICONTROL Log Email Activity] a [!DNL Salesforce].

   ![](assets/salesforce-sync-settings-4.png)

1. Fare clic sulla scheda **[!UICONTROL Salesforce API]**. In questa scheda è possibile impostare le preferenze per la registrazione delle informazioni su [!DNL Salesforce]. Al termine, fai clic su **[!UICONTROL Save]**.

   ![](assets/salesforce-sync-settings-5.png)

## Registrazione dell&#39;attività e-mail a [!DNL Salesforce] tramite e-mail a [!DNL Salesforce] (CCN) {#logging-email-activity-to-salesforce-via-email-to-salesforce-bcc}

Dopo aver attivato &quot;[!UICONTROL Email to Salesforce (BCC)]&quot;, riceverai un CCN delle e-mail di vendita e le e-mail verranno registrate come attività su opportunità, lead e contatti.

>[!PREREQUISITES]
>
>[!DNL Salesforce] e [!DNL Sales Insight Actions] devono essere connessi.

**Per registrare le e-mail in [!DNL Salesforce] tramite e-mail (CCN)**

1. In Marketo Sales, fare clic sull&#39;icona a forma di ingranaggio e selezionare **[!UICONTROL Settings]**.

   ![](assets/salesforce-sync-settings-6.png)

1. In [!UICONTROL Admin Settings] (o &quot;[!UICONTROL My Account]&quot; se non sei un amministratore), fai clic su **[!UICONTROL Salesforce]**.

   ![](assets/salesforce-sync-settings-7.png)

1. Fare clic sulla scheda **[!UICONTROL Sync Settings]**.

   ![](assets/salesforce-sync-settings-8.png)

1. Fare clic sulla scheda **[!UICONTROL Email to Salesforce (BCC)]** e quindi su **[!UICONTROL Activate]**.

   ![](assets/salesforce-sync-settings-9.png)

Se per qualche motivo l&#39;indirizzo di posta elettronica all&#39;indirizzo [!DNL Salesforce] non viene richiamato, eseguire la procedura seguente per attivare la funzionalità Ccn nell&#39;account [!DNL Salesforce]:

1. Accedi all&#39;istanza [!DNL Salesforce].
1. Trova il tuo nome utente nell’angolo in alto a destra e seleziona la barra a discesa.
1. Seleziona **[!UICONTROL My Settings]**.
1. Seleziona **[!UICONTROL Email]**.
1. Seleziona **[!UICONTROL My Email to Salesforce]**.
1. In questa pagina verrà visualizzato un campo con etichetta &quot;[!UICONTROL Email to Salesforce Address]&quot;. Se accanto a esso non è presente alcun elemento popolato, scorrere verso il basso fino a &quot;[!UICONTROL My Acceptable Email Addresses]&quot;.
1. Immettere gli indirizzi e-mail che si desidera impostare come CCN.
1. Fai clic su **[!UICONTROL Save Changes]**.

**Impossibile trovare il mio indirizzo e-mail a [!DNL Salesforce] nelle mie impostazioni**

Se l&#39;indirizzo di posta elettronica personale a [!DNL Salesforce] non è visualizzato nelle impostazioni, è possibile che l&#39;amministratore non lo abbia abilitato. Ciò può accadere se il tuo team è nuovo di [!DNL Salesforce] o se il tuo team non ha mai utilizzato l&#39;indirizzo Ccn fornito da [!DNL Salesforce].

>[!NOTE]
>
>Per configurare questa impostazione, è necessario disporre dei privilegi di amministratore.

1. Fai clic su **[!UICONTROL Setup]**.
1. Fai clic su **[!UICONTROL Email Administration]**.
1. Fai clic su **[!UICONTROL Email to Salesforce]**.
1. Fai clic su **[!UICONTROL Edit]**.
1. Seleziona la casella accanto a &quot;Attivo&quot;.
1. Fai clic su **[!UICONTROL Save]**.

## Sincronizza [!DNL Sales Insight Actions] attività/promemoria con [!DNL Salesforce] attività {#sync-sales-insight-actions-tasks-reminders-to-salesforce-tasks}

1. In [!DNL Sales Insight Actions], fare clic sull&#39;icona a forma di ingranaggio e selezionare **[!UICONTROL Settings]**.

   ![](assets/salesforce-sync-settings-10.png)

1. In [!UICONTROL Admin Settings] (o &quot;[!UICONTROL My Account]&quot; se non sei un amministratore), fai clic su **[!UICONTROL Salesforce]**.

   ![](assets/salesforce-sync-settings-11.png)

1. Fare clic sulla scheda **[!UICONTROL Sync Settings]**.

   ![](assets/salesforce-sync-settings-12.png)

1. Fare clic sulla freccia accanto a Sincronizza attività/promemoria vendite Marketo con [!DNL Salesforce] attività.

   ![](assets/salesforce-sync-settings-13.png)

1. Scegliere l&#39;opzione desiderata (&quot;Non sincronizzare con [!DNL Salesforce] attività&quot; è selezionata per impostazione predefinita).

   ![](assets/salesforce-sync-settings-14.png)

## È in corso la prima sincronizzazione di [!DNL Sales Insight Actions] attività con [!DNL Salesforce] {#syncing-sales-insight-ations-tasks-with-salesforce-for-the-first-time}

Quando si attiva la sincronizzazione tra [!DNL Sales Insight Actions] e [!DNL Salesforce] attività, le attività [!DNL Salesforce] vengono importate. Non verrà eseguito il push delle attività correnti presenti in [!DNL Sales Insight Actions] a [!DNL Salesforce]. Per ridurre l&#39;ingombro e i duplicati, le uniche attività sincronizzate da [!DNL Sales Insight Actions] in [!DNL Salesforce] sono quelle create dopo la sincronizzazione di [!DNL Sales Insight Actions] con SFDC.

Ecco cosa accade quando si sincronizzano [!DNL Sales Insight Actions] e le attività di SFDC:

Non appena si fa clic su Salva durante la sincronizzazione delle attività, queste vengono sincronizzate. Inizialmente questo richiederà del tempo.

Tutti i promemoria aggiornati o creati nelle ultime 24 ore verranno inseriti da SFDC a [!DNL Sales Insight Actions]. La sincronizzazione è basata sulla data di scadenza e tutte queste attività verranno sincronizzate nel back-end, ma in Centro comandi verranno visualizzate solo le attività in scadenza oggi e domani.

Se la sincronizzazione è stata attivata in precedenza ed è stata eliminata qualsiasi attività in SFDC, qualsiasi elemento eliminato negli ultimi 15 giorni verrà eliminato da Centro comandi.

Le attività verranno sincronizzate costantemente tra [!DNL Sales Insight Actions] e SFDC, purché la sincronizzazione sia abilitata.

Dopo la sincronizzazione iniziale, tutte le attività create, modificate, completate o eliminate in [!DNL Sales Insight Actions] verranno sincronizzate con l&#39;elenco delle attività in [!DNL Salesforce]. E qualsiasi elemento creato, modificato, completato o eliminato in [!DNL Salesforce] aggiornerà l&#39;elenco delle attività in [!DNL Sales Insight Actions].

Per attivare questa sincronizzazione, selezionare la casella di sincronizzazione nella pagina [!UICONTROL Settings] dell&#39;applicazione Web.
