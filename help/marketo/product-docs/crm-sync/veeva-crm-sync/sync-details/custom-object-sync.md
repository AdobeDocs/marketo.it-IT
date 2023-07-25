---
description: Sincronizzazione oggetti personalizzati - Documentazione di Marketo - Documentazione del prodotto
title: Sincronizzazione oggetto personalizzato
hide: true
hidefromtoc: true
exl-id: 68bc14e7-dfc9-4dce-b159-24d734ee3c6f
feature: Veeva CRM
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '201'
ht-degree: 0%

---

# Sincronizzazione oggetto personalizzato {#custom-object-sync}

Anche gli oggetti personalizzati creati nell’istanza di CRM Veeva possono far parte del Marketo Engage. Ecco come configurarlo.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

>[!PREREQUISITES]
>
>Per utilizzare un oggetto personalizzato, è necessario associarlo a un oggetto contatto o account in Veeva CRM.

## Abilita oggetto personalizzato {#enable-custom-object}

1. In Marketo, fai clic su **Amministratore**, quindi **Sincronizzazione oggetti Veeva**.

   ![](assets/custom-object-sync-1.png)

1. Se si tratta del primo oggetto personalizzato, fare clic su **Schema di sincronizzazione**.

   ![](assets/custom-object-sync-2.png)

1. Clic **Disattiva sincronizzazione globale**.

   ![](assets/custom-object-sync-3.png)

   >[!NOTE]
   >
   >La sincronizzazione iniziale dello schema di oggetti personalizzato Veeva potrebbe richiedere alcuni minuti.

1. Trascina nell’area di lavoro l’oggetto personalizzato da sincronizzare.

   ![](assets/custom-object-sync-4.png)

   >[!NOTE]
   >
   >Gli oggetti personalizzati devono avere nomi univoci. Marketo non supporta due oggetti personalizzati diversi con lo stesso nome.

1. Clic **Abilita sincronizzazione**.

   ![](assets/custom-object-sync-5.png)

1. Clic **Abilita sincronizzazione** di nuovo.

   ![](assets/custom-object-sync-6.png)

1. Torna a **Veeva** scheda.

   ![](assets/custom-object-sync-7.png)

1. Clic **Abilita sincronizzazione**.

   ![](assets/custom-object-sync-8.png)

1. Per visualizzare tutti gli oggetti personalizzati di Veeva, fare clic su Sincronizzazione oggetti amministratore e visualizzazione.

   ![](assets/custom-object-sync-9.png)

   >[!NOTE]
   >
   >Marketo supporta solo entità personalizzate collegate alle entità standard con profondità da uno a due livelli.

Eccellente! È ora possibile utilizzare i dati di questo oggetto personalizzato nelle campagne avanzate e negli elenchi avanzati.

>[!MORELIKETHIS]
>
>* [Sincronizzazione dei messaggi chiave di chiamata e chiamata](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/syncing-call-and-call-key-messages.md){target="_blank"}
>* [Aggiungi/Rimuovi campo oggetto personalizzato come vincoli di elenco avanzato/trigger](/help/marketo/product-docs/crm-sync/veeva-crm-sync/sync-details/add-remove-custom-object-field-as-smart-list-trigger-constraints.md){target="_blank"}
