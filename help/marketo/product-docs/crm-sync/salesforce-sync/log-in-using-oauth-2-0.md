---
description: Accedere utilizzando OAuth 2.0 - Documenti Marketo - Documentazione del prodotto
title: Accedere utilizzando OAuth 2.0
exl-id: 0a70505d-d2b8-4dc9-ad11-decc86588f7f
source-git-commit: 88c4e844f7ce26b12bae8177dd5311813fb4adcb
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 0%

---

# Accedere utilizzando OAuth 2.0 {#log-in-using-oauth-2-0}

Salesforce utilizza il protocollo OAuth per consentire agli utenti delle applicazioni di accedere in modo sicuro (autenticare l’applicazione utilizzando OAuth 2.0) ai dati senza dover rivelare le credenziali di accesso. Di seguito sono riportati i passaggi da eseguire per collegare e sincronizzare Marketo in modo sicuro con Salesforce.

>[!IMPORTANT]
>
>Per collegare Marketo e Salesforce utilizzando OAuth, accedi a Marketo tramite browser privato (in incognito) in modo da evitare di connettersi a Salesforce con il nome utente errato.

## Configurazione app connessa {#set-up-connected-app}

1. In Salesforce, in Configurazione, in Strumenti piattaforma, passa a App, App Manager e fai clic su **Nuova app connessa**.

   ![](assets/setting-up-oauth-2-1.png)

1. Compila i dettagli e fai clic su **Salva**.

   ![](assets/setting-up-oauth-2-2.png)

1. Fai clic sul pulsante **Abilita impostazioni OAuth** casella di controllo. Per URL di callback, immetti `https://app.marketo.com/salesforce/getSfdcOAuthTokensRedirect`. Seleziona tutti gli ambiti OAuth disponibili e fai clic su **Aggiungi**.

   ![](assets/setting-up-oauth-2-3.png)

1. Fai clic su **Salva**.

   ![](assets/setting-up-oauth-2-4.png)

1. Fai clic su **Continua**.

   ![](assets/setting-up-oauth-2-5.png)

1. Copia la chiave del consumatore e il segreto del consumatore.

   ![](assets/setting-up-oauth-2-6.png)

>[!NOTE]
>
>Salva le informazioni relative alla chiave del consumatore e al segreto di consumo da utilizzare in futuro in Marketo.

## Configurazione Marketo {#set-up-marketo}

>[!PREREQUISITES]
>
>* L’accesso API deve essere abilitato per l’utente Salesforce Sync (se sei un utente Salesforce Professional Edition, tale accesso non è disponibile per impostazione predefinita). Contatta il tuo Account Executive di Salesforce.
>* È necessario creare l’utente di Marketo Sync in Salesforce.
>* Per i clienti esistenti, l’opzione &quot;Abilita sincronizzazione OAuth&quot; è abilitata nell’abbonamento del cliente.
>* I blocchi pop-up sono disabilitati.
>* Viene creata l’app connessa e sono disponibili per l’uso la chiave del consumatore e il segreto del consumatore.


>[!CAUTION]
>
>Prima di fare clic su , nascondi dall’utente di sincronizzazione tutti i campi di cui non hai bisogno in Marketo **Campi di sincronizzazione**. Dopo aver fatto clic su Campi di sincronizzazione, tutti i campi che l’utente può visualizzare in SFDC verranno creati in Marketo in modo permanente e non possono essere eliminati.

1. Nella sezione Marketo Admin, fai clic su **CRM**, quindi **Sincronizzazione con Salesforce**.

   ![](assets/setting-up-oauth-2-7.png)

1. Aggiungi la chiave del consumatore e le informazioni del segreto del consumatore registrate in precedenza e fai clic su e **Salva**.

   ![](assets/setting-up-oauth-2-8.png)

1. Nella pagina di sincronizzazione di Marketo Salesforce, fai clic sul pulsante **Accedi con Salesforce** pulsante .

   ![](assets/setting-up-oauth-2-9.png)

   >[!CAUTION]
   >
   >Se visualizzi i campi Nome utente/Password/Token e non il pulsante &quot;Accedi con Salesforce&quot;, la sottoscrizione Marketo è abilitata per l&#39;autenticazione di base. Fai riferimento a [Configurazione di Marketo con autenticazione di base](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md). Una volta che la sincronizzazione inizia a utilizzare un set di credenziali, non vi è alcun cambiamento di credenziali Salesforce o sottoscrizione. Se desideri utilizzare Oauth 2.0, contatta il team dell’account Adobe (il tuo Account Manager).

1. Verrà visualizzato un pop-up con la pagina di accesso di Salesforce. Immetti la chiave nelle tue credenziali &quot;Marketo Sync User&quot; e accedi.

   ![](assets/setting-up-oauth-2-10.png)

1. Immetti il codice di verifica ricevuto tramite e-mail (inviato da Salesforce) e fai clic su **Verifica**.

   ![](assets/setting-up-oauth-2-11.png)

1. Dopo la verifica, viene visualizzata la pagina di accesso che richiede l’accesso. Fai clic su **Consenti**.

   ![](assets/setting-up-oauth-2-12.png)

1. In pochi minuti verrà visualizzato un pop-up in Marketo. Fai clic su **Conferma credenziali**.

   ![](assets/setting-up-oauth-2-13.png)

1. Al termine della sincronizzazione dei campi, fai clic su **Avvia sincronizzazione Salesforce**.

   ![](assets/setting-up-oauth-2-14.png)

1. Fai clic su **Avvia sincronizzazione**.

   ![](assets/setting-up-oauth-2-15.png)

La sincronizzazione tra Marketo e Salesforce è in corso.

![](assets/setting-up-oauth-2-16.png)

>[!MORELIKETHIS]
>
>* [Passaggio 1 di 3: Aggiungi campi Marketo a Salesforce (Enterprise/Senza limiti)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [Passaggio 2 di 3: Creare un utente Salesforce per Marketo (Enterprise/Senza limiti)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
>* [Installa il pacchetto Marketo Sales Insight in Salesforce AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md)
>* [Configurare Marketo Sales Insight in Salesforce Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)

