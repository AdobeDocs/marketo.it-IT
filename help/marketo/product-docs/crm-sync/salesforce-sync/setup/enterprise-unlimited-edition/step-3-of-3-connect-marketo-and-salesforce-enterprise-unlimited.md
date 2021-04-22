---
unique-page-id: 2360366
description: 'Passaggio 3 di 3: collegare Marketo e Salesforce (Enterprise/Unlimited) - Marketo Docs - Documentazione del prodotto'
title: 'Passaggio 3 di 3: collegare Marketo e Salesforce (Enterprise/Unlimited)'
exl-id: ef74bc53-9dc9-43c7-a9aa-565463fdd2e5
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 0%

---

# Passaggio 3 di 3: Connetti Marketo e Salesforce (Enterprise/Senza limiti) {#step-of-connect-marketo-and-salesforce-enterprise-unlimited}

In questo articolo, configurerai Marketo per la sincronizzazione con la tua istanza Salesforce configurata.

>[!PREREQUISITES]
>
>* [Passaggio 1 di 3: Aggiungi campi Marketo a Salesforce (Enterprise/Senza limiti)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [Passaggio 2 di 3: Creare un utente Salesforce per Marketo (Enterprise/Senza limiti)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)


## Recupera il token di sicurezza dell&#39;utente di sincronizzazione {#retrieve-sync-user-security-token}

>[!TIP]
>
>Se disponi già del token di sicurezza, procedi direttamente a Imposta credenziali utente e servizi di sincronizzazione per la preparazione!

1. Accedi a Salesforce con l&#39;utente di sincronizzazione Marketo, fai clic sul nome dell&#39;utente di sincronizzazione, quindi **Impostazioni personali**.

   ![](assets/image2015-6-12-9-3a12-3a47.png)

1. Nella ricerca rapida, digita &quot;reset&quot; e fai clic su **Reset My Security Token**.

   ![](assets/image2015-6-12-9-3a13-3a39.png)

1. Fai clic su **Ripristina token di sicurezza**.

   ![](assets/image2014-12-9-9-3a52-3a50.png)

   Il token di sicurezza ti verrà inviato tramite e-mail.

## Imposta credenziali utente di sincronizzazione {#set-sync-user-credentials}

1. In Marketo, vai su **Amministratore**, seleziona **CRM** e fai clic su **Sincronizza con [Salesforce.com](https://Salesforce.com)**

   ![](assets/image2014-12-9-9-3a52-3a58.png)

   >[!NOTE]
   >
   >Prima di fare clic su **Campi di sincronizzazione**, assicurarsi di [nascondere dall&#39;utente di sincronizzazione tutti i campi di cui non si ha bisogno](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-field-sync/hide-a-salesforce-field-from-the-marketo-sync.md) in Marketo. Una volta fatto clic su Campi di sincronizzazione, tutti i campi che l’utente può visualizzare verranno creati in Marketo in modo permanente e non possono essere eliminati.

1. Immetti le credenziali utente Salesforce Sync create nella parte 2 della configurazione Salesforce ([Professional](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md), [Enterprise](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)) e fai clic su **Sincronizza campi**.

   ![](assets/image2014-12-9-9-3a53-3a8.png)

   >[!NOTE]
   >
   >Seleziona **Sandbox** se stai sincronizzando una Sandbox Marketo con una Sandbox Salesforce.

1. Leggere l&#39;avviso, quindi fare clic su **Conferma credenziali**.

   ![](assets/image2014-12-9-9-3a53-3a16.png)

   >[!CAUTION]
   >
   >Se desideri controllare le mappature [e personalizzarle](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/edit-initial-field-mappings.md), questa è la tua unica possibilità! Dopo aver fatto clic su Avvia sincronizzazione Salesforce, questa operazione viene eseguita.

## Avvia sincronizzazione Salesforce {#start-salesforce-sync}

1. Fai clic su **Avvia sincronizzazione Salesforce** per avviare la sincronizzazione Marketo-Salesforce permanente.

   ![](assets/image2014-12-9-9-3a53-3a24.png)

   >[!CAUTION]
   >
   >Marketo non eseguirà la deduplicazione automatica contro una sincronizzazione Salesforce o quando immetti manualmente i lead.

1. Fare clic su **Avvia sincronizzazione**.

   ![](assets/image2014-12-9-9-3a53-3a32.png)

   >[!NOTE]
   >
   >Il tempo necessario per completare la sincronizzazione iniziale varia a seconda delle dimensioni e della complessità del database.

## Verifica sincronizzazione {#verify-sync}

Marketo fornisce messaggi di stato per la sincronizzazione Salesforce nell’area Amministratore. Per verificare che la sincronizzazione funzioni correttamente, segui questi passaggi.

1. In Marketo, fai clic su **Amministratore**, quindi su **Salesforce**.

   ![](assets/image2014-12-9-9-3a53-3a40.png)

1. Lo stato di sincronizzazione è visibile nell’angolo in alto a destra. Verrà visualizzato uno dei tre messaggi seguenti: **Ultima sincronizzazione**, **Sincronizzazione in corso** o **Non riuscita**.

   ![](assets/image2014-12-9-9-3a53-3a50.png)

   ![](assets/image2014-12-9-9-3a54-3a4.png)

   ![](assets/image2014-12-9-9-3a54-3a35.png)

Wow, hai appena finito di configurare una delle caratteristiche più potenti di Marketo, vai!

>[!MORELIKETHIS]
>
>* [Passaggio 1 di 3: Aggiungi campi Marketo a Salesforce (Enterprise/Senza limiti)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [Passaggio 2 di 3: Creare un utente Salesforce per Marketo (Enterprise/Senza limiti)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
>* [Installa il pacchetto Marketo Sales Insight in Salesforce AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)
>* [Configurare Marketo Sales Insight in Salesforce Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)

