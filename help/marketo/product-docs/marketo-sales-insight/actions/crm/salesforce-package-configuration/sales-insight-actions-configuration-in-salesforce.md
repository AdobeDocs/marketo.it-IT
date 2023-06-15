---
description: Configurazione delle azioni Sales Insight in Salesforce - Documenti Marketo - Documentazione del prodotto
title: Configurazione delle azioni di approfondimento sulle vendite in Salesforce
exl-id: 2d842886-3501-4aca-96fb-0d6763ab2b01
source-git-commit: 544dfc0892016223c1e5976bd8c9d108ade7c984
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---

# Configurazione delle azioni di approfondimento sulle vendite in Salesforce {#sales-insight-actions-configuration-in-salesforce}

>[!PREREQUISITES]
>
>* [Installa](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md) o [Aggiorna](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md) Pacchetto Sales Insight nell’istanza Salesforce
>* [Configurare Marketo Sales Insight in Salesforce Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)

## Aggiungi nuovo sito remoto in Salesforce {#add-new-remote-site-in-salesforce}

1. In Salesforce, fai clic su **Configurazione**.

   ![](assets/msi-actions-configuration-in-salesforce-1.png)

1. Cercare &quot;sito remoto&quot; e selezionare **Impostazioni sito remoto**.
   ![](assets/msi-actions-configuration-in-salesforce-2.png)

1. Clic **Nuovo sito remoto**.

   ![](assets/msi-actions-configuration-in-salesforce-3.png)

1. Immettere il nome del sito remoto (ad esempio &quot;MarketoSalesInsight1&quot;). Immetti l&#39;URL del sito remoto `https://ims-na1.adobelogin.com` e fai clic su **Salva**.

   ![](assets/msi-actions-configuration-in-salesforce-4.png)

1. Clic **Nuovo sito remoto** di nuovo.

   ![](assets/msi-actions-configuration-in-salesforce-4a.png)

1. Immettere il nome del sito remoto (ad esempio &quot;MarketoSalesInsight2&quot;). Immetti URL sito remoto `https://mkto-sales-connect.adobe.io` e fai clic su **Salva**.

## Abilitazione delle azioni di approfondimento sulle vendite nel CRM {#enabling-sales-insight-actions-across-the-crm}

1. In Salesforce, fai clic su **Configurazione approfondimento vendite Marketo** scheda.

   ![](assets/msi-actions-configuration-in-salesforce-5.png)

   >[!NOTE]
   >
   >Se nella barra superiore non trovi &quot;Marketo Sales Insight Config&quot;, fai clic sul pulsante **+** firmare e trovarlo in Tutte le schede.

1. Seleziona la **Abilita azioni MSI** casella di controllo.

   ![](assets/msi-actions-configuration-in-salesforce-6.png)

1. Immetti la chiave segreta API.

   ![](assets/msi-actions-configuration-in-salesforce-7.png)

   >[!NOTE]
   >
   >Se la chiave di sicurezza API non è a portata di mano, puoi trovarla seguendo i passaggi descritti in [questo articolo](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md).

1. Clic **Salva** al termine.

Questo attiverà automaticamente tutte le funzioni Azioni MSI descritte nell’articolo Panoramica delle funzioni.

>[!NOTE]
>
>È possibile disattivare tutte le funzioni Azioni MSI semplicemente deselezionando la casella di controllo &quot;Abilita azioni MSI&quot;.

## Governance delle azioni MSI {#msi-actions-governance}

1. Puoi disattivare le campagne di vendita e/o la scheda Attività nella sezione successiva. Questo sarà applicabile ai pannelli lead, contatto, account e opportunità.

   ![](assets/msi-actions-configuration-in-salesforce-8.png)

1. Per disattivare le azioni MSI, deseleziona le funzioni corrispondenti nelle impostazioni delle azioni.

   ![](assets/msi-actions-configuration-in-salesforce-9.png)

>[!NOTE]
>
>Le impostazioni di governance sono applicabili a tutti gli utenti MSI.
