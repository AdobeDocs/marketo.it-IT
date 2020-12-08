---
unique-page-id: 1147031
description: Elimina persona da SFDC - Marketo Docs - Documentazione prodotto
title: Elimina persona da SFDC
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 0%

---


# Elimina persona da SFDC {#delete-person-from-sfdc}

Se devi rimuovere un set specifico di lead da Salesforce ma lasciarli come utenti in Marketo, puoi utilizzare l’azione di flusso Elimina persona da SFDC.

>[!NOTE]
>
>**FYI**
>
>Marketo sta standardizzando la lingua tra tutte le iscrizioni, pertanto è possibile che nell&#39;abbonamento siano presenti lead/lead e persone in docs.marketo.com. Questi termini significano la stessa cosa; non influisce sulle istruzioni dell&#39;articolo. Ci sono anche altri cambiamenti. [Ulteriori](http://docs.marketo.com/display/DOCS/Updates+to+Marketo+Terminology)informazioni.

>[!NOTE]
>
>Disponibile solo se integrato con Salesforce.

1. Nel database, fai clic sulla persona da rimuovere da Salesforce. Quindi fai clic su Azioni **** persona e seleziona **Salesforce**.

   ![](assets/person-actions-salesforce.png)

1. Selezionare **Elimina persona da SFDC**.

   ![](assets/delete-person-from-sfdc.png)

1. Accertatevi che l&#39;impostazione **Elimina in Marketo** sia **false**, quindi fate clic su **Esegui ora**.

   ![](assets/run-action-delete-lead-from-sfdc.png)

   Una volta eseguito il passaggio del flusso, la persona non sarà più un lead in Salesforce ma rimarrà in Marketo.

   >[!CAUTION]
   >
   >Se imposti **Elimina in Marketo** su **true** e elimini le persone da Marketo e i lead da Salesforce, saranno eliminati per sempre. Questo non può essere annullato.

