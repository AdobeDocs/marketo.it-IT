---
unique-page-id: 2953471
description: Sincr. SFDC - Sincronizzazione oggetti personalizzata - Documenti Marketo - Documentazione del prodotto
title: Sincronizzazione SFDC - Sincronizzazione oggetti personalizzata
exl-id: e491e0bc-04a9-4e78-97c3-a25b945d546a
source-git-commit: e04e2d6932830535493c431de50d6cf9e2298fb1
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Sincr. SFDC: Sincronizzazione oggetti personalizzata {#sfdc-sync-custom-object-sync}

Gli oggetti personalizzati creati nella tua istanza Salesforce possono far parte anche di Marketo.  Ecco come configurarlo.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

>[!PREREQUISITES]
>
>Per utilizzare un oggetto personalizzato, è necessario associarlo a un [lead](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-field-sync.md), [contatta](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-contact-sync.md)oppure [account](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/sfdc-sync-account-sync.md) oggetto in Salesforce.

## Abilita oggetto personalizzato  {#enable-custom-object}

1. Fai clic su **Amministratore** e **Sincronizzazione oggetti Salesforce** link.

   ![](assets/image2015-11-19-10-3a28-3a5.png).

1. Se si tratta del primo oggetto personalizzato, fare clic su **Schema di sincronizzazione**.

   ![](assets/rtaimage-2.png)

1. Fai clic su **Disattiva sincronizzazione globale**.

   ![](assets/image2015-4-22-10-3a45-3a0.png)

   >[!NOTE]
   >
   >La sincronizzazione iniziale dello schema di oggetti personalizzati Salesforce potrebbe richiedere alcuni minuti.

   ![](assets/image2015-4-22-10-3a45-3a18.png)

1. Trascina l’oggetto personalizzato da sincronizzare nell’area di lavoro.

   ![](assets/image2015-4-22-10-3a45-3a30.png)

   >[!NOTE]
   >
   >Gli oggetti personalizzati devono avere nomi univoci. Marketo non supporta due oggetti personalizzati diversi con lo stesso nome.

1. Fai clic su **Abilita sincronizzazione**.

   ![](assets/image2015-4-22-10-3a45-3a50.png)

1. Fai clic su **Abilita sincronizzazione** di nuovo.

   ![](assets/image2015-4-22-10-3a46-3a10.png)

   >[!NOTE]
   >
   >Non dimenticare di riabilitare la sincronizzazione globale.

1. Torna alla pagina **Salesforce** scheda .

   ![](assets/image2015-4-22-10-3a46-3a25.png)

1. Fai clic su **Abilita sincronizzazione**.

   ![](assets/image2015-4-22-10-3a50-3a26.png)

1. Per visualizzare tutti gli oggetti personalizzati Salesforce, fai clic su **Amministratore** e **Sincronizzazione oggetti Salesforce** collegamento (come nel precedente passaggio 1).

   ![](assets/image2016-6-23-9-3a28-3a23.png)

   >[!NOTE]
   >
   >Marketo supporta solo entità personalizzate collegate a entità standard con uno o due livelli di profondità.

### Novità: {#whats-next}

[Aggiungi/rimuovi campo di oggetto personalizzato come vincoli di elenco avanzato/trigger](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md)

Eccellente! È ora possibile utilizzare i dati di questo oggetto personalizzato nelle campagne avanzate e negli elenchi smart.
