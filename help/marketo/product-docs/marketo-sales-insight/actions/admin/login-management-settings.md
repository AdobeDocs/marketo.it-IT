---
description: Impostazioni di gestione accesso - Documentazione Marketo - Documentazione del prodotto
title: Impostazioni gestione accesso
exl-id: 077f7f97-1413-4495-b2c9-94194e8dbcc2
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---

# Impostazioni gestione accesso {#login-management-settings}

Le impostazioni di Gestione dell’accesso consentono agli amministratori di impostare le preferenze di autenticazione per gli utenti delle azioni di approfondimento sulle vendite a livello globale.

>[!NOTE]
>
>Per impostazione predefinita, l&#39;opzione Solo Salesforce viene selezionata per le istanze Azioni approfondimenti vendite. Questa impostazione è consigliata in modo che gli utenti possano [accesso automatico](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md) da Salesforce.

## Aggiorna impostazioni gestione accesso {#update-login-management-settings}

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

Aggiorna le preferenze di gestione degli accessi seguendo la procedura riportata di seguito.

1. Fai clic sull’icona a forma di ingranaggio e seleziona **Impostazioni**.

   ![](assets/login-management-settings-1.png)

1. In Impostazioni amministrazione, fai clic su **Generale**.

   ![](assets/login-management-settings-2.png)

1. Scorri verso il basso fino alla scheda Gestione accesso e seleziona l’impostazione desiderata (in questo esempio scegliamo Solo Salesforce). Clic **Salva** al termine.

   ![](assets/login-management-settings-3.png)

## Domande frequenti solo su Salesforce {#salesforce-only-faq}

Solo Salesforce significa che gli utenti possono eseguire l’autenticazione solo per utilizzare le azioni di approfondimento sulle vendite con Salesforce. È la selezione predefinita per le istanze Azioni approfondimento vendite ed è consigliata per la capacità di consentire agli utenti di eseguire l’autenticazione senza dover gestire un nome utente e una password.

### In che modo un nuovo utente alla mia istanza attiva il proprio account quando si seleziona &quot;Solo Salesforce&quot;? {#activate-when-salesforce-only-is-selected}

Facendo clic su **Guida introduttiva** nel messaggio e-mail di invito, i nuovi utenti verranno inviati a una schermata di attivazione dell’account in cui verrà richiesto di collegare la loro istanza Salesforce per attivare l’account Sales Insight Actions.

![](assets/login-management-settings-4.png)

### Con quali metodi di autenticazione possono autenticarsi gli utenti quando si seleziona &quot;Solo Salesforce&quot;? {#what-authentication-methods}

Quando si accede alla schermata di accesso, gli utenti immetteranno innanzitutto il proprio indirizzo e-mail. Quindi fanno clic sul pulsante Salesforce One Click Login, dove possono eseguire l’autenticazione utilizzando l’account Salesforce a cui hanno effettuato l’accesso.

>[!NOTE]
>
>Questo riguarda solo gli utenti che navigano direttamente alla schermata di accesso. Gli utenti che accedono alle azioni da Salesforce accederanno con [Accesso automatico](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md).

![](assets/login-management-settings-5.png)

### Come viene gestita l’autenticazione utente per le azioni quando un utente accede a una funzione Azioni da Salesforce e viene selezionato &quot;Solo Salesforce&quot;? {#how-is-user-authentication-handled}

Quando un utente fa clic su una delle azioni (Chiamata, E-mail, Campagna, Attività, Elenco campagne, ecc.), utilizziamo l’autenticazione SFDC per accedere automaticamente al suo account Sales Insight Actions. Questa autenticazione viene chiamata [Accesso automatico](/help/marketo/product-docs/marketo-sales-insight/actions/admin/auto-login-from-salesforce.md).

## Domande frequenti su tutti i metodi di accesso {#all-login-methods-faq}

### In che modo un nuovo utente alla mia istanza attiva il proprio account quando si seleziona &quot;Tutti i metodi di accesso&quot;? {#activate-when-all-login-methods-is-selected}

Quando un nuovo utente viene invitato a un’istanza, riceverà un’e-mail di attivazione dell’account. Cliccando sul pulsante &quot;Inizia&quot; si aprirà una pagina in cui viene chiesto di creare e confermare una password. Una volta creata, l’account viene attivato e l’utente lo assume tramite il flusso di lavoro di onboarding.

![](assets/login-management-settings-6.png)

### Con cosa possono accedere gli utenti della mia istanza se si seleziona &quot;Tutti i metodi di accesso&quot;? {#what-are-users-allowed-to-log-in-with-all-login}

Quando si utilizza la pagina di accesso, gli utenti immetteranno innanzitutto il proprio indirizzo e-mail. Vengono quindi inviati a una pagina che fornisce tutte le opzioni di accesso (nome utente/password, SFDC, Gmail, SSO) per l’autenticazione con.
