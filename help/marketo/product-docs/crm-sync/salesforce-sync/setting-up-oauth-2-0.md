---
description: Configurazione di OAuth 2.0 - Documenti Marketo - Documentazione del prodotto
title: Configurazione di OAuth 2.0
translation-type: tm+mt
source-git-commit: 2d03d93e120c8b3ce359c6aca44730cfa7c16bf9
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---


# Configurazione di OAuth 2.0 {#setting-up-oauth-2-0}

Salesforce utilizza il protocollo OAuth per consentire agli utenti delle applicazioni di accedere in modo sicuro (autenticare l’applicazione utilizzando OAuth 2.0) ai dati tramite le chiamate API REST senza dover rivelare le credenziali di accesso. Di seguito sono riportati i passaggi da eseguire per collegare e sincronizzare in modo sicuro Marketo con Salesforce.

## Configurazione app connessa {#set-up-connected-app}

1. In Salesforce, in Configurazione, in Strumenti piattaforma, passa a App, App Manager e fai clic su **Nuova app connessa**.

   ![](assets/setting-up-oauth-2-1.png)

1. Compila i dettagli e fai clic su **Salva**.

   ![](assets/setting-up-oauth-2-2.png)

1. Fai clic sulla casella di controllo **Abilita impostazioni OAuth** . Per URL di callback, immetti `https://app.marketo.com/salesforce/getSfdcOAuthTokensRedirect`. Seleziona tutti gli ambiti OAuth disponibili e fai clic su **Aggiungi**.

   ![](assets/setting-up-oauth-2-3.png)

1. Fare clic su **Salva**.

   ![](assets/setting-up-oauth-2-4.png)

1. Fare clic su **Continua**.

   ![](assets/setting-up-oauth-2-5.png)

1. Copia la chiave del consumatore e il segreto del consumatore.

   ![](assets/setting-up-oauth-2-6.png)

>[!NOTE]
>
>Salva le informazioni relative alla chiave del consumatore e al segreto di consumo per un uso successivo in Marketo.

## Imposta Marketo {#set-up-marketo}

>[!PREREQUISITES]
>
>* L’accesso API deve essere abilitato per l’utente Salesforce Sync (se sei un utente Salesforce Professional Edition, tale accesso non è disponibile per impostazione predefinita). Contatta il tuo Account Executive di Salesforce.
>* L’utente di Marketo Sync deve essere creato in Salesforce.
>* Per i clienti esistenti, l’opzione &quot;Abilita sincronizzazione OAuth&quot; è abilitata nell’abbonamento del cliente.
>* I blocchi pop-up sono disabilitati.
>* Viene creata l’app connessa e sono disponibili per l’uso la chiave del consumatore e il segreto del consumatore.


1. Nella sezione Amministratore Marketo, fai clic su **CRM**, quindi su **Sincronizza con Salesforce**.

   ![](assets/setting-up-oauth-2-7.png)

1. Aggiungi la chiave del consumatore e le informazioni del segreto di consumo registrate in precedenza e fai clic su e **Salva**.

   ![](assets/setting-up-oauth-2-8.png)

1. Nella pagina di sincronizzazione di Marketo Salesforce, fai clic sul pulsante **Accedi con Salesforce** .

   ![](assets/setting-up-oauth-2-9.png)

1. Verrà visualizzato un pop-up con la pagina di accesso di Salesforce. Immetti la chiave nelle tue credenziali &quot;Utente sincronizzazione Marketo&quot; e accedi.

   ![](assets/setting-up-oauth-2-10.png)

1. Immetti il codice di verifica ricevuto tramite e-mail (inviato da Salesforce) e fai clic su **Verifica**.

   ![](assets/setting-up-oauth-2-11.png)

1. Dopo la verifica, viene visualizzata la pagina di accesso che richiede l’accesso. Fare clic su **Consenti**.

   ![](assets/setting-up-oauth-2-12.png)

1. In pochi minuti apparirà un pop-up in Marketo. Fare clic su **Conferma credenziali**.

   ![](assets/setting-up-oauth-2-13.png)

1. Al termine della sincronizzazione dei campi, fai clic su **Avvia sincronizzazione Salesforce**.

   ![](assets/setting-up-oauth-2-14.png)

1. Fare clic su **Avvia sincronizzazione**.

   ![](assets/setting-up-oauth-2-15.png)

La sincronizzazione tra Marketo e Salesforce è in corso.

![](assets/setting-up-oauth-2-16.png)
