---
description: Attivare/disattivare la sincronizzazione personalizzata degli oggetti - Documenti Marketo - Documentazione del prodotto
title: Attiva/Disattiva la sincronizzazione personalizzata degli oggetti
exl-id: 01417fb6-70f5-449b-ad56-42e1c0b2ff68
source-git-commit: 2ce44b7c44517a6fdb3f616a3d69b25158ea4ec9
workflow-type: tm+mt
source-wordcount: '218'
ht-degree: 0%

---

# Attiva/Disattiva la sincronizzazione personalizzata degli oggetti {#enable-disable-custom-object-sync}

Anche gli oggetti personalizzati creati nella tua istanza CRM di Veeva possono far parte del Marketo Engage. Ecco come configurarlo.

## Attiva o disattiva la sincronizzazione degli oggetti personalizzati {#enable-or-disable-the-custom-object-sync}

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

1. In Marketo, fai clic su **Amministratore**, quindi **Sincronizzazione oggetti Veeva**.

   ![](assets/enable-disable-custom-object-sync-1.png)

1. Se si tratta del primo oggetto personalizzato, fare clic su Sincronizza schema. In caso contrario, fai clic su **Aggiorna schema** per essere certo di avere le ultime notizie.

   ![](assets/enable-disable-custom-object-sync-2.png)

1. Se la sincronizzazione globale è in esecuzione, disattivala facendo clic su **Disattiva sincronizzazione globale**.

   ![](assets/enable-disable-custom-object-sync-3.png)

   >[!NOTE]
   >
   >La sincronizzazione dello schema di oggetti personalizzati Veeva potrebbe richiedere alcuni minuti.

1. Fai clic su **Aggiorna schema**.

   ![](assets/enable-disable-custom-object-sync-4.png)

Selezionare l&#39;oggetto da sincronizzare e fare clic su Abilita sincronizzazione.

![](assets/enable-disable-custom-object-sync-5.png)

>[!TIP]
>
>Marketo può sincronizzare un oggetto personalizzato solo se ha una relazione diretta con l&#39;oggetto Contact o Account in Veeva CRM.

1. Fai clic su **Abilita sincronizzazione** di nuovo.

   ![](assets/enable-disable-custom-object-sync-6.png)

1. Torna alla scheda Veeva e fai clic su **Abilita sincronizzazione**.

   ![](assets/enable-disable-custom-object-sync-7.png)

## Utilizzo degli oggetti personalizzati {#using-your-custom-objects}

>[!NOTE]
>
>Non è possibile utilizzare oggetti personalizzati nelle campagne avanzate con i trigger.

1. Nell’elenco avanzato, trascina il filtro &quot;Ha opportunità&quot; e imposta su **True**.

   ![](assets/enable-disable-custom-object-sync-8.png)

1. Facoltativamente, utilizza i vincoli di filtro per restringere lo stato attivo.

   ![](assets/enable-disable-custom-object-sync-9.png)

Eccellente! È ora possibile utilizzare i dati dell’oggetto personalizzato nelle campagne avanzate e negli elenchi avanzati.

>[!MORELIKETHIS]
>
>[Aggiungi/rimuovi campo di oggetto personalizzato come vincoli di elenco avanzato/trigger](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target=&quot;_blank&quot;}
