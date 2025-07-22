---
unique-page-id: 18317669
description: Impostazioni di sincronizzazione Salesforce - Documentazione Marketo - Documentazione del prodotto
title: Impostazioni sincronizzazione Salesforce
exl-id: 024c60ac-569f-4051-9eee-1e8d00f7296c
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 2%

---

# Impostazioni sincronizzazione Salesforce {#salesforce-sync-settings}

## Registrazione dell’attività e-mail in Salesforce tramite API {#logging-email-activity-to-salesforce-via-api}

Questa funzionalità richiede di essere nell’edizione Enterprise/Unlimited di Salesforce o nell’edizione Professional se hai acquistato Integration tramite API di servizi Web.

>[!PREREQUISITES]
>
>Salesforce e Sales Connect devono essere connessi.

1. In [!DNL Sales Connect], fare clic sull&#39;icona ingranaggio in alto a destra e selezionare **[!UICONTROL Settings]**.

   ![](assets/one-2.png)

1. In [!UICONTROL My Account] ([!UICONTROL Admin Settings] se sei un amministratore), fai clic su **[!UICONTROL Salesforce]**.

   ![](assets/two-2.png)

1. Fare clic sulla scheda **[!UICONTROL Sync Settings]**.

   ![](assets/three-1.png)

1. Fare clic sulla freccia accanto a Registra attività e-mail in [!DNL Salesforce].

   ![](assets/four-1.png)

1. Fare clic sulla scheda **[!UICONTROL Salesforce API]**. In questa scheda è possibile impostare le preferenze per la registrazione delle informazioni su [!DNL Salesforce]. Al termine, fai clic su **[!UICONTROL Save]**.

   ![](assets/five.png)

## Registrazione dell’attività e-mail a Salesforce tramite e-mail a Salesforce (BCC) {#logging-email-activity-to-salesforce-via-email-to-salesforce-bcc}

Dopo aver attivato &quot;E-mail a Salesforce (CCN)&quot;, riceverai un CCN delle e-mail di vendita e le e-mail verranno registrate come attività su opportunità, lead e contatti.

>[!PREREQUISITES]
>
>[!DNL Salesforce] e [!DNL Sales Connect] devono essere connessi.

**Per registrare le e-mail in Salesforce tramite e-mail (CCN)**

1. In [!UICONTROL Sales Connect], fare clic sull&#39;icona ingranaggio in alto a destra e selezionare **[!UICONTROL Settings]**.

   ![](assets/one-3.png)

1. In [!UICONTROL My Account] ([!UICONTROL Admin Settings] se sei un amministratore), fai clic su **[!UICONTROL Salesforce]**.

   ![](assets/two-3.png)

1. Fare clic sulla scheda **[!UICONTROL Sync Settings]**.

   ![](assets/three-1.png)

1. Fare clic sulla scheda **[!UICONTROL Email to Salesforce (BCC)]** e quindi su **[!UICONTROL Activate]**.

   ![](assets/six-2.png)

Se per qualche motivo l&#39;indirizzo di posta elettronica all&#39;indirizzo [!DNL Salesforce] non viene richiamato, eseguire la procedura seguente per attivare la funzionalità Ccn nell&#39;account [!DNL Salesforce]:

1. Accedi all&#39;istanza [!DNL Salesforce].
1. Trova il tuo nome utente nell’angolo in alto a destra e seleziona la barra a discesa.
1. Seleziona **[!UICONTROL My Settings]**.
1. Seleziona **[!UICONTROL Email]**.
1. Seleziona **[!UICONTROL My Email to Salesforce]**.
1. In questa pagina viene visualizzato il campo &quot;Email to Salesforce Address&quot; (Invia e-mail a indirizzo). Se non è presente alcun elemento popolato accanto a esso, scorri verso il basso fino a &quot;I miei indirizzi e-mail accettabili&quot;.
1. Immettere gli indirizzi e-mail che si desidera impostare come CCN.
1. Fai clic su **[!UICONTROL Save Changes]**.

**Impossibile trovare il mio indirizzo e-mail a [!DNL Salesforce] nelle mie impostazioni**

Se nelle tue Impostazioni non trovi Il mio indirizzo e-mail a Salesforce, l’amministratore potrebbe non averlo abilitato. Ciò può accadere se il tuo team è nuovo di [!DNL Salesforce] o se il tuo team non ha mai utilizzato l&#39;indirizzo Ccn fornito da [!DNL Salesforce].

>[!NOTE]
>
>Per configurare questa impostazione, è necessario disporre dei privilegi di amministratore.

1. Fai clic su **[!UICONTROL Setup]**.
1. Fai clic su **[!UICONTROL Email Administration]**.
1. Fai clic su **[!UICONTROL Email to Salesforce]**.
1. Fai clic su **[!UICONTROL Edit]**.
1. Selezionare la casella accanto a &quot;[!UICONTROL Active]&quot;.
1. Fai clic su **[!UICONTROL Save]**.

## Sincronizza attività/promemoria vendite con [!DNL Salesforce] attività {#sync-sales-connect-tasks-reminders-to-salesforce-tasks}

1. Fare clic sull&#39;icona a forma di ingranaggio in alto a destra e selezionare **[!UICONTROL Settings]**.

   ![](assets/one-3.png)

1. In [!UICONTROL My Account] ([!UICONTROL Admin Settings] se sei un amministratore), fai clic su **[!UICONTROL Salesforce]**.

   ![](assets/two-2.png)

1. Fare clic sulla scheda **[!UICONTROL Sync Settings]**.

   ![](assets/three-1.png)

1. Fare clic sulla freccia accanto a [!UICONTROL Sync Sales Engage Tasks/Reminders to Salesforce Tasks].

   ![](assets/seven-2.png)

1. Scegliere l&#39;opzione desiderata (&quot;[!UICONTROL Do not sync to Salesforce tasks]&quot; è selezionato per impostazione predefinita).

   ![](assets/eight.png)
