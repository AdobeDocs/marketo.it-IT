---
unique-page-id: 4719297
description: Attivare/disattivare la sincronizzazione personalizzata degli oggetti - Documenti Marketo - Documentazione del prodotto
title: Attiva/Disattiva la sincronizzazione personalizzata degli oggetti
exl-id: f17d9135-b33e-48c0-9220-131fb437e9e5
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---

# Attiva/disattiva la sincronizzazione personalizzata degli oggetti {#enable-disable-custom-object-sync}

Gli oggetti personalizzati creati nella tua istanza Salesforce possono far parte anche di Marketo. Ecco come configurarlo.

## Attiva/disattiva la sincronizzazione personalizzata degli oggetti {#enable-disable-custom-object-sync-1}

>[!NOTE]
>
>Sono richiesti i diritti di amministratore.

1. Fai clic su **Amministratore**.

   ![](assets/one.png)

1. Nel menu Gestione database fare clic su **Sincronizzazione oggetti Salesforce**.

   ![](assets/two-2.png)

1. Se si tratta del primo oggetto personalizzato, fare clic su **Sincronizza schema.** In caso contrario, fare clic su  **Aggiorna** schema per verificare di disporre della versione più recente.

   ![](assets/image2014-12-10-10-3a14-3a44.png)

1. Se la sincronizzazione globale è in esecuzione, è necessario disattivarla facendo clic su **Disattiva sincronizzazione globale.**

   ![](assets/image2014-12-10-10-3a14-3a54.png)

   >[!NOTE]
   >
   >La sincronizzazione dello schema di oggetti personalizzati Salesforce potrebbe richiedere alcuni minuti.

1. Fare clic su **Aggiorna schema**.

   ![](assets/image2014-12-10-10-3a15-3a7.png)

1. Selezionare l&#39;oggetto da sincronizzare e fare clic su **Abilita sincronizzazione**.

   >[!TIP]
   >
   >Marketo può sincronizzare un oggetto personalizzato solo se ha una relazione diretta con l’oggetto Lead, Contatto o Account in Salesforce.

   ![](assets/image2014-12-10-10-3a15-3a30.png)

1. Fare nuovamente clic su **Abilita sincronizzazione**.

   ![](assets/image2014-12-10-10-3a15-3a40.png)

1. Torna alla scheda **Salesforce** e fai clic su **Abilita sincronizzazione**.

   ![](assets/image2014-12-10-10-3a15-3a49.png)

## Utilizzo degli oggetti personalizzati {#using-your-custom-objects}

>[!NOTE]
>
>Non è possibile utilizzare oggetti personalizzati nelle campagne avanzate con i trigger.

1. Nell’elenco avanzato, trascina il filtro **Con opportunità** e imposta su **true**.

   ![](assets/image2015-8-26-9-3a39-3a28.png)

1. Quindi, utilizza i vincoli del filtro per restringere lo stato attivo.

   ![](assets/image2015-8-24-14-3a18-3a53.png)

   Eccellente! È ora possibile utilizzare i dati di questo oggetto personalizzato nelle campagne avanzate e negli elenchi smart.

>[!MORELIKETHIS]
>
>[Aggiungi/rimuovi campo di oggetto personalizzato come vincoli di elenco avanzato/trigger](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/optional-steps/add-remove-custom-object-field-as-smart-list-trigger-constraints.md)
