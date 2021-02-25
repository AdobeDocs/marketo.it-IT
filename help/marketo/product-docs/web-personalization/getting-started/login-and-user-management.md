---
unique-page-id: 7513771
description: Login e gestione utenti - Documenti Marketo - Documentazione prodotto
title: Login e gestione utente
translation-type: tm+mt
source-git-commit: fbaf57ec4f3532c2d71acf23171d60873b1c997c
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

---


# Login e gestione utente {#login-and-user-management}

## Creare un ruolo utente di personalizzazione Web {#create-a-web-personalization-user-role}

1. Andate alla sezione **Admin**, quindi fate clic su **Utenti e ruoli**.

   ![](assets/image2015-4-28-19-3a50-3a49.png)

1. Fare clic su **Ruoli**.

   ![](assets/image2015-4-28-19-3a57-3a58.png)

   >[!NOTE]
   >
   >Se il ruolo utente di Web Personalization (WP) esiste già, accertatevi che sia configurato come mostrato al punto 4.

1. Fare clic su **Nuovo ruolo**.

   ![](assets/three-1.png)

1. Immettete un nome per il ruolo e selezionate Autorizzazioni. Fare clic su **Crea** (il ruolo deve essere [applicabile a tutte le aree di lavoro](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md)).

   ![](assets/four.png)

   >[!TIP]
   >
   >Per dare agli utenti l&#39;autorizzazione per accedere a tutto ciò che si trova in Targeting e personalizzazione, selezionare le caselle _all_.

## Autorizzazioni utente per la personalizzazione Web e il contenuto predittivo {#web-personalization-and-predictive-content-user-permissions}

**Targeting e personalizzazione**: L&#39;utente dispone solo di autorizzazioni di visualizzazione, se questa è selezionata.

**Admin Web Personalization + Predictive**: L&#39;utente ha accesso solo alle Impostazioni account e alle Impostazioni contenuto per l&#39;app Web Personalization (Personalizzazione Web) e Predictive Content. Gli utenti possono visualizzare le pagine nell&#39;app ma non dispongono delle autorizzazioni di creazione, modifica, eliminazione e avvio.

**Predictive Content Editor**: L&#39;utente ha accesso all&#39;app Predictive Content. L&#39;autorizzazione consente di creare, modificare, eliminare elementi di contenuto. Non consente di abilitare il contenuto per l&#39;uso predittivo sul Web o nell&#39;e-mail.

**Predictive Content Launcher**: L&#39;utente ha accesso a tutte le funzioni Predictive Content (Contenuto predittivo), ad eccezione di Account e Content Settings (Impostazioni contenuto). L&#39;autorizzazione consente di creare, modificare, eliminare e abilitare le parti di contenuto.

**Editor** campagna Web: L&#39;utente dispone dell&#39;accesso dell&#39;editor a tutte le funzionalità di personalizzazione Web per creare, modificare ed eliminare, ma non avviare campagne Web.

**Avvio** campagna Web: L&#39;utente ha accesso a tutte le funzionalità dell&#39;app Web Personalization, eccetto Impostazioni account e contenuto. L&#39;autorizzazione consente di creare, modificare, eliminare e avviare campagne Web.

## Assegna ruolo WP all&#39;utente {#assign-wp-role-to-user}

1. Vai a **Utenti**.

   ![](assets/image2015-4-29-11-3a31-3a3.png)

1. Selezionare l&#39;utente a cui concedere l&#39;accesso WP e fare clic su **Modifica utente**.

   ![](assets/image2015-4-29-11-3a38-3a46.png)

1. Selezionare il ruolo utente WP per tutte le aree di lavoro.

   ![](assets/seven.png)

1. Gli utenti abilitati di recente visualizzeranno la sezione **Personalizzazione Web** in My Marketo al successivo accesso.

   ![](assets/eight.png)
