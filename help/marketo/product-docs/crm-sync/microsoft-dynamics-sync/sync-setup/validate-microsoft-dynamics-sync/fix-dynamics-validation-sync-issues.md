---
unique-page-id: 10095429
description: Correggi problemi di sincronizzazione convalida delle dinamiche - Documenti Marketo - Documentazione del prodotto
title: Correggi problemi di sincronizzazione convalida delle dinamiche
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 0%

---


# Correggi problemi di sincronizzazione convalida delle dinamiche {#fix-dynamics-validation-sync-issues}

## Convalida risultati strumento di sincronizzazione {#validate-sync-tool-results}

Quando si esegue Dynamics Validate Sync, questo report viene generato. Se accanto a un passaggio è presente un&#39; ![eliminazione](assets/delete.png) , vedere di seguito per identificare e risolvere il problema. Quindi, eseguite nuovamente i passaggi di convalida della sincronizzazione finché il risultato non mostra altri segni di spunta.

![](assets/image2015-9-22-15-3a58-3a12.png)

## URL valido {#url-is-valid}

Se disponete di un’ ![eliminazione](assets/delete.png) , verificate che l’URL sia valido. Trovatela qui in Risorse per sviluppatori e consultate Servizio organizzazione. L&#39;URL potrebbe non essere valido per diversi motivi.

1. Accedi a Dynamics. Fate clic sull&#39;icona Impostazioni e selezionate Impostazioni **avanzate**.

   ![](assets/one.png)

1. Fate clic su Impostazioni e selezionate **Personalizzazioni**.

   ![](assets/two.png)

1. Fate clic su Risorse **per** sviluppatori.

   ![](assets/three.png)

1. L’URL del servizio organizzazione si trova in Endpoint di servizio.

   ![](assets/four.png)

## Nome utente e password validi {#username-and-password-are-valid}

Se hai un ![—](assets/delete.png) qui, verifica che il tuo nome utente e la password di Microsoft Dynamics siano validi.

## L&#39;utente di sincronizzazione è assegnato al ruolo di sincronizzazione utente di Marketo {#sync-user-is-assigned-to-the-marketo-sync-user-role}

Se hai un ![—](assets/delete.png) qui, devi verificare che il ruolo Utente sincronizzazione Marketo sia selezionato in Microsoft Dynamics. Vedere il passo 2 della documentazione di installazione di MIcrosoft Dynamics.

1. In Dynamics, fai clic sull&#39;icona Impostazioni e seleziona Impostazioni **** avanzate.

   ![](assets/one.png)

1. Fate clic su **Impostazioni** e selezionate **Protezione**.

   ![](assets/six.png)

1. Fate clic su **Utenti.**

   ![](assets/image2015-9-24-9-3a47-3a25.png)

1. Fate clic sul collegamento per l’utente di sincronizzazione.

   ![](assets/seven.png)

1. Fate clic su **Gestisci ruoli**.

   ![](assets/eight.png)

1. Verifica che il ruolo Utente sincronizzazione marketing sia selezionato. In caso contrario, controllarlo e fare clic su **OK.**

   ![](assets/image2015-9-24-9-3a59-3a21.png)

## Soluzione Marketo installata correttamente {#marketo-solution-is-properly-installed}

Se hai un ![—](assets/delete.png) qui, vai a Microsoft Dynamics per verificare che l&#39;installazione di Marketo sia presente. Vedere il passaggio 1 della documentazione di configurazione di MIcrosoft Dynamics.

1. In Dynamics, fai clic sull&#39;icona Impostazioni e seleziona Impostazioni **** avanzate.

   ![](assets/one.png)

1. Fare clic su **Settings **e selezionare **Soluzioni.**

   ![](assets/eleven.png)

1. Verifica che la soluzione sia elencata.

   ![](assets/twelve.png)

## Tutti i passaggi della soluzione sono abilitati {#all-steps-in-the-solution-are-enabled}

Se disponete di un ![—](assets/delete.png) qui, verificate che nessuno dei passaggi predefiniti sia stato disattivato. Tutti i passaggi vengono automaticamente attivati al momento dell&#39;installazione, ma possono essere disattivati durante la personalizzazione.

## L&#39;utente di sincronizzazione è assegnato alla soluzione Marketo {#sync-user-is-assigned-to-the-marketo-solution}

Se disponete di un ![—](assets/delete.png) qui, accertatevi che l&#39;utente Sinc. sia assegnato nella pagina Marketo Predefinito di Microsoft Dynamics.

1. In Dynamics, fai clic sull&#39;icona Impostazioni e seleziona Impostazioni **** avanzate.

   ![](assets/one.png)

1. Fare clic su **Settings **e selezionare **Marketing Config**.

   ![](assets/thirteen.png)

1. Verificare che l&#39;utente di sincronizzazione sia assegnato come predefinito.

   ![](assets/fourteen.png)

## Sincronizza utente con nome utente e password {#sync-user-matches-username-and-password}

Se disponete di un ![—](assets/delete.png) qui, accertatevi di assegnare l&#39;utente di sincronizzazione corretto nel campo Utente marketing nel passaggio Configurazione predefinita configurazione configurazione Marketo in Microsoft Dynamics.

>[!NOTE]
>
>**Articoli correlati**
>
>[Convalida della sincronizzazione di Microsoft Dynamics](../../../../../product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync.md)

