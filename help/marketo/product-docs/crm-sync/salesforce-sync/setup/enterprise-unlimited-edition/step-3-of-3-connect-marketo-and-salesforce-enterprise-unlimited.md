---
unique-page-id: 2360366
description: Passaggio 3 di 3 - Connessione di Marketo e Salesforce (Enterprise/Unlimited) - Documentazione di Marketo - Documentazione del prodotto
title: 'Passaggio 3 di 3: connessione di Marketo e Salesforce (Enterprise/Unlimited)'
exl-id: ef74bc53-9dc9-43c7-a9aa-565463fdd2e5
feature: Salesforce Integration
source-git-commit: 4045f262889d06304111288d30da893529396e81
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 0%

---

# Passaggio 3 di 3: Connessione di Marketo e Salesforce (Enterprise/Unlimited) {#step-of-connect-marketo-and-salesforce-enterprise-unlimited}

In questo articolo configurerai il Marketo Engage per la sincronizzazione con l’istanza Salesforce configurata.

>[!PREREQUISITES]
>
>* [Passaggio 1 di 3: aggiunta di campi Marketo a Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md){target="_blank"}
>* [Passaggio 2 di 3: creare un utente Salesforce per Marketo (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"}

## Recupera token di sicurezza utente di sincronizzazione {#retrieve-sync-user-security-token}

>[!TIP]
>
>Se disponi già del token di sicurezza, passa direttamente a Imposta credenziali utente e kudo di sincronizzazione per la preparazione.

1. Accedi a Salesforce con l’utente Marketo Sync, fai clic sul nome dell’utente Sync, quindi **[!UICONTROL Le mie impostazioni]**.

   ![](assets/image2015-6-12-9-3a12-3a47.png)

1. Nella ricerca rapida digitare &quot;reset&quot; e fare clic su **[!UICONTROL Reimposta il token di sicurezza]**.

   ![](assets/image2015-6-12-9-3a13-3a39.png)

1. Clic **[!UICONTROL Ripristina token di sicurezza]**.

   ![](assets/image2014-12-9-9-3a52-3a50.png)

   Il token di sicurezza ti verrà inviato via e-mail.

## Imposta credenziali utente di sincronizzazione {#set-sync-user-credentials}

1. In Marketo, vai a **[!UICONTROL Amministratore]**, seleziona **[!UICONTROL CRM]** e fai clic su **Sincronizza con [Salesforce.com](https://Salesforce.com)**

   ![](assets/image2014-12-9-9-3a52-3a58.png)

   >[!NOTE]
   >
   >Assicurati di [nascondi tutti i campi non necessari](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/hide-a-salesforce-field-from-the-marketo-sync.md){target="_blank"} in Marketo dall’utente di sincronizzazione prima di fare clic su **[!UICONTROL Sincronizza campi]**. Dopo aver fatto clic su Sincronizza campi, tutti i campi visualizzati dall&#39;utente verranno creati in Marketo in modo permanente e non potranno essere eliminati.

1. Immetti le credenziali utente di sincronizzazione Salesforce create nella parte 2 della configurazione Salesforce ([Professionale](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/professional-edition/step-2-of-3-create-a-salesforce-user-for-marketo-professional.md){target="_blank"} or [Enterprise](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"}) e fai clic su **[!UICONTROL Sincronizza campi]** (spunta **[!UICONTROL Sandbox]** solo se stai sincronizzando una Sandbox Marketo in una Sandbox Salesforce).

   ![](assets/image2014-12-9-9-3a53-3a8.png)

   >[!CAUTION]
   >
   >Se visualizzi un pulsante &quot;Accedi a Salesforce&quot; invece dei campi Nome utente/Password/Token, l’abbonamento Marketo è abilitato per OAuth. Per favore [fai riferimento a questo articolo](/help/marketo/product-docs/crm-sync/salesforce-sync/log-in-using-oauth-2-0.md){target="_blank"}. Non appena la sincronizzazione inizia a utilizzare un set di credenziali, _non vi è alcun cambio di credenziali o abbonamento Salesforce_. Se desideri utilizzare l’autenticazione di base, rivolgiti al team dell’account Adobe (il tuo Account Manager).

1. Leggi l’avviso, quindi fai clic su **[!UICONTROL Conferma credenziali]**.

   ![](assets/image2014-12-9-9-3a53-3a16.png)

   >[!CAUTION]
   >
   >Se si desidera controllare il [mappature e personalizzarle](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/edit-initial-field-mappings.md){target="_blank"}, questa è la tua unica occasione per farlo! Dopo aver fatto clic su Avvia Salesforce Sync, l&#39;operazione è completata.

## Avvia Salesforce Sync {#start-salesforce-sync}

1. Clic **[!UICONTROL Avvia Salesforce Sync]** per avviare la sincronizzazione permanente Marketo-Salesforce.

   ![](assets/image2014-12-9-9-3a53-3a24.png)

   >[!CAUTION]
   >
   >Marketo non esegue la deduplicazione automatica in base a una sincronizzazione Salesforce o quando si immettono manualmente i lead.

1. Clic **[!UICONTROL Avvia sincronizzazione]**.

   ![](assets/image2014-12-9-9-3a53-3a32.png)

   >[!NOTE]
   >
   >Il tempo necessario per completare la sincronizzazione iniziale varia a seconda delle dimensioni e della complessità del database.

## Verifica sincronizzazione {#verify-sync}

Marketo fornisce messaggi di stato per la sincronizzazione Salesforce nell’area Amministratore. Per verificare che la sincronizzazione funzioni correttamente, segui la procedura riportata di seguito.

1. In Marketo, fai clic su **[!UICONTROL Amministratore]**, quindi **Salesforce**.

   ![](assets/image2014-12-9-9-3a53-3a40.png)

1. Lo stato di sincronizzazione è visibile nell&#39;angolo superiore destro. Verrà visualizzato uno dei tre messaggi seguenti: **[!UICONTROL Ultima sincronizzazione]**, **[!UICONTROL Sincronizzazione in corso]**, o **[!UICONTROL Non riuscito]**.

   ![](assets/image2014-12-9-9-3a53-3a50.png)

   ![](assets/image2014-12-9-9-3a54-3a4.png)

   ![](assets/image2014-12-9-9-3a54-3a35.png)

Hai appena finito di configurare una delle funzionalità più potenti di Marketo, vai!

>[!MORELIKETHIS]
>
>* [Passaggio 1 di 3: aggiunta di campi Marketo a Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md){target="_blank"}
>* [Passaggio 2 di 3: creare un utente Salesforce per Marketo (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"}
>* [Installare il pacchetto Marketo Sales Insight nell’AppExchange di Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}
>* [Configurare Marketo Sales Insight in Salesforce Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md){target="_blank"}
