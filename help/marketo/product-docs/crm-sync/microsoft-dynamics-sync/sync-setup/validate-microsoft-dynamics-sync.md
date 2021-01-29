---
unique-page-id: 8783322
description: Convalida di Microsoft Dynamics Sync - Documenti Marketo - Documentazione prodotto
title: Convalida della sincronizzazione di Microsoft Dynamics
translation-type: tm+mt
source-git-commit: 20d4c8a079916f47267df3dab5a8e663f6eb019b
workflow-type: tm+mt
source-wordcount: '266'
ht-degree: 0%

---


# Convalida sincronizzazione Microsoft Dynamics {#validate-microsoft-dynamics-sync}

>[!CAUTION]
>
>Se per la sincronizzazione di Dynamics è abilitata l&#39;autenticazione a più fattori (MFA), devi disabilitarla affinché Dynamics si sincronizzi correttamente con Marketo. Per ulteriori informazioni, contattare [Supporto marketing](https://nation.marketo.com/t5/Support/ct-p/Support).

## Eseguire Convalida sincronizzazione in Marketo {#run-validate-sync-in-marketo}

È molto importante eseguire lo strumento Convalida sincronizzazione per assicurarsi che Microsoft Dynamics Sync con Marketo sia configurato correttamente prima di stabilire la connessione finale tra di essi. Il processo genera un elenco di controllo composto da sette passaggi di configurazione che individuano dove esistono dei problemi. La verifica corretta di tali operazioni può consentire di risparmiare molto tempo in seguito.

1. Fare clic sulla scheda **Amministratore**, quindi sul collegamento **Microsoft Dynamics** nell&#39;area Integrazione.

   ![](assets/image2015-9-28-16-3a7-3a51.png)

1. Selezionare **Microsoft**.

   ![](assets/image2015-9-28-16-3a10-3a47.png)

1. Fare clic sulla scheda **Convalida impostazione sincronizzazione**.

   ![](assets/image2015-9-28-16-3a11-3a45.png)

1. Immettete il vostro nome utente, la password e l’URL (l’ID client e il Segreto cliente sono facoltativi). Fare clic su **Next** al termine.

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >Se hai sincronizzato in precedenza, **CRM** nella struttura a sinistra leggerà **Microsoft Dynamics** e i dati nel modulo precedente potrebbero essere precompilati.

1. Se tutto va bene, Convalida sincronizzazione genera un elenco di controllo pieno di segni di spunta verdi ![—](assets/check.png).

   ![](assets/image2015-9-22-15-3a58-3a12.png)

1. Se viene visualizzato un ![—](assets/delete.png), il passaggio presenta un problema. Per identificare e risolvere il problema, vedere [Correggi problemi di sincronizzazione convalida delle dinamiche](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md). Quindi, eseguite nuovamente i passaggi di convalida della sincronizzazione fino a ottenere un risultato simile a quello dell&#39;immagine precedente.

   >[!CAUTION]
   >
   >Al momento non è supportato l&#39;aggiornamento sandbox per Marketo Dynamics Sync. Se devi aggiornare la sandbox di Dynamics CRM, sarà necessaria una nuova sandbox di Marketo. Contatta il tuo Customer Success Manager per ulteriori informazioni.

>[!MORELIKETHIS]
>
>[Correggi problemi di sincronizzazione convalida delle dinamiche](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md)
