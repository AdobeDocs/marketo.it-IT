---
description: Impostazioni di gestione accesso - Documentazione Marketo - Documentazione del prodotto
title: Impostazioni gestione accesso
exl-id: 077f7f97-1413-4495-b2c9-94194e8dbcc2
feature: Sales Insight Actions
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 0%

---

# Impostazioni gestione accesso {#login-management-settings}

Le impostazioni di Gestione accesso consentono agli amministratori di impostare le preferenze di autenticazione per gli utenti delle azioni di Sales Insight a livello globale.

>[!NOTE]
>
>Per impostazione predefinita, l&#39;opzione [!UICONTROL Salesforce Only] sarà selezionata per [!DNL Sales Insight Actions] istanze. È consigliabile configurare questa impostazione in modo che gli utenti possano [accedere automaticamente](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md) da [!DNL Salesforce].

## Aggiorna impostazioni gestione accesso {#update-login-management-settings}

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

Aggiorna le preferenze di gestione degli accessi seguendo la procedura riportata di seguito.

1. Fare clic sull&#39;icona ingranaggio e selezionare **[!UICONTROL Settings]**.

   ![](assets/login-management-settings-1.png)

1. In [!UICONTROL Admin Settings], fare clic su **[!UICONTROL General]**.

   ![](assets/login-management-settings-2.png)

1. Scorri verso il basso fino alla scheda [!UICONTROL Login Management] e seleziona l&#39;impostazione desiderata (in questo esempio scegliamo solo Salesforce). Al termine, fai clic su **[!UICONTROL Save]**.

   ![](assets/login-management-settings-3.png)

## Domande frequenti solo su Salesforce {#salesforce-only-faq}

Solo Salesforce significa che gli utenti possono eseguire l&#39;autenticazione solo per utilizzare [!DNL Sales Insight Actions] con [!DNL Salesforce]. È la selezione predefinita per [!DNL Sales Insight Actions] istanze ed è consigliata in quanto consente agli utenti di eseguire l&#39;autenticazione senza dover gestire nome utente e password.

### In che modo un nuovo utente alla mia istanza attiva il proprio account quando &quot;[!UICONTROL Salesforce Only]&quot; è selezionato? {#activate-when-salesforce-only-is-selected}

Facendo clic sul pulsante **[!UICONTROL Getting Started]** nell&#39;e-mail di invito, i nuovi utenti verranno inviati a una schermata di attivazione dell&#39;account in cui verrà richiesto di connettere la loro istanza Salesforce per attivare l&#39;account [!DNL Sales Insight Actions].

![](assets/login-management-settings-4.png)

### Con quali metodi di autenticazione possono autenticarsi gli utenti quando &quot;[!UICONTROL Salesforce Only]&quot; è selezionato? {#what-authentication-methods}

Quando si accede alla schermata di accesso, gli utenti immetteranno innanzitutto il proprio indirizzo e-mail. Fare quindi clic sul pulsante Salesforce One Click [!UICONTROL Login], in cui è possibile eseguire l&#39;autenticazione utilizzando l&#39;account Salesforce a cui è connesso.

>[!NOTE]
>
>Questo riguarda solo gli utenti che navigano direttamente alla schermata di accesso. Gli utenti che accedono alle azioni da [!DNL Salesforce] accederanno con [Accesso automatico](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md).

![](assets/login-management-settings-5.png)

### Come viene gestita l’autenticazione utente per le azioni quando un utente accede a una funzione Azioni da Salesforce e viene selezionato &quot;Solo Salesforce&quot;? {#how-is-user-authentication-handled}

Quando un utente fa clic su una delle azioni (Chiamata, E-mail, Campagna, Attività, Elenco campagne, ecc...), utilizziamo l’autenticazione SFDC per accedere automaticamente al suo account [!DNL Sales Insight Actions]. Questa autenticazione viene chiamata [Accesso automatico](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md).

## Domande frequenti su tutti i metodi di accesso {#all-login-methods-faq}

### In che modo un nuovo utente alla mia istanza attiva il proprio account quando si seleziona &quot;Tutti i metodi di accesso&quot;? {#activate-when-all-login-methods-is-selected}

Quando un nuovo utente viene invitato a un’istanza, riceverà un’e-mail di attivazione dell’account. Cliccando sul pulsante &quot;Inizia&quot; si aprirà una pagina in cui viene chiesto di creare e confermare una password. Una volta creata, l’account viene attivato e l’utente lo assume tramite il flusso di lavoro di onboarding.

![](assets/login-management-settings-6.png)

### Con quali utenti dell&#39;istanza posso effettuare l&#39;accesso quando &quot;[!UICONTROL All Login Methods]&quot; è selezionato? {#what-are-users-allowed-to-log-in-with-all-login}

Quando si utilizza la pagina di accesso, gli utenti immetteranno innanzitutto il proprio indirizzo e-mail. Vengono quindi inviati a una pagina che fornisce tutte le opzioni di accesso (nome utente/password, SFDC, Gmail, SSO) per l’autenticazione.
