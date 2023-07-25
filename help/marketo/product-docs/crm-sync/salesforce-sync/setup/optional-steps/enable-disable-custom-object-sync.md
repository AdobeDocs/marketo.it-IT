---
unique-page-id: 4719297
description: Abilitare/Disabilitare la sincronizzazione oggetti personalizzati - Documentazione di Marketo - Documentazione del prodotto
title: Abilita/Disabilita sincronizzazione oggetti personalizzati
exl-id: f17d9135-b33e-48c0-9220-131fb437e9e5
feature: Salesforce Integration
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---

# Abilita/Disabilita sincronizzazione oggetti personalizzati {#enable-disable-custom-object-sync}

Anche gli oggetti personalizzati creati nell’istanza Salesforce possono far parte di Marketo. Ecco come configurarlo.

## Abilita/Disabilita sincronizzazione oggetti personalizzati {#enable-disable-custom-object-sync-1}

>[!NOTE]
>
>Diritti di amministrazione richiesti.

1. Clic **Amministratore**.

   ![](assets/one.png)

1. Nel menu Gestione database fare clic su **Sincronizzazione oggetti Salesforce**.

   ![](assets/two-2.png)

1. Se si tratta del primo oggetto personalizzato, fare clic su **Sincronizza schema.** Altrimenti fai clic su **Aggiorna schema** per avere la versione più recente.

   ![](assets/image2014-12-10-10-3a14-3a44.png)

1. Se la sincronizzazione globale è in esecuzione, è necessario disattivarla facendo clic su **Disattiva sincronizzazione globale.**

   ![](assets/image2014-12-10-10-3a14-3a54.png)

   >[!NOTE]
   >
   >La sincronizzazione dello schema di oggetti personalizzato di Salesforce potrebbe richiedere alcuni minuti.

1. Clic **Aggiorna schema**.

   ![](assets/image2014-12-10-10-3a15-3a7.png)

1. Selezionare l&#39;oggetto da sincronizzare e fare clic su **Abilita sincronizzazione**.

   >[!TIP]
   >
   >Marketo può sincronizzare un oggetto personalizzato solo se ha una relazione diretta con l’oggetto Lead, Contact o Account in Salesforce.

   ![](assets/image2014-12-10-10-3a15-3a30.png)

1. Clic **Abilita sincronizzazione** di nuovo.

   ![](assets/image2014-12-10-10-3a15-3a40.png)

1. Torna a **Salesforce** e fai clic su **Abilita sincronizzazione**.

   ![](assets/image2014-12-10-10-3a15-3a49.png)

## Utilizzo degli oggetti personalizzati {#using-your-custom-objects}

>[!NOTE]
>
>Non è possibile utilizzare oggetti personalizzati nelle campagne intelligenti con trigger.

1. Nell’elenco avanzato, trascina il puntatore del mouse su **Ha un’opportunità** filtra e imposta su **true**.

   ![](assets/image2015-8-26-9-3a39-3a28.png)

1. Quindi, utilizzate i vincoli di filtro per restringere lo stato attivo.

   ![](assets/image2015-8-24-14-3a18-3a53.png)

   Eccellente! Ora puoi utilizzare i dati di questo oggetto personalizzato nelle campagne avanzate e negli elenchi avanzati.

>[!MORELIKETHIS]
>
>[Aggiungi/Rimuovi campo oggetto personalizzato come vincoli di elenco avanzato/trigger](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md)
