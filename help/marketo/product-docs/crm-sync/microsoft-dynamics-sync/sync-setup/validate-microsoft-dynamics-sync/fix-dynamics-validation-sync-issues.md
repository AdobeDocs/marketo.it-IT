---
unique-page-id: 10095429
description: Risoluzione dei problemi di sincronizzazione della convalida di Dynamics - Documenti Marketo - Documentazione del prodotto
title: Correggere i problemi di sincronizzazione della convalida di Dynamics
exl-id: 1a300249-65b7-49b1-bf50-82236916298f
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---

# Correggere i problemi di sincronizzazione della convalida di Dynamics {#fix-dynamics-validation-sync-issues}

## Convalida i risultati dello strumento di sincronizzazione {#validate-sync-tool-results}

Quando esegui Dynamics Validate Sync, genera questo rapporto. Se accanto a un passaggio è presente un ![elimina](assets/delete.png) , vedi di seguito per identificare e risolvere il problema. Quindi esegui nuovamente i passaggi di convalida della sincronizzazione fino a quando il risultato non mostra altro che segni di spunta.

![](assets/image2015-9-22-15-3a58-3a12.png)

## URL valido {#url-is-valid}

Se disponi di un ![delete](assets/delete.png) qui, verifica che l&#39;URL sia valido. È disponibile qui in Risorse per sviluppatori e consulta Servizio organizzazione. L&#39;URL potrebbe non essere valido per una serie di motivi.

1. Accedi a Dynamics. Fai clic sull&#39;icona Impostazioni e seleziona **Impostazioni avanzate**.

   ![](assets/one.png)

1. Fai clic su Impostazioni e seleziona **Personalizzazioni**.

   ![](assets/two.png)

1. Fai clic su **Risorse per sviluppatori**.

   ![](assets/three.png)

1. L&#39;URL del servizio organizzazione si trova in Endpoint di servizio.

   ![](assets/four.png)

## Nome utente e password validi {#username-and-password-are-valid}

Se disponi di un ![—](assets/delete.png) qui, verifica che il nome utente e la password di Microsoft Dynamics siano validi.

## L&#39;utente di sincronizzazione viene assegnato al ruolo utente di sincronizzazione Marketo {#sync-user-is-assigned-to-the-marketo-sync-user-role}

Se si dispone di un ![—](assets/delete.png) qui, è necessario verificare che il ruolo Utente sincronizzazione Marketo sia selezionato in Microsoft Dynamics. Vedere il passaggio 2 della documentazione di installazione di Microsoft Dynamics.

1. In Dynamics, fai clic sull’icona Impostazioni e seleziona **Impostazioni avanzate**.

   ![](assets/one.png)

1. Fare clic su **Impostazioni** e selezionare **Protezione**.

   ![](assets/six.png)

1. Fare clic su **Utenti.**

   ![](assets/image2015-9-24-9-3a47-3a25.png)

1. Fai clic sul collegamento per l’utente di sincronizzazione.

   ![](assets/seven.png)

1. Fare clic su **Gestisci ruoli**.

   ![](assets/eight.png)

1. Verifica che sia selezionato il ruolo Utente di sincronizzazione di Marketo. In caso contrario, selezionarlo e fare clic su **OK.**

   ![](assets/image2015-9-24-9-3a59-3a21.png)

## La soluzione Marketo è installata correttamente {#marketo-solution-is-properly-installed}

Se disponi di un ![—](assets/delete.png) qui, vai a Microsoft Dynamics per verificare che l&#39;installazione di Marketo sia presente. Vedi il passaggio 1 della documentazione di configurazione di MIcrosoft Dynamics.

1. In Dynamics, fai clic sull’icona Impostazioni e seleziona **Impostazioni avanzate**.

   ![](assets/one.png)

1. Fai clic su **Impostazioni** e seleziona **Soluzioni.**

   ![](assets/eleven.png)

1. Verifica che la soluzione sia elencata.

   ![](assets/twelve.png)

## Tutti i passaggi della soluzione sono abilitati {#all-steps-in-the-solution-are-enabled}

Se disponi di un ![—](assets/delete.png) qui, verifica che nessuno dei passaggi predefiniti sia stato disattivato. Tutti i passaggi vengono attivati automaticamente al momento dell’installazione, ma possono essere disattivati durante una personalizzazione.

## L&#39;utente di sincronizzazione viene assegnato alla soluzione Marketo {#sync-user-is-assigned-to-the-marketo-solution}

Se disponi di un ![—](assets/delete.png) qui, assicurati che l’utente di sincronizzazione sia assegnato alla pagina Predefinito di Marketo in Microsoft Dynamics.

1. In Dynamics, fai clic sull’icona Impostazioni e seleziona **Impostazioni avanzate**.

   ![](assets/one.png)

1. Fare clic su **Impostazioni** e selezionare **Configurazione Marketo**.

   ![](assets/thirteen.png)

1. Verifica che l’utente di sincronizzazione sia assegnato come predefinito.

   ![](assets/fourteen.png)

## Sincronizza l&#39;utente con nome utente e password {#sync-user-matches-username-and-password}

Se si dispone di un ![—](assets/delete.png) qui, assicurarsi di assegnare l&#39;utente di sincronizzazione corretto nel campo Utente di Marketo nel passaggio Configurazione predefinita configurazione Marketo in Microsoft Dynamics.

>[!MORELIKETHIS]
>
>[Convalida della sincronizzazione di Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)
