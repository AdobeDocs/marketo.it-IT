---
unique-page-id: 1147031
description: Elimina persona da SFDC - Marketo Docs - Documentazione prodotto
title: Elimina persona da SFDC
translation-type: tm+mt
source-git-commit: 5b9f48c98464c79bcdca2e335f6a4a2edce98ce4
workflow-type: tm+mt
source-wordcount: '135'
ht-degree: 0%

---


# Elimina persona da SFDC {#delete-person-from-sfdc}

Se devi rimuovere un set specifico di lead da Salesforce ma lasciarli come utenti in Marketo, puoi utilizzare l’azione di flusso Elimina persona da SFDC.

>[!NOTE]
>
>Disponibile solo se integrato con Salesforce.

1. Nel database, fai clic sulla persona da rimuovere da Salesforce. Fare clic su **Azioni persona** e selezionare **Salesforce**.

   ![](assets/person-actions-salesforce.png)

1. Selezionare **Elimina persona da SFDC**.

   ![](assets/delete-person-from-sfdc.png)

1. Assicurarsi che l&#39;impostazione **Elimina in Marketo** sia **false**, quindi fare clic su **Esegui ora**.

   ![](assets/run-action-delete-lead-from-sfdc.png)

   Una volta eseguito il passaggio del flusso, la persona non sarà più un lead in Salesforce ma rimarrà in Marketo.

   >[!CAUTION]
   >
   >Se si imposta **Elimina in Marketo** su **true** ed elimina le persone da Marketo e i lead da Salesforce, questi non saranno più disponibili per sempre. Questo non può essere annullato.
