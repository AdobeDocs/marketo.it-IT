---
unique-page-id: 2953471
description: Sincr. SFDC - Sincronizzazione oggetti personalizzata - Documenti Marketo - Documentazione prodotto
title: Sincr. SFDC - Sincronizzazione oggetti personalizzata
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '214'
ht-degree: 0%

---


# Sincr. SFDC: Sincronizzazione oggetti personalizzata {#sfdc-sync-custom-object-sync}

Anche gli oggetti personalizzati creati nell’istanza Salesforce possono far parte di Marketo.  Ecco come impostarlo.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

>[!PREREQUISITES]
>
>Per utilizzare un oggetto personalizzato, deve essere associato a un oggetto [lead](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-field-sync.md), [contact](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md) o [account](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md) in Salesforce.

## Abilita oggetto personalizzato {#enable-custom-object}

1. Fare clic su **Admin** e sul collegamento **Salesforce Objects Sync**.

   ![](assets/image2015-11-19-10-3a28-3a5.png).

1. Se si tratta del primo oggetto personalizzato, fare clic su **Sincronizza schema**.

   ![](assets/rtaimage-2.png)

1. Fare clic su **Disattiva sincronizzazione globale**.

   ![](assets/image2015-4-22-10-3a45-3a0.png)

   >[!NOTE]
   >
   >La sincronizzazione iniziale dello schema oggetto personalizzato di Salesforce potrebbe richiedere alcuni minuti.

   ![](assets/image2015-4-22-10-3a45-3a18.png)

1. Trascinate l’oggetto personalizzato da sincronizzare nel quadro.

   ![](assets/image2015-4-22-10-3a45-3a30.png)

   >[!NOTE]
   >
   >Gli oggetti personalizzati devono avere nomi univoci. Marketo non supporta due diversi oggetti personalizzati con lo stesso nome.

1. Fare clic su **Abilita sincronizzazione**.

   ![](assets/image2015-4-22-10-3a45-3a50.png)

1. Fare di nuovo clic su **Abilita sincronizzazione**.

   ![](assets/image2015-4-22-10-3a46-3a10.png)

   >[!NOTE]
   >
   >Non dimenticare di riabilitare la sincronizzazione globale!

1. Torna alla scheda **Salesforce**.

   ![](assets/image2015-4-22-10-3a46-3a25.png)

1. Fare clic su **Abilita sincronizzazione**.

   ![](assets/image2015-4-22-10-3a50-3a26.png)

1. Per visualizzare tutti gli oggetti personalizzati Salesforce, fai clic su **Admin** e sul collegamento **Salesforce Objects Sync** (come nel passaggio 1 sopra).

   ![](assets/image2016-6-23-9-3a28-3a23.png)

   >[!NOTE]
   >
   >Marketo supporta solo entità personalizzate collegate a entità standard con uno o due livelli di profondità.

### Ulteriori informazioni: {#whats-next}

[Aggiungi/rimuovi campo oggetto personalizzato come vincolo di elenco avanzato/trigger](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md)

Eccellente! È ora possibile utilizzare i dati di questo oggetto personalizzato in campagne smart ed elenchi smart.
