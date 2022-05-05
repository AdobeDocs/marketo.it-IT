---
description: Sincronizzazione oggetti personalizzata - Documenti Marketo - Documentazione del prodotto
title: Sincronizzazione oggetti personalizzata
hide: true
hidefromtoc: true
exl-id: 68bc14e7-dfc9-4dce-b159-24d734ee3c6f
source-git-commit: 2ce44b7c44517a6fdb3f616a3d69b25158ea4ec9
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 0%

---

# Sincronizzazione oggetti personalizzata {#custom-object-sync}

Anche gli oggetti personalizzati creati nella tua istanza CRM di Veeva possono far parte del Marketo Engage. Ecco come configurarlo.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

>[!PREREQUISITES]
>
>Per utilizzare un oggetto personalizzato, deve essere associato a un contatto o a un oggetto account in Veeva CRM.

## Abilita oggetto personalizzato {#enable-custom-object}

1. In Marketo, fai clic su **Amministratore**, quindi **Sincronizzazione oggetti Veeva**.

   ![](assets/custom-object-sync-1.png)

1. Se si tratta del primo oggetto personalizzato, fare clic su **Schema di sincronizzazione**.

   ![](assets/custom-object-sync-2.png)

1. Fai clic su **Disattiva sincronizzazione globale**.

   ![](assets/custom-object-sync-3.png)

   >[!NOTE]
   >
   >La sincronizzazione iniziale dello schema di oggetti personalizzati Veeva potrebbe richiedere alcuni minuti.

1. Trascina l’oggetto personalizzato da sincronizzare nell’area di lavoro.

   ![](assets/custom-object-sync-4.png)

   >[!NOTE]
   >
   >Gli oggetti personalizzati devono avere nomi univoci. Marketo non supporta due oggetti personalizzati diversi con lo stesso nome.

1. Fai clic su **Abilita sincronizzazione**.

   ![](assets/custom-object-sync-5.png)

1. Fai clic su **Abilita sincronizzazione** di nuovo.

   ![](assets/custom-object-sync-6.png)

1. Torna alla pagina **Veeva** scheda .

   ![](assets/custom-object-sync-7.png)

1. Fai clic su **Abilita sincronizzazione**.

   ![](assets/custom-object-sync-8.png)

1. Per visualizzare tutti gli oggetti personalizzati Veeva, fare clic su Sincronizzazione oggetti amministrazione e veeva.

   ![](assets/custom-object-sync-9.png)

   >[!NOTE]
   >
   >Marketo supporta solo le entità personalizzate collegate a entità standard con profondità compresa tra uno e due livelli.

Eccellente! È ora possibile utilizzare i dati di questo oggetto personalizzato in Smart Campaigns ed Elenchi avanzati.

>[!MORELIKETHIS]
>
>* [Sincronizzazione dei messaggi chiave di chiamata e chiamata](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target=&quot;_blank&quot;}
>* [Aggiungi/rimuovi campo di oggetto personalizzato come vincoli di elenco avanzato/trigger](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target=&quot;_blank&quot;}

