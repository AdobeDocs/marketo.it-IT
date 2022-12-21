---
unique-page-id: 7513771
description: Accesso e gestione degli utenti - Documenti Marketo - Documentazione del prodotto
title: Accesso e gestione utente
exl-id: 3cf5a50a-1926-4fb6-a1fe-39ba5eb2560f
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

---

# Accesso e gestione utente {#login-and-user-management}

## Creare un ruolo utente di personalizzazione web {#create-a-web-personalization-user-role}

1. Vai a **Amministratore** sezione , quindi fai clic su **Utenti e ruoli**.

   ![](assets/image2015-4-28-19-3a50-3a49.png)

1. Fai clic su **Ruoli**.

   ![](assets/image2015-4-28-19-3a57-3a58.png)

   >[!NOTE]
   >
   >Se il ruolo utente della personalizzazione web (WP) esiste già, accertati che sia configurato come mostrato nel passaggio 4.

1. Fai clic su **Nuovo ruolo**.

   ![](assets/three-1.png)

1. Immetti un Nome ruolo e seleziona Autorizzazioni. Fai clic su **Crea** (questo ruolo deve [applica a tutte le aree di lavoro](/help/marketo/product-docs/administration/users-and-roles/managing-marketo-users.md)).

   ![](assets/four.png)

   >[!TIP]
   >
   >Per dare agli utenti l&#39;autorizzazione per accedere a tutto ciò che si trova in Targeting e Personalizzazione, assicurati di selezionare _tutto_ le caselle di controllo.

## Autorizzazioni utente per la personalizzazione web e il contenuto predittivo {#web-personalization-and-predictive-content-user-permissions}

**Targeting e personalizzazione**: L&#39;utente dispone di autorizzazioni di sola visualizzazione, se questa autorizzazione è selezionata solo.

**Admin Web Personalization + Predictive**: L’utente ha accesso solo alle impostazioni account e alle impostazioni di contenuto per l’app Web Personalization e Predictive Content . Gli utenti possono visualizzare le pagine nell’app ma non dispongono delle autorizzazioni di creazione, modifica, eliminazione e avvio.

**Editor di contenuti predittivi**: L’utente dispone dell’accesso dell’editor all’app Predictive Content . L’autorizzazione consente di creare, modificare, eliminare parti di contenuto. Non consente di abilitare il contenuto per l’uso predittivo sul web o sull’e-mail.

**Launcher dei contenuti predittivi**: L’utente ha accesso a tutte le funzioni di Predictive Content (Contenuto predittivo), ad eccezione delle impostazioni account e contenuto. L’autorizzazione consente di creare, modificare, eliminare e abilitare parti di contenuto.

**Editor web Campaign**: L’utente dispone dell’accesso dell’editor a tutte le funzioni di personalizzazione web per creare, modificare ed eliminare le campagne web, ma non per avviarle.

**Avvio campagna web**: L’utente ha accesso a tutte le funzioni dell’app di personalizzazione web, ad eccezione delle Impostazioni account e contenuto. L&#39;autorizzazione consente di creare, modificare, eliminare e avviare campagne Web.

## Assegnare il ruolo WP all&#39;utente {#assign-wp-role-to-user}

1. Vai a **Utenti**.

   ![](assets/image2015-4-29-11-3a31-3a3.png)

1. Selezionare l&#39;utente a cui concedere l&#39;accesso WP e fare clic su **Modifica utente**.

   ![](assets/image2015-4-29-11-3a38-3a46.png)

1. Selezionare il ruolo utente WP per tutte le aree di lavoro.

   ![](assets/seven.png)

1. Gli utenti appena abilitati visualizzeranno il **Personalizzazione web** in My Marketo la prossima volta che effettuano l&#39;accesso.

   ![](assets/eight.png)
