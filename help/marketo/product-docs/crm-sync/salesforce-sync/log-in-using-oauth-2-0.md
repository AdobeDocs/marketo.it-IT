---
description: Accedi con OAuth 2.0 - Documentazione Marketo - Documentazione del prodotto
title: Accedere utilizzando OAuth 2.0
exl-id: 0a70505d-d2b8-4dc9-ad11-decc86588f7f
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '491'
ht-degree: 3%

---

# Accedere utilizzando OAuth 2.0 {#log-in-using-oauth-2-0}

Salesforce utilizza il protocollo OAuth per consentire agli utenti delle applicazioni di accedere in modo sicuro (autenticare l’applicazione utilizzando OAuth 2.0) ai dati senza dover rivelare le credenziali di accesso. Di seguito sono riportati i passaggi da eseguire per collegare e sincronizzare in modo sicuro Marketo Engage con Salesforce.

>[!IMPORTANT]
>
>Per connettere Marketo e [!DNL Salesforce] tramite OAuth, accedi a Marketo tramite un browser privato (in incognito) per evitare di connetterti a [!DNL Salesforce] con un nome utente errato.

## Configurare l’app connessa {#set-up-connected-app}

1. In Salesforce, in Configurazione, all&#39;interno di Strumenti Platform, passa ad App, App Manager e fai clic su **[!UICONTROL New Connected App]**.

   ![](assets/setting-up-oauth-2-1.png)

1. Immettere i dettagli e fare clic su **[!UICONTROL Save]**.

   ![](assets/setting-up-oauth-2-2.png)

1. Selezionare la casella di controllo **[!UICONTROL Enable OAuth Settings]**. Per l&#39;URL di richiamata, immettere `https://app.marketo.com/salesforce/getSfdcOAuthTokensRedirect`. Selezionare tutti gli ambiti OAuth disponibili e fare clic su **[!UICONTROL Add]**.

   ![](assets/setting-up-oauth-2-3.png)

1. Fai clic su **[!UICONTROL Save]**.

   ![](assets/setting-up-oauth-2-4.png)

1. Fai clic su **[!UICONTROL Continue]**.

   ![](assets/setting-up-oauth-2-5.png)

1. Copia la chiave del consumatore e il segreto del consumatore (saranno necessari in seguito per l’utilizzo in Marketo Engage).

   ![](assets/setting-up-oauth-2-6.png)

>[!CAUTION]
>
>Mentre si trova ancora nella pagina Nuova app connessa, scorri verso il basso e assicurati che la casella di controllo &quot;Require Proof Key for Code Exchange (PKCE)&quot; (Richiedi chiave di prova per scambio codice) sia selezionata _NOT_, in quanto interferirebbe con la configurazione.

## Configurare Marketo {#set-up-marketo}

>[!PREREQUISITES]
>
>* L&#39;accesso API deve essere abilitato per l&#39;utente di Salesforce Sync (se sei un utente di Salesforce Professional Edition, tale accesso non è disponibile per impostazione predefinita, contatta il tuo Salesforce Account Executive).
>* L&#39;utente di Marketo Sync deve essere creato in Salesforce.
>* Per i clienti esistenti, la funzione &quot;Abilita OAuth per la sincronizzazione con SFDC&quot; è abilitata nell’abbonamento del cliente.
>* Blocchi popup disattivati.
>* L&#39;app connessa è stata creata e sono disponibili [!UICONTROL Consumer Key] e [!UICONTROL Consumer Secret].

>[!CAUTION]
>
>Prima di fare clic su **[!UICONTROL Sync Fields]**, accertarsi di nascondere all&#39;utente di sincronizzazione tutti i campi non necessari in Marketo. Dopo aver fatto clic su Sincronizza campi, tutti i campi che l’utente può visualizzare in SFDC verranno creati in Marketo in modo permanente e non potranno essere eliminati.

1. Nella sezione Amministrazione di Marketo, fare clic su **[!UICONTROL CRM]**, quindi su **[!UICONTROL Sync with Salesforce]**.

   ![](assets/setting-up-oauth-2-7.png)

1. Aggiungi la chiave del consumatore e le informazioni sul segreto del consumatore registrate in precedenza e fai clic su e **[!UICONTROL Save]**.

   ![](assets/setting-up-oauth-2-8.png)

1. Nella pagina di sincronizzazione di Marketo Salesforce fare clic sul pulsante **[!UICONTROL Login with Salesforce]**.

   ![](assets/setting-up-oauth-2-9.png)

   >[!CAUTION]
   >
   >Se vedi campi Nome utente/Password/Token e non un pulsante &quot;Accedi con Salesforce&quot;, l’abbonamento Marketo è abilitato per l’autenticazione di base. Fare riferimento a [Configurazione di Marketo con autenticazione di base](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md){target="_blank"}. Una volta che la sincronizzazione inizia con un set di credenziali, non si passa da una credenziale di Salesforce all’altra o all’abbonamento. Per configurare Oauth 2.0 per l&#39;autenticazione Salesforce, contattare il [Supporto Marketo](https://nation.marketo.com/t5/support/ct-p/Support).

1. Viene visualizzato un pop-up con la pagina di accesso di Salesforce. Inserisci le credenziali &quot;Utente di Marketo Sync&quot; e accedi.

   ![](assets/setting-up-oauth-2-10.png)

1. Immettere il codice di verifica ricevuto tramite e-mail (inviato da Salesforce) e fare clic su **[!UICONTROL Verify]**.

   ![](assets/setting-up-oauth-2-11.png)

1. Una volta completata la verifica, viene visualizzata la pagina di accesso che richiede l’accesso. Fai clic su **[!UICONTROL Allow]**.

   ![](assets/setting-up-oauth-2-12.png)

1. Tra pochi minuti verrà visualizzato un pop-up in Marketo. Fai clic su **[!UICONTROL Confirm Credentials]**.

   ![](assets/setting-up-oauth-2-13.png)

1. Al termine della sincronizzazione dei campi, fare clic su **[!UICONTROL Start Salesforce Sync]**.

   ![](assets/setting-up-oauth-2-14.png)

1. Fai clic su **[!UICONTROL Start Sync]**.

   ![](assets/setting-up-oauth-2-15.png)

La sincronizzazione tra Marketo e [!DNL Salesforce] è in corso.

![](assets/setting-up-oauth-2-16.png)

>[!MORELIKETHIS]
>
>* [Passaggio 1 di 3: aggiunta di campi Marketo a Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md){target="_blank"}
>* [Passaggio 2 di 3: creazione di un utente Salesforce per Marketo (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"}
>* [Installa il pacchetto Marketo Sales Insight in Salesforce AppExchange](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}
>* [Configurare Marketo Sales Insight in Salesforce Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md){target="_blank"}
