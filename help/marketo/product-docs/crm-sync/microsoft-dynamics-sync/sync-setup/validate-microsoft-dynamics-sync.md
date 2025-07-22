---
unique-page-id: 8783322
description: Convalida [!DNL Microsoft Dynamics] Sincronizzazione - Documenti Marketo - Documentazione del prodotto
title: Convalida [!DNL Microsoft Dynamics] Sincronizzazione
exl-id: 00297a8d-36c3-42f6-a9b8-4a8dd7c1f30d
feature: Microsoft Dynamics
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---

# Convalida sincronizzazione [!DNL Microsoft Dynamics] {#validate-microsoft-dynamics-sync}

>[!CAUTION]
>
>Se Multi-Factor Authentication (MFA) è abilitato per la sincronizzazione di [!DNL Dynamics], è necessario disattivarlo affinché [!DNL Dynamics] possa essere sincronizzato correttamente con Marketo. Per ulteriori informazioni, contattare il [Supporto Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

## Eseguire Convalida sincronizzazione in Marketo {#run-validate-sync-in-marketo}

È molto importante eseguire lo strumento Convalida sincronizzazione per assicurarsi che la sincronizzazione di [!DNL Microsoft Dynamics] con Marketo sia configurata correttamente prima di stabilire la connessione finale tra di loro. Il processo genera un elenco di controllo di sette passaggi di configurazione che individuano dove sono presenti i problemi. La verifica che siano state eseguite correttamente può risparmiare molto tempo in un secondo momento.

1. Fare clic sulla scheda **[!UICONTROL Admin]** e quindi sul collegamento **[!DNL Microsoft Dynamics]** nell&#39;area di integrazione.

   ![](assets/image2015-9-28-16-3a7-3a51.png)

1. Seleziona **[!DNL Microsoft]**.

   ![](assets/image2015-9-28-16-3a10-3a47.png)

1. Fare clic sulla scheda **[!UICONTROL Validate Sync Setup]**.

   ![](assets/image2015-9-28-16-3a11-3a45.png)

1. Inserisci il nome utente, la password e l’URL (l’ID client e il segreto client sono facoltativi). Al termine, fai clic su **[!UICONTROL Next]**.

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >Se è già stata eseguita la sincronizzazione, **CRM** nella struttura a sinistra leggerà **[!DNL Microsoft Dynamics]** e i dati nel modulo precedente potrebbero essere precompilati.

1. Se tutto funziona correttamente, la funzione di convalida sincronizzazione genera un elenco di controllo pieno di segni di spunta verdi ![—](assets/check.png).

   ![](assets/image2015-9-22-15-3a58-3a12.png)

1. Se vedi un ![—](assets/delete.png), quel passaggio presenta un problema. Consulta [Correzione [!DNL Dynamics] Problemi di sincronizzazione della convalida](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md) per identificare e risolvere il problema. Quindi esegui nuovamente i passaggi di convalida della sincronizzazione fino a quando il risultato non si presenta come nell’immagine precedente.

   >[!CAUTION]
   >
   >Al momento non è supportato l&#39;aggiornamento della sandbox per la sincronizzazione [!DNL Marketo Dynamics]. Se è necessario aggiornare la sandbox CRM di [!DNL Dynamics], sarà necessaria una nuova sandbox Marketo. Per ulteriori informazioni, contatta il tuo Customer Success Manager.

>[!MORELIKETHIS]
>
>[Correzione [!DNL Dynamics] Problemi di sincronizzazione convalida](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md)
