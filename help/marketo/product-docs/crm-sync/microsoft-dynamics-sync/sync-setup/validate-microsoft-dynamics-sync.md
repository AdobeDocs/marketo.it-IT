---
unique-page-id: 8783322
description: Convalida sincronizzazione Microsoft Dynamics - Documentazione Marketo - Documentazione del prodotto
title: Convalida sincronizzazione Microsoft Dynamics
exl-id: 00297a8d-36c3-42f6-a9b8-4a8dd7c1f30d
feature: Microsoft Dynamics
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---

# Convalida sincronizzazione Microsoft Dynamics {#validate-microsoft-dynamics-sync}

>[!CAUTION]
>
>Se per Dynamics Sync è abilitato Multi-Factor Authentication (MFA), è necessario disattivarlo per consentire la corretta sincronizzazione di Dynamics con Marketo. Per ulteriori informazioni, contattare [Supporto Marketo](https://nation.marketo.com/t5/Support/ct-p/Support).

## Eseguire Convalida sincronizzazione in Marketo {#run-validate-sync-in-marketo}

È molto importante eseguire lo strumento Convalida sincronizzazione per verificare che Microsoft Dynamics Sync con Marketo sia configurato correttamente prima di stabilire la connessione finale tra di essi. Il processo genera un elenco di controllo di sette passaggi di configurazione che individuano dove sono presenti i problemi. La verifica che siano state eseguite correttamente può risparmiare molto tempo in un secondo momento.

1. Fai clic su **Amministratore** e quindi la scheda **Microsoft Dynamics** nell’area Integrazione.

   ![](assets/image2015-9-28-16-3a7-3a51.png)

1. Seleziona **Microsoft**.

   ![](assets/image2015-9-28-16-3a10-3a47.png)

1. Fai clic su **Convalida impostazione sincronizzazione** scheda.

   ![](assets/image2015-9-28-16-3a11-3a45.png)

1. Inserisci il nome utente, la password e l’URL (l’ID client e il segreto client sono facoltativi). Clic **Successivo** al termine.

   ![](assets/four-1.png)

   >[!NOTE]
   >
   >Se hai già eseguito la sincronizzazione, **CRM** nell’albero a sinistra verrà letto **Microsoft Dynamics** e i dati nel modulo di cui sopra possono essere precompilati.

1. Se tutto funziona correttamente, la funzione Convalida sincronizzazione genera un elenco di controllo pieno di segni di spunta verdi ![—](assets/check.png).

   ![](assets/image2015-9-22-15-3a58-3a12.png)

1. Se viene visualizzata una ![—](assets/delete.png), questo passaggio presenta un problema. Consulta [Correggi i problemi di sincronizzazione della convalida Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md) per identificare e risolvere il problema. Quindi esegui nuovamente i passaggi di convalida della sincronizzazione fino a quando il risultato non si presenta come nell’immagine precedente.

   >[!CAUTION]
   >
   >Al momento non è supportato l’aggiornamento della sandbox per Marketo Dynamics Sync. Se devi aggiornare la sandbox di Dynamics CRM, sarà necessaria una nuova sandbox di Marketo. Per ulteriori informazioni, contatta l’Adobe Account Team (il tuo Account Manager).

>[!MORELIKETHIS]
>
>[Correggi i problemi di sincronizzazione della convalida Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/sync-setup/validate-microsoft-dynamics-sync/fix-dynamics-validation-sync-issues.md)
