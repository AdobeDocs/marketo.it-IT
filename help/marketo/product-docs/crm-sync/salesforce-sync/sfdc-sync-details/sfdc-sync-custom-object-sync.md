---
unique-page-id: 2953471
description: Sincronizzazione SFDC - Sincronizzazione oggetti personalizzati - Documentazione di Marketo - Documentazione del prodotto
title: Sincronizzazione SFDC - Sincronizzazione oggetto personalizzato
exl-id: e491e0bc-04a9-4e78-97c3-a25b945d546a
feature: Salesforce Integration
source-git-commit: 0087a5e88b8bd9601875f68a2e7cadeebdb5d682
workflow-type: tm+mt
source-wordcount: '236'
ht-degree: 0%

---

# Sincronizzazione SFDC: Sincronizzazione oggetto personalizzata {#sfdc-sync-custom-object-sync}

Anche gli oggetti personalizzati creati nell’istanza Salesforce possono far parte del Marketo Engage. Ecco come configurarlo.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

>[!PREREQUISITES]
>
>Per utilizzare un oggetto personalizzato, è necessario associarlo a un oggetto [lead](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-field-sync.md){target="_blank"}, [contact](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md){target="_blank"} o [account](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md){target="_blank"} in Salesforce.

>[!IMPORTANT]
>
>L&#39;utente di Marketo Sync ha bisogno dell&#39;accesso in lettura all&#39;oggetto personalizzato per elencarlo ed eseguire una sincronizzazione.

## Abilita oggetto personalizzato  {#enable-custom-object}

1. Fai clic su **[!UICONTROL Amministratore]** e sul collegamento **[!UICONTROL Sincronizzazione oggetti Salesforce]**.

   ![](assets/image2015-11-19-10-3a28-3a5.png).

1. Se si tratta del primo oggetto personalizzato, fare clic su **[!UICONTROL Sincronizza schema]**.

   ![](assets/rtaimage-2.png)

1. Fare clic su **[!UICONTROL Disattiva sincronizzazione globale]**.

   ![](assets/image2015-4-22-10-3a45-3a0.png)

   >[!NOTE]
   >
   >Una sincronizzazione iniziale dello schema di oggetti personalizzato di Salesforce potrebbe richiedere alcuni minuti.

   ![](assets/image2015-4-22-10-3a45-3a18.png)

1. Trascina nell’area di lavoro l’oggetto personalizzato da sincronizzare.

   ![](assets/image2015-4-22-10-3a45-3a30.png)

   >[!NOTE]
   >
   >Gli oggetti personalizzati devono avere nomi univoci. Marketo non supporta due oggetti personalizzati diversi con lo stesso nome.

1. Fare clic su **[!UICONTROL Abilita sincronizzazione]**.

   ![](assets/image2015-4-22-10-3a45-3a50.png)

1. Fai di nuovo clic su **[!UICONTROL Abilita sincronizzazione]**.

   ![](assets/image2015-4-22-10-3a46-3a10.png)

   >[!NOTE]
   >
   >Non dimenticare di riattivare la sincronizzazione globale.

1. Torna alla scheda **Salesforce**.

   ![](assets/image2015-4-22-10-3a46-3a25.png)

1. Fare clic su **[!UICONTROL Abilita sincronizzazione]**.

   ![](assets/image2015-4-22-10-3a50-3a26.png)

1. Per visualizzare tutti gli oggetti personalizzati Salesforce, fai clic su **[!UICONTROL Amministratore]** e sul collegamento **[!UICONTROL Sincronizzazione oggetti Salesforce]** (come nel passaggio 1 precedente).

   ![](assets/image2016-6-23-9-3a28-3a23.png)

   >[!NOTE]
   >
   >Marketo supporta solo entità personalizzate collegate a entità standard profonde uno o due livelli.

### Passaggio successivo: {#whats-next}

[Aggiungi/Rimuovi campo oggetto personalizzato come elenco avanzato/vincoli trigger](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target="_blank"}

Eccellente! Ora puoi utilizzare i dati di questo oggetto personalizzato nelle campagne avanzate e negli elenchi avanzati.
