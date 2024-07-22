---
unique-page-id: 37355600
description: Disinstallare MSI dall’istanza di MS Dynamics - Documentazione di Marketo - Documentazione del prodotto
title: Disinstallare MSI dall’istanza di MS Dynamics
exl-id: 86e8dbc9-236f-42ad-96e8-cdb1b4c3bed2
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '157'
ht-degree: 0%

---

# Disinstallare MSI dall’istanza di MS Dynamics {#uninstall-msi-from-your-ms-dynamics-instance}

Per disinstallare MSI dall’istanza di MS Dynamics, è necessario eseguire i passaggi sia in Marketo che in MS Dynamics.

>[!PREREQUISITES]
>
>[Disabilita sincronizzazione globale MS Dynamics](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/uninstalling/disable-global-ms-dynamics-sync.md)

1. In Marketo, fai clic su **Amministratore**.

   ![](assets/one-1.png)

1. Fare clic su **Informazioni sulle vendite**.

   ![](assets/six.png)

1. Fare clic su **Modifica sincronizzazione campi**.

   ![](assets/seven.png)

1. Selezionare la casella di controllo **Disattiva sincronizzazione** e fare clic su **Salva**.

   >[!NOTE]
   >
   >Prima di disabilitare la sincronizzazione dei campi, assicurati di [disabilitare Global MS Dynamics Sync](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/uninstalling/disable-global-ms-dynamics-sync.md).

   ![](assets/eight.png)

## Nell’istanza di MS Dynamics vengono eseguiti i seguenti passaggi: {#the-following-steps-take-place-in-your-ms-dynamics-instance}

1. Fare clic su **Impostazioni avanzate**.

1. Fai clic su **Soluzioni**.

1. Seleziona **Marketo Sales Insight** e fai clic sull&#39;icona Elimina.

1. Quando viene visualizzata la finestra modale Disinstalla soluzione, fare clic su **OK**.

   In genere la disinstallazione completa della soluzione MS Dynamics richiede circa 20 minuti. Tuttavia, se disponi di un’istanza MS Dynamics di grandi dimensioni, potrebbe richiedere un po’ più di tempo.

   >[!NOTE]
   >
   >Ricorda di attivare la sincronizzazione globale di MS Dynamics dopo la disinstallazione di MSI.
