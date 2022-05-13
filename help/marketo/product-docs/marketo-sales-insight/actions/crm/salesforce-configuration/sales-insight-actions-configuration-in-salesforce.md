---
description: Configurazione delle azioni di Insight sulle vendite in Salesforce - Documenti Marketo - Documentazione del prodotto
title: Configurazione delle azioni di Insight sulle vendite in Salesforce
exl-id: 2d842886-3501-4aca-96fb-0d6763ab2b01
source-git-commit: 222b0692998be1fd15dc6465af1da627e1c32683
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 0%

---

# Configurazione delle azioni di Insight sulle vendite in Salesforce {#sales-insight-actions-configuration-in-salesforce}

>[!PREREQUISITES]
>
>* [Installa](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md) o [Aggiornamento](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md) Pacchetto di informazioni sulle vendite nella tua istanza Salesforce
>* [Configurare Marketo Sales Insight in Salesforce Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)


## Aggiungi nuovo sito remoto in Salesforce {#add-new-remote-site-in-salesforce}

1. In Salesforce, fai clic su **Configurazione**.

   ![](assets/msi-actions-configuration-in-salesforce-1.png)

1. Cerca &quot;sito remoto&quot; e seleziona **Impostazioni del sito remoto**.
   ![](assets/msi-actions-configuration-in-salesforce-2.png)

1. Fai clic su **Nuovo sito remoto**.

   ![](assets/msi-actions-configuration-in-salesforce-3.png)

1. Immettere il nome del sito remoto (può essere simile a &quot;MarketoSalesInsight&quot;). Inserisci l’URL del sito remoto (https://ims-na1-stg1.adobelogin.com) e fai clic su **Salva**.

   ![](assets/msi-actions-configuration-in-salesforce-4.png)

## Abilitazione delle azioni Approfondimenti vendite nel CRM {#enabling-sales-insight-actions-across-the-crm}

1. In Salesforce, fai clic sul pulsante **Configurazione di Marketo Sales Insight** scheda .

   ![](assets/msi-actions-configuration-in-salesforce-5.png)

   >[!NOTE]
   >
   >Se non trovi &quot;Marketo Sales Insight Config&quot; nella barra superiore, fai clic sul pulsante **+** firmare e trovarla sotto Tutte le schede.

1. Seleziona la **Abilita azioni MSI** casella di controllo.

   ![](assets/msi-actions-configuration-in-salesforce-6.png)

1. Immetti la chiave segreto API.

   ![](assets/msi-actions-configuration-in-salesforce-7.png)

   >[!NOTE]
   >
   >Se la chiave di sicurezza API non è utile, puoi trovarlo seguendo i passaggi descritti in [articolo](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md).

1. Fai clic su **Salva** al termine.

In questo modo verranno abilitate automaticamente tutte le funzionalità delle azioni MSI descritte nell&#39;articolo sulla panoramica delle funzioni.

>[!NOTE]
>
>È possibile disabilitare tutte le funzionalità delle azioni MSI semplicemente deselezionando la casella di controllo &quot;Abilita azioni MSI&quot;.

## Governance delle azioni MSI {#msi-actions-governance}

1. È possibile disabilitare le campagne di vendita e/o la scheda Attività nella sezione successiva. Questo sarà applicabile ai pannelli lead, contatti, account e opportunità.

   ![](assets/msi-actions-configuration-in-salesforce-8.png)

1. È possibile disabilitare le azioni MSI deselezionando le funzioni corrispondenti nelle impostazioni Azioni.

   ![](assets/msi-actions-configuration-in-salesforce-9.png)

>[!NOTE]
>
>Le impostazioni di governance sono applicabili a tutti gli utenti MSI.
