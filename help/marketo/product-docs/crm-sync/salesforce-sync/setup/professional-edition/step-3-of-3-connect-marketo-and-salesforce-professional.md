---
unique-page-id: 3571800
description: Passaggio 3 di 3 - Connessione di Marketo e Salesforce (Professional) - Documentazione di Marketo - Documentazione del prodotto
title: Passaggio 3 di 3 - Connessione di Marketo e Salesforce (Professional)
exl-id: a35e22ef-6378-45e0-be7e-687b0832ecf3
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 0%

---

# Passaggio 3 di 3: collegare Marketo e Salesforce (Professional) {#step-of-connect-marketo-and-salesforce-professional}

In questo articolo configurerai Marketo per la sincronizzazione con l’istanza Salesforce configurata.

>[!PREREQUISITES]
>
>* [Passaggio 1 di 3: aggiunta di campi Marketo a Salesforce (Professional)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-1-of-3-add-marketo-fields-to-salesforce-professional.md)
>* [Passaggio 2 di 3: creare un utente Salesforce per Marketo (Professional)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md)

## Recupera token di sicurezza utente di sincronizzazione {#retrieve-sync-user-security-token}

>[!TIP]
>
>Se disponi già del token di sicurezza, passa direttamente a Imposta credenziali utente e kudo di sincronizzazione per la preparazione.

1. Accedi a Salesforce con l’utente Marketo Sync, fai clic sul nome dell’utente Sync, quindi **Le mie impostazioni**.

   ![](assets/image2015-5-21-14-3a11-3a17.png)

1. Nella barra di ricerca di navigazione, digita &quot;reset&quot; e fai clic su **Reimposta il token di sicurezza**.

   ![](assets/image2014-12-9-9-3a52-3a42.png)

1. Clic **Ripristina token di sicurezza**.

   ![](assets/image2015-5-21-14-3a13-3a5.png)

   Il token di sicurezza ti verrà inviato via e-mail.

## Imposta credenziali utente di sincronizzazione {#set-sync-user-credentials}

1. In Marketo, vai a **Amministratore**, seleziona **CRM** e fai clic su **Sincronizza con [Salesforce.com](https://Salesforce.com)**.

   ![](assets/image2014-12-9-9-3a52-3a58.png)

   >[!NOTE]
   >
   >Assicurati di [nascondi tutti i campi non necessari](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync.md) in Marketo dall’utente di sincronizzazione prima di fare clic su **Sincronizza campi**. Dopo aver fatto clic su Sincronizza campi, tutti i campi visualizzati dall&#39;utente verranno creati in Marketo in modo permanente e non potranno essere eliminati.

1. Immetti le credenziali utente di sincronizzazione Salesforce create nella parte 2 della configurazione Salesforce ([Professionale](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md), [Enterprise](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md) e fai clic su **Sincronizza campi**.

   ![](assets/image2014-12-9-9-3a53-3a8.png)

   >[!NOTE]
   >
   >Verifica **Sandbox** se stai sincronizzando una Sandbox Marketo in una Sandbox Salesforce.

1. Leggi l’avviso, quindi fai clic su **Conferma credenziali**.

   ![](assets/image2014-12-9-9-3a53-3a16.png)

   >[!CAUTION]
   >
   >Se si desidera controllare il [mappature e personalizzarle](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/edit-initial-field-mappings.md), questa è la tua unica occasione per farlo! Dopo aver fatto clic su Avvia Salesforce Sync, l&#39;operazione è completata.

## Avvia Salesforce Sync {#start-salesforce-sync}

1. Clic **Avvia Salesforce Sync** per avviare la sincronizzazione permanente Marketo-Salesforce.

   ![](assets/image2014-12-9-9-3a53-3a24.png)

   >[!CAUTION]
   >
   >Marketo non esegue la deduplicazione automatica in base a una sincronizzazione Salesforce o quando si immettono manualmente i lead.

1. Clic **Avvia sincronizzazione**.

   ![](assets/image2014-12-9-9-3a53-3a32.png)

   >[!NOTE]
   >
   >Il tempo necessario per completare la sincronizzazione iniziale varia a seconda delle dimensioni e della complessità del database.

## Verifica sincronizzazione {#verify-sync}

Marketo fornisce messaggi di stato per la sincronizzazione Salesforce nell’area Amministratore. Per verificare che la sincronizzazione funzioni correttamente, segui la procedura riportata di seguito.

1. In Marketo, fai clic su **Amministratore**, quindi **Salesforce**.

   ![](assets/image2014-12-9-9-3a53-3a40.png)

1. Lo stato di sincronizzazione è visibile nell&#39;angolo superiore destro. Verrà visualizzato uno dei tre messaggi seguenti: **Ultima sincronizzazione**, **Sincronizzazione in corso**, o **Non riuscito**.

   ![](assets/image2014-12-9-9-3a53-3a50.png)

   ![](assets/image2014-12-9-9-3a54-3a4.png)

   ![](assets/image2014-12-9-9-3a54-3a35.png)

Wow, hai appena finito di configurare una delle funzionalità più potenti di Marketo, vai!

>[!MORELIKETHIS]
>
>* [Installare il pacchetto Marketo Sales Insight nell’AppExchange di Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)
>* [Configurare Marketo Sales Insight in Salesforce Professional Edition](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md)
