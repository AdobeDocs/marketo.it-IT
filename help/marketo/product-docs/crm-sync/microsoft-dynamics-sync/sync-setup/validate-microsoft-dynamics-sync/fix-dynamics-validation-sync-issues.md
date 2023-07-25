---
unique-page-id: 10095429
description: Correzione dei problemi di sincronizzazione della convalida Dynamics - Documentazione di Marketo - Documentazione del prodotto
title: Correggi i problemi di sincronizzazione della convalida Dynamics
exl-id: 1a300249-65b7-49b1-bf50-82236916298f
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 0%

---

# Correggi i problemi di sincronizzazione della convalida Dynamics {#fix-dynamics-validation-sync-issues}

## Convalida risultati strumento di sincronizzazione {#validate-sync-tool-results}

Quando esegui Dynamics Validate Sync, viene generato un rapporto. Se è presente un ![x](assets/delete.png) accanto a un passaggio, vedere le opzioni seguenti per identificare e risolvere il problema. Quindi, esegui nuovamente i passaggi di convalida della sincronizzazione fino a quando il risultato non mostra nient’altro che segni di spunta verdi.

![](assets/image2015-9-22-15-3a58-3a12.png)

## URL valido {#url-is-valid}

Se si dispone di ![x](assets/delete.png) in questo caso, verifica che l’URL sia valido. Puoi trovarlo qui in Risorse per sviluppatori e consulta Servizio organizzazioni. L’URL potrebbe non essere valido per una serie di motivi.

1. Accedi a Dynamics. Fai clic sull’icona Impostazioni e seleziona **Impostazioni avanzate**.

   ![](assets/one.png)

1. Fai clic su Impostazioni e seleziona **Personalizzazioni**.

   ![](assets/two.png)

1. Clic **Risorse per sviluppatori**.

   ![](assets/three.png)

1. L’URL del servizio organizzazione si trova in Endpoint servizio.

   ![](assets/four.png)

## Nome utente e password validi {#username-and-password-are-valid}

Se si dispone di ![x](assets/delete.png) in questo caso, verifica che le credenziali di Microsoft Dynamics siano valide. Per l’autenticazione Web API S2S, il nome utente in Marketo deve corrispondere al [indirizzo e-mail](https://docs.microsoft.com/en-us/power-platform/admin/manage-application-users#view-or-edit-the-details-of-an-application-user) dell’utente dell’applicazione nel sistema CRM. Per gli altri tipi, deve corrispondere al nome utente dell&#39;utente di sincronizzazione.

## L&#39;utente Sync è assegnato al ruolo Utente Sync di Marketo {#sync-user-is-assigned-to-the-marketo-sync-user-role}

Se si dispone di ![x](assets/delete.png) in questo caso, potrebbe trattarsi di uno dei tre problemi riportati di seguito.

**Opzione uno - Verificare che il ruolo utente di Marketo Sync sia selezionato in Microsoft Dynamics**:

1. In Dynamics, fai clic sull’icona Impostazioni e seleziona **Impostazioni avanzate**.

   ![](assets/one.png)

1. Clic **Impostazioni** e seleziona **Sicurezza**.

   ![](assets/six.png)

1. Clic **Utenti.**

   ![](assets/image2015-9-24-9-3a47-3a25.png)

1. Fare clic sul collegamento dell&#39;utente di sincronizzazione.

   ![](assets/seven.png)

1. Clic **Gestisci ruoli**.

   ![](assets/eight.png)

1. Verificare che il ruolo Utente di sincronizzazione Marketo sia selezionato. In caso contrario, selezionalo e fai clic su **OK.**

   ![](assets/image2015-9-24-9-3a59-3a21.png)

**Opzione 2 - Conferma del consenso**:

1. Rivedi [Concedere il consenso per la registrazione di ID client e app](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/grant-consent-for-client-id-and-app-registration.md) per confermare che l’app dispone del consenso dell’amministratore per chiamare le API.

**Opzione tre - Sincronizza utente**:

1. Verifica che l&#39;utente di sincronizzazione sia aggiunto alla configurazione di Marketo.

## La soluzione Marketo è installata correttamente {#marketo-solution-is-properly-installed}

Se si dispone di ![x](assets/delete.png) In questo caso, vai a Microsoft Dynamics per verificare che sia presente l’installazione di Marketo. Consulta il passaggio 1 della documentazione di configurazione di Microsoft Dynamics.

1. In Dynamics, fai clic sull’icona Impostazioni e seleziona **Impostazioni avanzate**.

   ![](assets/one.png)

1. Clic **Impostazioni** e seleziona **Soluzioni.**

   ![](assets/eleven.png)

1. Verifica che la soluzione sia elencata.

   ![](assets/twelve.png)

## Tutti i passaggi della soluzione sono abilitati {#all-steps-in-the-solution-are-enabled}

Se si dispone di ![x](assets/delete.png) in questo caso, verifica che nessuno dei passaggi predefiniti sia stato disattivato. Tutti i passaggi vengono abilitati automaticamente durante l’installazione, ma possono essere disattivati durante una personalizzazione.

## L&#39;utente di sincronizzazione è assegnato alla soluzione Marketo {#sync-user-is-assigned-to-the-marketo-solution}

Se si dispone di ![x](assets/delete.png) In questo caso, assicurati che l’utente Sync sia assegnato alla pagina Predefinita di Marketo in Microsoft Dynamics.

1. In Dynamics, fai clic sull’icona Impostazioni e seleziona **Impostazioni avanzate**.

   ![](assets/one.png)

1. Clic **Impostazioni** e seleziona **Configurazione Marketo**.

   ![](assets/thirteen.png)

1. Verificare che l&#39;utente di sincronizzazione sia assegnato come predefinito.

   ![](assets/fourteen.png)

## L&#39;utente di sincronizzazione corrisponde al nome utente e alla password {#sync-user-matches-username-and-password}

Se si dispone di ![x](assets/delete.png) In questo caso, assicurati di assegnare l’utente di sincronizzazione corretto nel campo Utente Marketo del passaggio di configurazione predefinita di Marketo in Microsoft Dynamics.

>[!MORELIKETHIS]
>
>[Convalida sincronizzazione Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)
