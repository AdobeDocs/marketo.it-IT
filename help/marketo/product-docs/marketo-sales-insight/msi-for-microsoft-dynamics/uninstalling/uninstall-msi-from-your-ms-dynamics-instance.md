---
unique-page-id: 37355600
description: Disinstallare MSI dall’istanza di MS Dynamics - Documentazione di Marketo - Documentazione del prodotto
title: Disinstallare MSI dall’istanza di MS Dynamics
exl-id: 86e8dbc9-236f-42ad-96e8-cdb1b4c3bed2
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '156'
ht-degree: 0%

---

# Disinstallare MSI dall’istanza di MS Dynamics {#uninstall-msi-from-your-ms-dynamics-instance}

Per disinstallare MSI dall’istanza di MS Dynamics, è necessario eseguire i passaggi sia in Marketo che in MS Dynamics.

>[!PREREQUISITES]
>
>[Disabilita sincronizzazione MS Dynamics globale](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/uninstalling/disable-global-ms-dynamics-sync.md)

1. In Marketo, fai clic su **Amministratore**.

   ![](assets/one-1.png)

1. Clic **Insight sulle vendite**.

   ![](assets/six.png)

1. Clic **Modifica sincronizzazione campi**.

   ![](assets/seven.png)

1. Seleziona la **Disattiva sincronizzazione** e fai clic su **Salva**.

   >[!NOTE]
   >
   >Assicurati di [disattivare la sincronizzazione globale di MS Dynamics](/help/marketo/product-docs/marketo-sales-insight/msi-for-microsoft-dynamics/uninstalling/disable-global-ms-dynamics-sync.md) prima di disabilitare la sincronizzazione dei campi.

   ![](assets/eight.png)

## Nell’istanza di MS Dynamics vengono eseguiti i seguenti passaggi: {#the-following-steps-take-place-in-your-ms-dynamics-instance}

1. Clic **Impostazioni avanzate**.

1. Clic **Soluzioni**.

1. Seleziona **Insight sulla vendita di Marketo** e fai clic sull’icona elimina.

1. Quando viene visualizzata la finestra modale Disinstalla soluzione, fai clic su **OK**.

   In genere la disinstallazione completa della soluzione MS Dynamics richiede circa 20 minuti. Tuttavia, se disponi di un’istanza MS Dynamics di grandi dimensioni, potrebbe richiedere un po’ più di tempo.

   >[!NOTE]
   >
   >Ricorda di attivare la sincronizzazione globale di MS Dynamics dopo la disinstallazione di MSI.
