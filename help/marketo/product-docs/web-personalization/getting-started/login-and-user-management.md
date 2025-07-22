---
unique-page-id: 7513771
description: Gestione di accesso e utenti - Documentazione di Marketo - Documentazione del prodotto
title: Gestione di login e utenti
exl-id: 3cf5a50a-1926-4fb6-a1fe-39ba5eb2560f
feature: Web Personalization
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 0%

---

# Gestione di login e utenti {#login-and-user-management}

## Crea un ruolo utente [!UICONTROL Web Personalization] {#create-a-web-personalization-user-role}

1. Vai alla sezione **[!UICONTROL Admin]**, quindi fai clic su **[!UICONTROL Users & Roles]**.

   ![](assets/image2015-4-28-19-3a50-3a49.png)

1. Fai clic su **[!UICONTROL Roles]**.

   ![](assets/image2015-4-28-19-3a57-3a58.png)

   >[!NOTE]
   >
   >Se il ruolo utente di Web Personalization (WP) esiste già, assicurarsi che sia configurato come illustrato nel passaggio 4.

1. Fai clic su **[!UICONTROL New Role]**.

   ![](assets/three-1.png)

1. Immettere un [!UICONTROL Role Name] e selezionare [!UICONTROL Permissions]. Fare clic su **[!UICONTROL Create]** (questo ruolo deve [essere applicato a tutte le aree di lavoro](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md)).

   ![](assets/four.png)

   >[!TIP]
   >
   >Per consentire agli utenti di accedere a tutto in Targeting e Personalization, seleziona _tutte_ le caselle di controllo.

## Autorizzazioni per [!UICONTROL Web Personalization] e utenti di Predictive Content {#web-personalization-and-predictive-content-user-permissions}

**[!UICONTROL Targeting and Personalization]**: l&#39;utente dispone solo delle autorizzazioni di visualizzazione, se questa autorizzazione è selezionata solo.

**[!UICONTROL Admin Web Personalization + Predictive]**: l&#39;utente ha accesso solo alle impostazioni account e alle impostazioni contenuto per l&#39;app Web Personalization e Predictive Content. Gli utenti possono visualizzare le pagine nell’app, ma non dispongono delle autorizzazioni di creazione, modifica, eliminazione e avvio.

**[!UICONTROL Predictive Content Editor]**: l&#39;utente ha accesso come editor all&#39;app Predictive Content. L’autorizzazione consente di creare, modificare, eliminare parti di contenuto. Non consente di abilitare il contenuto per l’uso predittivo sul web o e-mail.

**[!UICONTROL Predictive Content Launcher]**: l&#39;utente ha accesso a tutte le funzionalità di Predictive Content, ad eccezione di Account e Content Settings. L’autorizzazione consente di creare, modificare, eliminare e abilitare le parti di contenuto.

**[!UICONTROL Web Campaign Editor]**: l&#39;utente dispone dell&#39;accesso editor a tutte le funzionalità di Web Personalization per creare, modificare ed eliminare ma non avviare campagne Web.

**[!UICONTROL Web Campaign Launcher]**: l&#39;utente ha accesso a tutte le funzionalità dell&#39;app Web Personalization, ad eccezione delle impostazioni account e contenuto. L’autorizzazione consente di creare, modificare, eliminare e avviare campagne web.

## Assegna ruolo WP all&#39;utente {#assign-wp-role-to-user}

1. Vai a **[!UICONTROL Users]**.

   ![](assets/image2015-4-29-11-3a31-3a3.png)

1. Selezionare l&#39;utente a cui concedere l&#39;accesso WP e fare clic su **[!UICONTROL Edit User]**.

   ![](assets/image2015-4-29-11-3a38-3a46.png)

1. Selezionare il ruolo utente WP per tutte le aree di lavoro.

   ![](assets/seven.png)

1. Gli utenti appena abilitati visualizzeranno il riquadro **[!UICONTROL Web Personalization]** in Il mio Marketo al prossimo accesso.

   ![](assets/eight.png)
