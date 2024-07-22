---
unique-page-id: 7513771
description: Gestione di accesso e utenti - Documentazione di Marketo - Documentazione del prodotto
title: Gestione di login e utenti
exl-id: 3cf5a50a-1926-4fb6-a1fe-39ba5eb2560f
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '305'
ht-degree: 0%

---

# Gestione di login e utenti {#login-and-user-management}

## Creazione di un ruolo utente di Web Personalization {#create-a-web-personalization-user-role}

1. Vai alla sezione **Amministratore**, quindi fai clic su **Utenti e ruoli**.

   ![](assets/image2015-4-28-19-3a50-3a49.png)

1. Fai clic su **Ruoli**.

   ![](assets/image2015-4-28-19-3a57-3a58.png)

   >[!NOTE]
   >
   >Se il ruolo utente di Web Personalization (WP) esiste già, assicurarsi che sia configurato come illustrato nel passaggio 4.

1. Fai clic su **Nuovo ruolo**.

   ![](assets/three-1.png)

1. Inserisci un Nome ruolo e seleziona Autorizzazioni. Fai clic su **Crea** (questo ruolo deve [essere applicato a tutte le aree di lavoro](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md)).

   ![](assets/four.png)

   >[!TIP]
   >
   >Per consentire agli utenti di accedere a tutto in Targeting e Personalization, seleziona _tutte_ le caselle di controllo.

## Autorizzazioni utente per Web Personalization e contenuti predittivi {#web-personalization-and-predictive-content-user-permissions}

**Targeting e Personalization**: l&#39;utente dispone solo delle autorizzazioni di visualizzazione, se questa autorizzazione è selezionata solo.

**Admin Web Personalization + Predictive**: l&#39;utente ha accesso solo alle impostazioni account e alle impostazioni contenuto per l&#39;app Web Personalization e Predictive Content. Gli utenti possono visualizzare le pagine nell’app, ma non dispongono delle autorizzazioni di creazione, modifica, eliminazione e avvio.

**Editor contenuti predittivi**: l&#39;utente ha accesso come editor all&#39;app Contenuti predittivi. L’autorizzazione consente di creare, modificare, eliminare parti di contenuto. Non consente di abilitare il contenuto per l’uso predittivo sul web o e-mail.

**Utilità di avvio contenuti predittivi**: l&#39;utente ha accesso a tutte le funzionalità di contenuti predittivi, ad eccezione delle impostazioni account e contenuto. L’autorizzazione consente di creare, modificare, eliminare e abilitare le parti di contenuto.

**Editor campagne Web**: l&#39;utente dispone dell&#39;accesso editor a tutte le funzionalità di Web Personalization per creare, modificare ed eliminare ma non avviare campagne Web.

**Utilità di avvio campagna Web**: l&#39;utente ha accesso a tutte le funzionalità dell&#39;app Web Personalization, ad eccezione delle impostazioni account e contenuto. L’autorizzazione consente di creare, modificare, eliminare e avviare campagne web.

## Assegna ruolo WP all&#39;utente {#assign-wp-role-to-user}

1. Vai a **Utenti**.

   ![](assets/image2015-4-29-11-3a31-3a3.png)

1. Selezionare l&#39;utente a cui concedere l&#39;accesso WP e fare clic su **Modifica utente**.

   ![](assets/image2015-4-29-11-3a38-3a46.png)

1. Selezionare il ruolo utente WP per tutte le aree di lavoro.

   ![](assets/seven.png)

1. Gli utenti appena abilitati visualizzeranno il riquadro **Web Personalization** in Il mio Marketo al successivo accesso.

   ![](assets/eight.png)
