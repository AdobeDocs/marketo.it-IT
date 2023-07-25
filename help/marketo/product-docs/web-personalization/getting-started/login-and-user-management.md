---
unique-page-id: 7513771
description: Gestione di accesso e utenti - Documentazione di Marketo - Documentazione del prodotto
title: Gestione di login e utenti
exl-id: 3cf5a50a-1926-4fb6-a1fe-39ba5eb2560f
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

---

# Gestione di login e utenti {#login-and-user-management}

## Creare un ruolo utente di personalizzazione web {#create-a-web-personalization-user-role}

1. Vai a **Amministratore** , quindi fai clic su **Utenti e ruoli**.

   ![](assets/image2015-4-28-19-3a50-3a49.png)

1. Clic **Ruoli**.

   ![](assets/image2015-4-28-19-3a57-3a58.png)

   >[!NOTE]
   >
   >Se il ruolo utente di Personalizzazione web (WP) esiste già, assicurati che sia configurato come illustrato nel passaggio 4.

1. Clic **Crea Ruolo**.

   ![](assets/three-1.png)

1. Inserisci un Nome ruolo e seleziona Autorizzazioni. Clic **Crea** (questo ruolo deve [applica a tutte le aree di lavoro](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md)).

   ![](assets/four.png)

   >[!TIP]
   >
   >Per consentire agli utenti di accedere a tutto in Targeting e Personalizzazione, assicurati di selezionare _tutto_ le caselle di controllo.

## Personalizzazione web e autorizzazioni utente per contenuti predittivi {#web-personalization-and-predictive-content-user-permissions}

**Targeting e personalizzazione**: l’utente dispone delle autorizzazioni di sola visualizzazione, se questa autorizzazione è selezionata solo.

**Admin Web Personalization + Predictive**: l’utente ha accesso solo alle impostazioni account e alle impostazioni contenuto per l’app Personalizzazione web e contenuti predittivi. Gli utenti possono visualizzare le pagine nell’app, ma non dispongono delle autorizzazioni di creazione, modifica, eliminazione e avvio.

**Editor contenuti predittivi**: l’utente dispone dell’accesso come editor all’app Predictive Content. L’autorizzazione consente di creare, modificare, eliminare parti di contenuto. Non consente di abilitare il contenuto per l’uso predittivo sul web o e-mail.

**Utilità di avvio contenuti predittivi**: l’utente ha accesso a tutte le funzioni di Contenuto predittivo, ad eccezione di Impostazioni account e contenuto. L’autorizzazione consente di creare, modificare, eliminare e abilitare le parti di contenuto.

**Editor campagna web**: l’utente dispone dell’accesso in qualità di editor a tutte le funzioni di personalizzazione web per creare, modificare ed eliminare ma non avviare campagne web.

**Modulo di avvio campagna web**: l’utente ha accesso a tutte le funzioni dell’app Web Personalization, eccetto le impostazioni account e contenuto. L’autorizzazione consente di creare, modificare, eliminare e avviare campagne web.

## Assegna ruolo WP all&#39;utente {#assign-wp-role-to-user}

1. Vai a **Utenti**.

   ![](assets/image2015-4-29-11-3a31-3a3.png)

1. Selezionare l&#39;utente a cui concedere l&#39;accesso WP e fare clic su **Modifica utente**.

   ![](assets/image2015-4-29-11-3a38-3a46.png)

1. Selezionare il ruolo utente WP per tutte le aree di lavoro.

   ![](assets/seven.png)

1. Gli utenti appena abilitati visualizzeranno **Personalizzazione web** al successivo accesso a Il mio Marketo.

   ![](assets/eight.png)
