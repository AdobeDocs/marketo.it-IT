---
unique-page-id: 3571800
description: Passaggio 3 di 3 - Connessione di Marketo e Salesforce (Professional) - Documentazione di Marketo - Documentazione del prodotto
title: Passaggio 3 di 3 - Connessione di Marketo e Salesforce (Professional)
exl-id: a35e22ef-6378-45e0-be7e-687b0832ecf3
feature: Salesforce Integration
source-git-commit: 756a38ba87dd5af9ee783e9709056d444d4f415b
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# Passaggio 3 di 3: collegare Marketo e Salesforce (Professional) {#step-of-connect-marketo-and-salesforce-professional}

In questo articolo configurerai il Marketo Engage per la sincronizzazione con l’istanza Salesforce configurata.

>[!PREREQUISITES]
>
>* [Passaggio 1 di 3: aggiunta di campi Marketo a Salesforce (Professional)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-1-of-3-add-marketo-fields-to-salesforce-professional.md){target="_blank"}
>* [Passaggio 2 di 3: creazione di un utente Salesforce per Marketo (Professional)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md){target="_blank"}

## Recupera token di sicurezza utente di sincronizzazione {#retrieve-sync-user-security-token}

>[!TIP]
>
>Se disponi già del token di sicurezza, passa direttamente a Imposta credenziali utente e kudo di sincronizzazione per la preparazione.

1. Accedi a Salesforce con l&#39;utente Marketo Sync, fai clic sul nome dell&#39;utente Sync, quindi su **[!UICONTROL Impostazioni personali]**.

   ![](assets/image2015-5-21-14-3a11-3a17.png)

1. Nella barra di ricerca di navigazione, digitare &quot;reset&quot; e fare clic su **[!UICONTROL Reset My Security Token]**.

   ![](assets/image2014-12-9-9-3a52-3a42.png)

1. Fare clic su **[!UICONTROL Reimposta token di sicurezza]**.

   ![](assets/image2015-5-21-14-3a13-3a5.png)

   Il token di sicurezza ti verrà inviato via e-mail.

## Imposta credenziali utente di sincronizzazione {#set-sync-user-credentials}

1. In Marketo, vai a **[!UICONTROL Amministratore]**, seleziona **[!UICONTROL CRM]**, quindi fai clic su **[!UICONTROL Sincronizza con Salesforce.com]**.

   ![](assets/image2014-12-9-9-3a52-3a58.png)

   >[!NOTE]
   >
   >Assicurarsi di [nascondere tutti i campi non necessari](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync.md){target="_blank"} in Marketo dall&#39;utente sincronizzato prima di fare clic su **[!UICONTROL Sincronizza campi]**. Dopo aver fatto clic su Sincronizza campi, tutti i campi visualizzati dall&#39;utente verranno creati in Marketo in modo permanente e non potranno essere eliminati.

1. Immetti le credenziali utente di sincronizzazione Salesforce create nella parte 2 della configurazione Salesforce ([Professional](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md), [Enterprise](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)) e fai clic su **[!UICONTROL Sincronizza campi]**.

   ![](assets/image2014-12-9-9-3a53-3a8.png)

   >[!NOTE]
   >
   >Seleziona **[!UICONTROL Sandbox]** se stai sincronizzando una Sandbox Marketo in una Sandbox Salesforce.

1. Leggi l&#39;avviso, quindi fai clic su **[!UICONTROL Conferma credenziali]**.

   ![](assets/image2014-12-9-9-3a53-3a16.png)

   >[!CAUTION]
   >
   >Se vuoi controllare le [mappature e personalizzarle](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/edit-initial-field-mappings.md){target="_blank"}, questa è la tua unica possibilità! Dopo aver fatto clic su Avvia Salesforce Sync, l&#39;operazione è completata.

## Avvia Salesforce Sync {#start-salesforce-sync}

1. Fare clic su **[!UICONTROL Avvia Salesforce Sync]** per avviare la sincronizzazione permanente Marketo-Salesforce.

   ![](assets/image2014-12-9-9-3a53-3a24.png)

   >[!CAUTION]
   >
   >Marketo non esegue la deduplicazione automatica in base a una sincronizzazione Salesforce o quando si immettono manualmente i lead.

1. Fare clic su **[!UICONTROL Avvia sincronizzazione]**.

   ![](assets/image2014-12-9-9-3a53-3a32.png)

   >[!NOTE]
   >
   >Il tempo necessario per completare la sincronizzazione iniziale varia a seconda delle dimensioni e della complessità del database.

## Verifica sincronizzazione {#verify-sync}

Marketo fornisce messaggi di stato per la sincronizzazione Salesforce nell’area Amministratore. Per verificare che la sincronizzazione funzioni correttamente, segui la procedura riportata di seguito.

1. In Marketo, fai clic su **[!UICONTROL Amministratore]**, quindi su **Salesforce**.

   ![](assets/image2014-12-9-9-3a53-3a40.png)

1. Lo stato di sincronizzazione è visibile nell&#39;angolo superiore destro. Verrà visualizzato uno dei tre messaggi seguenti: **[!UICONTROL Ultima sincronizzazione]**, **[!UICONTROL Sincronizzazione in corso]** o **[!UICONTROL Non riuscita]**.

   ![](assets/image2014-12-9-9-3a53-3a50.png)

   ![](assets/image2014-12-9-9-3a54-3a4.png)

   ![](assets/image2014-12-9-9-3a54-3a35.png)

Hai appena finito di configurare una delle funzionalità più potenti di Marketo, vai!

>[!MORELIKETHIS]
>
>* [Installa il pacchetto Marketo Sales Insight nell&#39;AppExchange Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}
>* [Configurare Marketo Sales Insight in Salesforce Professional Edition](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md){target="_blank"}
