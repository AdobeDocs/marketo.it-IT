---
unique-page-id: 10095429
description: Correggi problemi di sincronizzazione convalida delle dinamiche - Documenti Marketo - Documentazione del prodotto
title: Correggi problemi di sincronizzazione convalida delle dinamiche
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---


# Correggi problemi di sincronizzazione convalida delle dinamiche {#fix-dynamics-validation-sync-issues}

## Convalida risultati strumento di sincronizzazione {#validate-sync-tool-results}

Quando si esegue Dynamics Validate Sync, questo report viene generato. Se accanto a un passaggio è presente un ![delete](assets/delete.png), vedere di seguito per identificare e risolvere il problema. Quindi, eseguite nuovamente i passaggi di convalida della sincronizzazione finché il risultato non mostra altri segni di spunta.

![](assets/image2015-9-22-15-3a58-3a12.png)

## URL valido {#url-is-valid}

Se si dispone di un ![delete](assets/delete.png) qui, verificare che l&#39;URL sia valido. Trovatela qui in Risorse per sviluppatori e consultate Servizio organizzazione. L&#39;URL potrebbe non essere valido per diversi motivi.

1. Accedi a Dynamics. Fate clic sull&#39;icona Impostazioni e selezionate **Impostazioni avanzate**.

   ![](assets/one.png)

1. Fate clic su Impostazioni e selezionate **Personalizzazioni**.

   ![](assets/two.png)

1. Fare clic su **Risorse per sviluppatori**.

   ![](assets/three.png)

1. L’URL del servizio organizzazione si trova in Endpoint di servizio.

   ![](assets/four.png)

## Nome utente e password validi {#username-and-password-are-valid}

Se si dispone di un ![—](assets/delete.png) qui, verificare che il nome utente e la password di Microsoft Dynamics siano validi.

## L&#39;utente di sincronizzazione è assegnato al ruolo di sincronizzazione utente di Marketo{#sync-user-is-assigned-to-the-marketo-sync-user-role}

Se si dispone di un ![—](assets/delete.png) qui, è necessario verificare che il ruolo Utente sincronizzazione Marketo sia selezionato in Microsoft Dynamics. Vedere il passo 2 della documentazione di installazione di MIcrosoft Dynamics.

1. In Dynamics, fai clic sull&#39;icona Impostazioni e seleziona **Impostazioni avanzate**.

   ![](assets/one.png)

1. Fare clic su **Impostazioni** e selezionare **Protezione**.

   ![](assets/six.png)

1. Fare clic su **Utenti.**

   ![](assets/image2015-9-24-9-3a47-3a25.png)

1. Fate clic sul collegamento per l’utente di sincronizzazione.

   ![](assets/seven.png)

1. Fare clic su **Gestisci ruoli**.

   ![](assets/eight.png)

1. Verifica che il ruolo Utente sincronizzazione marketing sia selezionato. In caso contrario, controllare e fare clic su **OK.**

   ![](assets/image2015-9-24-9-3a59-3a21.png)

## La soluzione Marketo è installata correttamente {#marketo-solution-is-properly-installed}

Se disponete di un ![—](assets/delete.png) qui, andate a Microsoft Dynamics per verificare che l&#39;installazione di Marketo sia presente. Vedere il passaggio 1 della documentazione di configurazione di MIcrosoft Dynamics.

1. In Dynamics, fai clic sull&#39;icona Impostazioni e seleziona **Impostazioni avanzate**.

   ![](assets/one.png)

1. Fare clic su **Settings **e selezionare **Soluzioni.**

   ![](assets/eleven.png)

1. Verifica che la soluzione sia elencata.

   ![](assets/twelve.png)

## Tutti i passaggi della soluzione sono abilitati {#all-steps-in-the-solution-are-enabled}

Se si dispone di un ![—](assets/delete.png) qui, verificare che nessuno dei passaggi predefiniti sia stato disattivato. Tutti i passaggi vengono automaticamente attivati al momento dell&#39;installazione, ma possono essere disattivati durante la personalizzazione.

## L&#39;utente di sincronizzazione è assegnato alla soluzione Marketo {#sync-user-is-assigned-to-the-marketo-solution}

Se si dispone di un ![—](assets/delete.png) qui, assicurarsi che l&#39;utente Sync sia assegnato sulla pagina Marketing Default in Microsoft Dynamics.

1. In Dynamics, fai clic sull&#39;icona Impostazioni e seleziona **Impostazioni avanzate**.

   ![](assets/one.png)

1. Fare clic su **Settings **e selezionare **Configurazione Marketo**.

   ![](assets/thirteen.png)

1. Verificare che l&#39;utente di sincronizzazione sia assegnato come predefinito.

   ![](assets/fourteen.png)

## Sincronizza utente con nome utente e password {#sync-user-matches-username-and-password}

Se si dispone di un ![—](assets/delete.png) qui, assicurarsi di assegnare l&#39;utente di sincronizzazione corretto nel campo Utente Marketo nel passaggio di configurazione Configurazione predefinita configurazione Marketo in Microsoft Dynamics.

>[!MORELIKETHIS]
>
>[Convalida della sincronizzazione di Microsoft Dynamics](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)

