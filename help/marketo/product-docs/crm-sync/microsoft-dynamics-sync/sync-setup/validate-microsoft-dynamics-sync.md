---
unique-page-id: 8783322
description: Convalida di Microsoft Dynamics Sync - Documenti Marketo - Documentazione prodotto
title: Convalida della sincronizzazione di Microsoft Dynamics
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 0%

---


# Convalida della sincronizzazione di Microsoft Dynamics {#validate-microsoft-dynamics-sync}

>[!CAUTION]
>
>Se per la sincronizzazione di Dynamics è abilitata l&#39;autenticazione a più fattori (MFA), devi disabilitarla affinché Dynamics si sincronizzi correttamente con Marketo. Per ulteriori informazioni, contattate [il supporto](http://nation.marketo.com/community/support_solutions)di Marketo.

## Eseguire Convalida sincronizzazione in Marketo {#run-validate-sync-in-marketo}

È molto importante eseguire lo strumento Convalida sincronizzazione per assicurarsi che Microsoft Dynamics Sync con Marketo sia configurato correttamente prima di stabilire la connessione finale tra di essi. Il processo genera un elenco di controllo composto da sette passaggi di configurazione che individuano dove esistono dei problemi. La verifica corretta di tali operazioni può consentire di risparmiare molto tempo in seguito.

1. Fare clic sulla scheda **Admin** , quindi sul collegamento **Microsoft Dynamics** nell&#39;area Integrazione.

   ![](assets/image2015-9-28-16-3a7-3a51.png)

1. Selezionare **Microsoft**.

   ![](assets/image2015-9-28-16-3a10-3a47.png)

1. Fate clic sulla scheda **Convalida impostazione** sincronizzazione.

   ![](assets/image2015-9-28-16-3a11-3a45.png)

1. Immettete il vostro nome utente, la password e l’URL (l’ID client e il Segreto cliente sono facoltativi). Al termine, fate clic su **Avanti** .

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >Se hai già eseguito la sincronizzazione, **CRM** nella struttura a sinistra leggerà **Microsoft Dynamics** e i dati nel modulo precedente potrebbero essere precompilati.

1. Se tutto va bene, Convalida sincronizzazione genera un elenco di controllo pieno di segni di spunta verdi ![—](assets/check.png).

   ![](assets/image2015-9-22-15-3a58-3a12.png)

1. Se visualizzi un ![—](assets/delete.png), allora quel passaggio ha un problema. Consultate [Correzione dei problemi](validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md) di sincronizzazione convalida delle dinamiche per identificare e risolvere il problema. Quindi, eseguite nuovamente i passaggi di convalida della sincronizzazione fino a ottenere un risultato simile a quello dell&#39;immagine precedente.

   >[!CAUTION]
   >
   >Al momento non è supportato l&#39;aggiornamento sandbox per Marketo Dynamics Sync. Se devi aggiornare la sandbox di Dynamics CRM, sarà necessaria una nuova sandbox di Marketo. Contatta il tuo Customer Success Manager per ulteriori informazioni.

>[!NOTE]
>
>**Articoli correlati**
>
>[Correggi problemi di sincronizzazione convalida delle dinamiche](validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md)

