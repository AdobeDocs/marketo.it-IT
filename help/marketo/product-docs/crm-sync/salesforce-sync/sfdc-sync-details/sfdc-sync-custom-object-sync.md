---
unique-page-id: 2953471
description: Sincr. SFDC - Sincronizzazione oggetti personalizzata - Documenti Marketo - Documentazione prodotto
title: Sincr. SFDC - Sincronizzazione oggetti personalizzata
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '215'
ht-degree: 0%

---


# Sincr. SFDC: Sincronizzazione oggetti personalizzata {#sfdc-sync-custom-object-sync}

Anche gli oggetti personalizzati creati nell’istanza Salesforce possono far parte di Marketo.  Ecco come impostarlo.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

>[!PREREQUISITES]
>
>Per utilizzare un oggetto personalizzato, deve essere associato a un oggetto [lead](sfdc-sync-lead-sync.md), [](sfdc-sync-contact-sync.md)contactor [](sfdc-sync-account-sync.md)accountobject in Salesforce.

## Abilita oggetto personalizzato  {#enable-custom-object}

1. Fai clic su **Admin** e sul **collegamento** di sincronizzazione** degli oggetti Salesforce.**

   ![](assets/image2015-11-19-10-3a28-3a5.png).

1. Se si tratta del primo oggetto personalizzato, fare clic su **Sincronizza schema.**

   ![](assets/rtaimage-2.png)

1. Fate clic su **Disattiva sincronizzazione globale.**

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

1. Fate clic su **Abilita sincronizzazione.**

   ![](assets/image2015-4-22-10-3a45-3a50.png)

1. Fate di nuovo clic su **Abilita sincronizzazione** .

   ![](assets/image2015-4-22-10-3a46-3a10.png)

   >[!NOTE]
   >
   >**Promemoria**
   >
   >
   >Non dimenticare di riabilitare la sincronizzazione globale!

1. Tornare alla **Salesforce **tab.

   ![](assets/image2015-4-22-10-3a46-3a25.png)

1. Fate clic su **Abilita sincronizzazione.**

   ![](assets/image2015-4-22-10-3a50-3a26.png)

1. Per visualizzare tutti gli oggetti personalizzati Salesforce, fai clic su **Admin** e sul collegamento** Salesforce Objects Sync **link (come nel passaggio 1 precedente).

   ![](assets/image2016-6-23-9-3a28-3a23.png)

   >[!NOTE]
   >
   >Marketo supporta solo entità personalizzate collegate a entità standard con uno o due livelli di profondità.

### Ulteriori informazioni: {#whats-next}

[Aggiungi/rimuovi campo oggetto personalizzato come vincolo di elenco avanzato/trigger](../../../../product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md)

Eccellente! È ora possibile utilizzare i dati di questo oggetto personalizzato in campagne smart ed elenchi smart.

