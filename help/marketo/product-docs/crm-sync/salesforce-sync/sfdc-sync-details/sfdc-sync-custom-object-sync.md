---
unique-page-id: 2953471
description: Sincronizzazione SFDC - Sincronizzazione oggetti personalizzati - Documenti Marketo - Documentazione del prodotto
title: Sincronizzazione SFDC - Sincronizzazione oggetto personalizzato
exl-id: e491e0bc-04a9-4e78-97c3-a25b945d546a
feature: Salesforce Integration
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '277'
ht-degree: 2%

---

# Sincronizzazione SFDC: sincronizzazione oggetto personalizzato {#sfdc-sync-custom-object-sync}

Anche gli oggetti personalizzati creati nell&#39;istanza [!DNL Salesforce] possono far parte di Marketo.  Ecco come configurarlo.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

>[!PREREQUISITES]
>
>Per utilizzare un oggetto personalizzato, è necessario associarlo a un oggetto [lead](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-field-sync.md), [contact](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md) o [account](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md) in [!DNL Salesforce].

>[!IMPORTANT]
>
>L&#39;utente di Marketo Sync ha bisogno dell&#39;accesso in lettura all&#39;oggetto personalizzato per elencarlo ed eseguire una sincronizzazione.

## Abilita oggetto personalizzato  {#enable-custom-object}

1. Fare clic su **[!UICONTROL Admin]** e sul collegamento **[!UICONTROL Salesforce Objects Sync]**.

   ![](assets/image2015-11-19-10-3a28-3a5.png).

1. Se si tratta del primo oggetto personalizzato, fare clic su **[!UICONTROL Sync Schema]**.

   ![](assets/rtaimage-2.png)

1. Fai clic su **[!UICONTROL Disable Global Sync]**.

   ![](assets/image2015-4-22-10-3a45-3a0.png)

   >[!NOTE]
   >
   >La sincronizzazione iniziale dello schema di oggetti personalizzato [!DNL Salesforce] potrebbe richiedere alcuni minuti.

   ![](assets/image2015-4-22-10-3a45-3a18.png)

1. Trascina nell’area di lavoro l’oggetto personalizzato da sincronizzare.

   ![](assets/image2015-4-22-10-3a45-3a30.png)

   >[!NOTE]
   >
   >Gli oggetti personalizzati devono avere nomi univoci. Marketo non supporta due oggetti personalizzati diversi con lo stesso nome.

1. Fai clic su **[!UICONTROL Enable Sync]**.

   ![](assets/image2015-4-22-10-3a45-3a50.png)

1. Fare di nuovo clic su **[!UICONTROL Enable Sync]**.

   ![](assets/image2015-4-22-10-3a46-3a10.png)

   >[!NOTE]
   >
   >Non dimenticare di riattivare la sincronizzazione globale.

1. Torna alla scheda **[!UICONTROL Salesforce]**.

   ![](assets/image2015-4-22-10-3a46-3a25.png)

1. Fai clic su **[!UICONTROL Enable Sync]**.

   ![](assets/image2015-4-22-10-3a50-3a26.png)

1. Per visualizzare tutti gli oggetti personalizzati di [!DNL Salesforce], fare clic su **[!UICONTROL Admin]** e sul collegamento **[!UICONTROL Salesforce Objects Sync]** (come nel passaggio 1 precedente).

   ![](assets/image2016-6-23-9-3a28-3a23.png)

   >[!NOTE]
   >
   >* Marketo supporta solo entità personalizzate collegate a entità standard profonde uno o due livelli.
   >
   >* La struttura ad oggetti personalizzata può mostrare lo stesso oggetto più di una volta, a causa delle sue connessioni dirette con uno degli oggetti principali (ad esempio lead, contatti o account o connessioni indirette attraverso un oggetto intermedio). In questi casi, scegliere l&#39;oggetto più vicino all&#39;oggetto principale e sceglierne solo uno. La scelta dello stesso oggetto più volte può ostacolare la sincronizzazione dell&#39;oggetto personalizzato.

### Passaggio successivo: {#whats-next}

[Aggiungi/Rimuovi campo oggetto personalizzato come elenco avanzato/vincoli trigger](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target="_blank"}

Eccellente! Ora puoi utilizzare i dati di questo oggetto personalizzato nelle campagne avanzate e negli elenchi avanzati.
