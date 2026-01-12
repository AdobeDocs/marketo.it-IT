---
unique-page-id: 2360366
description: Passaggio 3 di 3 - Connessione di Marketo e Salesforce (Enterprise/Unlimited) - Documentazione di Marketo - Documentazione del prodotto
title: 'Passaggio 3 di 3: connessione di Marketo e Salesforce (Enterprise/Unlimited)'
exl-id: ef74bc53-9dc9-43c7-a9aa-565463fdd2e5
feature: Salesforce Integration
source-git-commit: f27e0d42161161347cc4c774853fb04e7ccecb5c
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 0%

---

# Passaggio 3 di 3: connettere Marketo e [!DNL Salesforce] (Enterprise/Unlimited) {#step-of-connect-marketo-and-salesforce-enterprise-unlimited}

In questo articolo configurerai Marketo per la sincronizzazione con l&#39;istanza [!DNL Salesforce] configurata.

>[!PREREQUISITES]
>
>* [Passaggio 1 di 3: aggiunta di campi Marketo a [!DNL Salesforce] (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [Passaggio 2 di 3: creazione di un  [!DNL Salesforce] utente per Marketo (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)

## Recupera token di sicurezza utente di sincronizzazione {#retrieve-sync-user-security-token}

>[!TIP]
>
>Se disponi già del token di sicurezza, passa direttamente a Imposta credenziali utente e kudo di sincronizzazione per la preparazione.

1. Accedere a [!DNL Salesforce] con l&#39;utente di sincronizzazione di Marketo, fare clic sul nome dell&#39;utente di sincronizzazione, quindi su **[!UICONTROL My Settings]**.

   ![](assets/image2015-6-12-9-3a12-3a47.png)

1. Nella ricerca rapida digitare &quot;reset&quot; e fare clic su **[!UICONTROL Reset My Security Token]**.

   ![](assets/image2015-6-12-9-3a13-3a39.png)

1. Fai clic su **[!UICONTROL Reset Security Token]**.

   ![](assets/image2014-12-9-9-3a52-3a50.png)

   Il token di sicurezza ti verrà inviato via e-mail.

## Imposta credenziali utente di sincronizzazione {#set-sync-user-credentials}

1. In Marketo, vai a **[!UICONTROL Admin]**, seleziona **CRM** e fai clic su **[!UICONTROL Sync with Salesforce.com]**

   ![](assets/image2014-12-9-9-3a52-3a58.png)

   >[!NOTE]
   >
   >Assicurarsi di [nascondere tutti i campi non necessari](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync.md) in Marketo dall&#39;utente sincronizzato prima di fare clic su **[!UICONTROL Sync Fields]**. Dopo aver fatto clic su [!UICONTROL Sync Fields], tutti i campi che l&#39;utente potrà visualizzare verranno creati in Marketo in modo permanente e non potranno essere eliminati.

1. Immettere le credenziali utente di sincronizzazione [!DNL Salesforce] create nella parte 2 della configurazione di [!DNL Salesforce] ([Professional](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md) o [Enterprise](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)) e fare clic su **[!UICONTROL Sync Fields]** (selezionare **[!UICONTROL Sandbox]** solo se si sta sincronizzando una sandbox di Marketo in una sandbox [!DNL Salesforce]).

   ![](assets/image2014-12-9-9-3a53-3a8.png)

   >[!CAUTION]
   >
   >Se viene visualizzato un pulsante &quot;Accedi a [!DNL Salesforce]&quot; invece dei campi Nome utente/Password/Token, la sottoscrizione Marketo è abilitata per OAuth. [fai riferimento a questo articolo](/help/marketo/product-docs/crm-sync/salesforce-sync/log-in-using-oauth-2-0.md). Non appena la sincronizzazione inizia a utilizzare un set di credenziali, **non si passa da [!DNL Salesforce] credenziali a un abbonamento o viceversa**. Se desideri utilizzare l’autenticazione di base, rivolgiti al tuo Account Manager.

1. Leggere l&#39;avviso, quindi fare clic su **[!UICONTROL Confirm Credentials]**.

   ![](assets/image2014-12-9-9-3a53-3a16.png)

   >[!CAUTION]
   >
   >Se vuoi controllare le [mappature e personalizzarle](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/edit-initial-field-mappings.md), questa è la tua unica possibilità! Dopo aver fatto clic su [!UICONTROL Start  Salesforce Sync], l&#39;operazione è completata.

## Avvia sincronizzazione [!DNL Salesforce] {#start-salesforce-sync}

1. Fare clic su **[!UICONTROL Start  Salesforce Sync]** per avviare la sincronizzazione permanente di Marketo-[!DNL Salesforce].

   ![](assets/image2014-12-9-9-3a53-3a24.png)

   >[!CAUTION]
   >
   >Marketo non eseguirà la deduplicazione automatica in base a una sincronizzazione [!DNL Salesforce] o quando si immettono manualmente i lead.

1. Fai clic su **[!UICONTROL Start Sync]**.

   ![](assets/image2014-12-9-9-3a53-3a32.png)

   >[!NOTE]
   >
   >Il tempo necessario per completare la sincronizzazione iniziale varia a seconda delle dimensioni e della complessità del database.

## Verifica sincronizzazione {#verify-sync}

Marketo fornisce messaggi di stato per la sincronizzazione [!DNL Salesforce] nell&#39;area di amministrazione. Per verificare che la sincronizzazione funzioni correttamente, segui la procedura riportata di seguito.

1. In Marketo, fai clic su **[!UICONTROL Admin]**, quindi su **[!UICONTROL Salesforce]**.

   ![](assets/image2014-12-9-9-3a53-3a40.png)

1. Lo stato di sincronizzazione è visibile nell&#39;angolo superiore destro. Verrà visualizzato uno dei tre messaggi seguenti: **[!UICONTROL Last Synced]**, **[!UICONTROL Sync in Progress]** o **[!UICONTROL Failed]**.

   ![](assets/image2014-12-9-9-3a53-3a50.png)

   ![](assets/image2014-12-9-9-3a54-3a4.png)

   ![](assets/image2014-12-9-9-3a54-3a35.png)

Hai appena finito di configurare una delle funzionalità più potenti di Marketo, vai!

>[!MORELIKETHIS]
>
>* [Passaggio 1 di 3: aggiunta di campi Marketo a [!DNL Salesforce] (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [Passaggio 2 di 3: creazione di un  [!DNL Salesforce] utente per Marketo (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
>* [Installa il pacchetto Marketo Sales Insight in [!DNL Salesforce] AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)
>* [Configura Marketo Sales Insight in [!DNL Salesforce] Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)
