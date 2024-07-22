---
description: Accedi con OAuth 2.0 - Documentazione Marketo - Documentazione del prodotto
title: Accedi con OAuth 2.0
exl-id: 0a70505d-d2b8-4dc9-ad11-decc86588f7f
feature: Salesforce Integration
source-git-commit: 4045f262889d06304111288d30da893529396e81
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 0%

---

# Accedi con OAuth 2.0 {#log-in-using-oauth-2-0}

Salesforce utilizza il protocollo OAuth per consentire agli utenti delle applicazioni di accedere in modo sicuro (autenticare l’applicazione utilizzando OAuth 2.0) ai dati senza dover rivelare le credenziali di accesso. Di seguito sono riportati i passaggi da eseguire per collegare e sincronizzare in modo sicuro il Marketo Engage con Salesforce.

>[!IMPORTANT]
>
>Per collegare Marketo e Salesforce tramite OAuth, accedi a Marketo tramite un browser privato (in incognito) per evitare di connetterti a Salesforce con un nome utente errato.

## Configurare l’app connessa {#set-up-connected-app}

1. In Salesforce, in Configurazione, in Strumenti Platform, passa ad App, App Manager e fai clic su **[!UICONTROL Nuova app connessa]**.

   ![](assets/setting-up-oauth-2-1.png)

1. Inserisci i dettagli e fai clic su **[!UICONTROL Salva]**.

   ![](assets/setting-up-oauth-2-2.png)

1. Selezionare la casella di controllo **[!UICONTROL Abilita impostazioni OAuth]**. Per l&#39;URL di richiamata, immettere `https://app.marketo.com/salesforce/getSfdcOAuthTokensRedirect`. Seleziona tutti gli ambiti OAuth disponibili e fai clic su **[!UICONTROL Aggiungi]**.

   ![](assets/setting-up-oauth-2-3.png)

1. Fai clic su **[!UICONTROL Salva]**.

   ![](assets/setting-up-oauth-2-4.png)

1. Fai clic su **[!UICONTROL Continua]**.

   ![](assets/setting-up-oauth-2-5.png)

1. Copia la chiave del consumatore e il segreto del consumatore (saranno necessari in seguito per l&#39;utilizzo in Marketo Engage).

   ![](assets/setting-up-oauth-2-6.png)

>[!CAUTION]
>
>Mentre si trova ancora nella pagina Nuova app connessa, scorri verso il basso e assicurati che la casella di controllo &quot;Require Proof Key for Code Exchange (PKCE)&quot; (Richiedi chiave di prova per scambio codice) sia selezionata _NOT_, in quanto interferirebbe con la configurazione.

## Configurare Marketo {#set-up-marketo}

>[!PREREQUISITES]
>
>* L’accesso API deve essere abilitato per l’utente Salesforce Sync (se sei un utente Salesforce Professional Edition, tale accesso non è disponibile per impostazione predefinita, contatta il tuo Account Executive Salesforce).
* L&#39;utente di Marketo Sync deve essere creato in Salesforce.
* Per i clienti esistenti, la funzione &quot;Abilita OAuth per la sincronizzazione SFDC&quot; è abilitata nell’abbonamento del cliente.
* Blocchi popup disattivati.
* L’app connessa viene creata e abbiamo la chiave consumer e il segreto consumer sono disponibili per l’uso.

>[!CAUTION]
>
Prima di fare clic su **[!UICONTROL Sincronizza campi]**, accertati di nascondere all&#39;utente di Marketo tutti i campi non necessari. Dopo aver fatto clic su Sincronizza campi, tutti i campi che l&#39;utente può visualizzare in SFDC verranno creati in Marketo in modo permanente e non potranno essere eliminati.

1. Nella sezione Amministratore Marketo, fai clic su **[!UICONTROL CRM]**, quindi su **[!UICONTROL Sincronizza con Salesforce]**.

   ![](assets/setting-up-oauth-2-7.png)

1. Aggiungi la chiave del consumatore e le informazioni sul segreto del consumatore registrate in precedenza e fai clic su e **[!UICONTROL Salva]**.

   ![](assets/setting-up-oauth-2-8.png)

1. Nella pagina di sincronizzazione di Marketo Salesforce, fai clic sul pulsante **[!UICONTROL Accedi con Salesforce]**.

   ![](assets/setting-up-oauth-2-9.png)

   >[!CAUTION]
   >
   Se visualizzi i campi Nome utente/Password/Token e non un pulsante &quot;Accedi con Salesforce&quot;, l’abbonamento a Marketo viene abilitato per l’autenticazione di base. Fare riferimento a [Configurazione di Marketo con autenticazione di base](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md){target="_blank"}. Una volta che la sincronizzazione inizia con un set di credenziali, non si passa da una credenziale Salesforce all’altra o all’abbonamento. Se desideri utilizzare Oauth 2.0, rivolgiti al team dell’account Adobe (il tuo Account Manager).

1. Viene visualizzato un pop-up con la pagina di accesso di Salesforce. Inserisci le credenziali &quot;Utente di Marketo Sync&quot; e accedi.

   ![](assets/setting-up-oauth-2-10.png)

1. Immetti il codice di verifica ricevuto tramite e-mail (inviato da Salesforce) e fai clic su **[!UICONTROL Verifica]**.

   ![](assets/setting-up-oauth-2-11.png)

1. Una volta completata la verifica, viene visualizzata la pagina di accesso che richiede l’accesso. Fare clic su **[!UICONTROL Consenti]**.

   ![](assets/setting-up-oauth-2-12.png)

1. Tra pochi minuti verrà visualizzato un pop-up in Marketo. Fare clic su **[!UICONTROL Conferma credenziali]**.

   ![](assets/setting-up-oauth-2-13.png)

1. Al termine della sincronizzazione dei campi, fare clic su **[!UICONTROL Avvia Salesforce Sync]**.

   ![](assets/setting-up-oauth-2-14.png)

1. Fare clic su **[!UICONTROL Avvia sincronizzazione]**.

   ![](assets/setting-up-oauth-2-15.png)

La sincronizzazione tra Marketo e Salesforce è in corso.

![](assets/setting-up-oauth-2-16.png)

>[!MORELIKETHIS]
>
* [Passaggio 1 di 3: aggiunta di campi Marketo a Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md){target="_blank"}
* [Passaggio 2 di 3: creazione di un utente Salesforce per Marketo (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md){target="_blank"}
* [Installa il pacchetto Marketo Sales Insight nell&#39;AppExchange Salesforce](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md){target="_blank"}
* [Configurare Marketo Sales Insight in Salesforce Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md){target="_blank"}
