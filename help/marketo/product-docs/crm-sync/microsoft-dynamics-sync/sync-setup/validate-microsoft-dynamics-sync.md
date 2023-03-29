---
unique-page-id: 8783322
description: Convalida Microsoft Dynamics Sync - Documentazione Marketo - Documentazione del prodotto
title: Convalida della sincronizzazione di Microsoft Dynamics
exl-id: 00297a8d-36c3-42f6-a9b8-4a8dd7c1f30d
source-git-commit: 88c4e844f7ce26b12bae8177dd5311813fb4adcb
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---

# Convalida della sincronizzazione di Microsoft Dynamics {#validate-microsoft-dynamics-sync}

>[!CAUTION]
>
>Se per la sincronizzazione di Dynamics è abilitata l’autenticazione a più fattori (MFA), devi disattivarla affinché Dynamics si sincronizzi correttamente con Marketo. Per ulteriori informazioni, contattare [Supporto Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

## Esegui Convalida sincronizzazione in Marketo {#run-validate-sync-in-marketo}

È molto importante eseguire lo strumento Convalida sincronizzazione per verificare che Microsoft Dynamics Sync con Marketo sia configurato correttamente prima di stabilire la connessione finale tra di essi. Il processo genera una lista di controllo di sette passaggi di configurazione che individuano dove esistono problemi. Verificare che siano stati eseguiti correttamente può risparmiare molto tempo in seguito.

1. Fai clic sul pulsante **Amministratore** e quindi la **Microsoft Dynamics** nell&#39;area Integrazione.

   ![](assets/image2015-9-28-16-3a7-3a51.png)

1. Seleziona **Microsoft**.

   ![](assets/image2015-9-28-16-3a10-3a47.png)

1. Fai clic sul pulsante **Convalida configurazione sincronizzazione** scheda .

   ![](assets/image2015-9-28-16-3a11-3a45.png)

1. Immetti il nome utente, la password e l’URL (l’ID client e il segreto client sono facoltativi). Fai clic su **Successivo** al termine.

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >Se hai sincronizzato in precedenza, **CRM** nell&#39;albero di sinistra leggerà **Microsoft Dynamics**, e i dati nel modulo precedente possono essere precompilati.

1. Se tutto va bene, Convalida sincronizzazione genera una lista di controllo piena di segni di spunta verdi ![—](assets/check.png).

   ![](assets/image2015-9-22-15-3a58-3a12.png)

1. Se vedi un ![—](assets/delete.png)Poi quel passaggio ha un problema. Vedi [Correggere i problemi di sincronizzazione della convalida di Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md) per identificare e risolvere il problema. Quindi esegui nuovamente i passaggi di convalida della sincronizzazione fino a ottenere un risultato simile all&#39;immagine precedente.

   >[!CAUTION]
   >
   >Al momento non è supportato l’aggiornamento della sandbox per Marketo Dynamics Sync. Se devi aggiornare la sandbox di Dynamics CRM, sarà necessaria una nuova sandbox Marketo. Per ulteriori informazioni, contatta il team dell&#39;account Adobe (il tuo Account Manager).

>[!MORELIKETHIS]
>
>[Correggere i problemi di sincronizzazione della convalida di Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md)
