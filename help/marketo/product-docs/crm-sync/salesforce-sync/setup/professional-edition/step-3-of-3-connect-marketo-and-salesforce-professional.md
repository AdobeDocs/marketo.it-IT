---
unique-page-id: 3571800
description: Passaggio 3 di 3 - Connect Marketo e Salesforce (Professional) - Marketo Docs - Documentazione prodotto
title: 'Passaggio 3 di 3: Connect Marketo e Salesforce (Professional)'
translation-type: tm+mt
source-git-commit: 2b5ccd7220557a5e966d33436d0f0d2a65e4589d
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 0%

---


# Passaggio 3 di 3: Connect Marketo e Salesforce (Professional) {#step-of-connect-marketo-and-salesforce-professional}

In questo articolo, configurerai Marketo per la sincronizzazione con la tua istanza Salesforce configurata.

>[!PREREQUISITES]
>
>* [Passaggio 1 di 3: Aggiunta di campi Marketo a Salesforce (Professional)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-1-of-3-add-marketo-fields-to-salesforce-professional.md)
>* [Passaggio 2 di 3: Creare un utente Salesforce per Marketo (Professional)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md)


## Recuperare il token di sicurezza per la sincronizzazione degli utenti {#retrieve-sync-user-security-token}

>[!TIP]
>
>Se disponete già del token di sicurezza, passate direttamente a Set Sync User Credentials and kudos for preparations (Imposta credenziali utente sincronizzazione).

1. Accedi a Salesforce con l&#39;utente di sincronizzazione Marketo, fai clic sul nome dell&#39;utente di sincronizzazione, quindi **My Settings**.

   ![](assets/image2015-5-21-14-3a11-3a17.png)

1. Nella barra di ricerca della navigazione, digitate &quot;reset&quot; e fate clic su **Reimposta token di protezione personale**.

   ![](assets/image2014-12-9-9-3a52-3a42.png)

1. Fare clic su **Reimposta token di protezione**.

   ![](assets/image2015-5-21-14-3a13-3a5.png)

   Il token di protezione verrà inviato via e-mail.

## Imposta credenziali utente sincronizzazione {#set-sync-user-credentials}

1. In Marketo, andare su **Admin**, selezionare **CRM**, quindi fare clic su **Sincronizza con [Salesforce.com](https://Salesforce.com)**.

   ![](assets/image2014-12-9-9-3a52-3a58.png)

   >[!NOTE]
   >
   >Assicurarsi di [nascondere tutti i campi non necessari](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-field-sync/hide-a-salesforce-field-from-the-marketo-sync.md) in Marketo dall&#39;utente di sincronizzazione prima di fare clic su **Sincronizza campi**. Dopo aver fatto clic su Sincronizza campi, tutti i campi che l&#39;utente può visualizzare verranno creati in Marketo in modo permanente e non potranno essere eliminati.

1. Immettete le credenziali Utente sincronizzazione Salesforce create nella parte 2 della configurazione Salesforce ([Professional](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md), [Enterprise](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) e fate clic su **Sincronizza campi**.

   ![](assets/image2014-12-9-9-3a53-3a8.png)

   >[!NOTE]
   >
   >Selezionare **Sandbox** se si sta sincronizzando una sandbox Marketo con una sandbox Salesforce.

1. Leggere l&#39;avviso, quindi fare clic su **Conferma credenziali**.

   ![](assets/image2014-12-9-9-3a53-3a16.png)

   >[!CAUTION]
   >
   >Se si desidera esaminare le mappature [e personalizzarle](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/edit-initial-field-mappings.md), questa è l&#39;unica possibilità! Dopo aver fatto clic su Avvia sincronizzazione Salesforce, questa operazione viene completata.

## Avvia sincronizzazione Salesforce {#start-salesforce-sync}

1. Fai clic su **Avvia sincronizzazione Salesforce** per avviare la sincronizzazione persistente tra Marketing e Salesforce.

   ![](assets/image2014-12-9-9-3a53-3a24.png)

   >[!CAUTION]
   >
   >Marketo non eseguirà automaticamente la deduplicazione rispetto a una sincronizzazione Salesforce, o quando immetti manualmente i lead.

1. Fare clic su **Avvia sincronizzazione**.

   ![](assets/image2014-12-9-9-3a53-3a32.png)

   >[!NOTE]
   >
   >Il tempo necessario per completare la sincronizzazione iniziale varia a seconda delle dimensioni e della complessità del database.

## Verifica sincronizzazione {#verify-sync}

Marketo fornisce messaggi di stato per la sincronizzazione Salesforce nell&#39;area Admin. Per verificare che la sincronizzazione funzioni correttamente, effettuate le seguenti operazioni.

1. In Marketo, fare clic su **Admin**, quindi su **Salesforce**.

   ![](assets/image2014-12-9-9-3a53-3a40.png)

1. Lo stato di sincronizzazione è visibile nell&#39;angolo superiore destro. Verrà visualizzato uno dei tre messaggi seguenti: **Ultima sincronizzazione**, **Sincronizzazione in corso** o **Non riuscita**.

   ![](assets/image2014-12-9-9-3a53-3a50.png)

   ![](assets/image2014-12-9-9-3a54-3a4.png)

   ![](assets/image2014-12-9-9-3a54-3a35.png)

Wow, hai appena finito di configurare una delle caratteristiche più potenti di Marketo, vai!

>[!MORELIKETHIS]
>
>* [Installazione del pacchetto marketing Sales Insight in Salesforce  AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)
>* [Configurare Marketing Sales Insight in Salesforce Professional Edition](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md)

