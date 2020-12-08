---
unique-page-id: 4719297
description: Attiva/Disattiva sincronizzazione oggetti personalizzata - Documenti Marketo - Documentazione prodotto
title: Attiva/Disattiva sincronizzazione oggetti personalizzata
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 0%

---


# Attiva/Disattiva sincronizzazione oggetti personalizzata {#enable-disable-custom-object-sync}

Anche gli oggetti personalizzati creati nell’istanza Salesforce possono far parte di Marketo. Ecco come impostarlo.

## Attiva/Disattiva sincronizzazione oggetti personalizzata {#enable-disable-custom-object-sync-1}

>[!NOTE]
>
>Diritti di amministratore richiesti.

1. Fate clic su **Admin**.

   ** ![](assets/one.png)

   **

1. Nel menu Gestione del database, fate clic su Sincronizzazione **** Salesforce **** Objects.

   ![](assets/two-2.png)

1. Se si tratta del primo oggetto personalizzato, fare clic su **Sincronizza schema.** In caso contrario, fare clic su **Aggiorna schema** per verificare di disporre della versione più recente.

   ![](assets/image2014-12-10-10-3a14-3a44.png)

1. Se la sincronizzazione globale è in esecuzione, sarà necessario disattivarla facendo clic su **Disattiva sincronizzazione globale.**

   ![](assets/image2014-12-10-10-3a14-3a54.png)

   >[!NOTE]
   >
   >La sincronizzazione dello schema oggetto personalizzato di Salesforce potrebbe richiedere alcuni minuti.

1. Fare clic su **Aggiorna schema**.

   ![](assets/image2014-12-10-10-3a15-3a7.png)

1. Selezionate l’oggetto da sincronizzare e fate clic su **Attiva sincronizzazione**.

   >[!TIP]
   >
   >Marketo può sincronizzare un oggetto personalizzato solo se ha una relazione diretta con l&#39;oggetto Lead, Contatto o Account in Salesforce.

   ![](assets/image2014-12-10-10-3a15-3a30.png)

1. Fate di nuovo clic su **Abilita sincronizzazione** .

   ** ![](assets/image2014-12-10-10-3a15-3a40.png)

   **

1. Torna alla scheda **Salesforce** e fai clic su **Abilita sincronizzazione**.

   ![](assets/image2014-12-10-10-3a15-3a49.png)

## Utilizzo degli oggetti personalizzati {#using-your-custom-objects}

>[!NOTE]
>
>Non è possibile utilizzare oggetti personalizzati nelle campagne smart con i trigger.

1. Nell’elenco avanzato, trascinate il mouse sul **filtro** Con opportunità e impostate su **true**.

   ![](assets/image2015-8-26-9-3a39-3a28.png)

1. Quindi, utilizzate i vincoli del filtro per restringere la messa a fuoco.

   ![](assets/image2015-8-24-14-3a18-3a53.png)

   Eccellente! È ora possibile utilizzare i dati di questo oggetto personalizzato nelle campagne smart ed elenchi smart.

>[!NOTE]
>
>**Articoli correlati**
>
>* [Aggiungi/rimuovi campo oggetto personalizzato come vincolo di elenco avanzato/trigger](add-remove-custom-object-field-as-smart-list-trigger-constraints.md)

>



