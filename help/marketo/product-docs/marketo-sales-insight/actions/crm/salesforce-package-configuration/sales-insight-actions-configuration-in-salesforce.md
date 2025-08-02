---
description: Configurazione delle azioni di Insight per le vendite in Salesforce - Documenti Marketo - Documentazione del prodotto
title: Configurazione delle azioni di Sales Insight in Salesforce
exl-id: 2d842886-3501-4aca-96fb-0d6763ab2b01
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '207'
ht-degree: 0%

---

# Configurazione di [!DNL Sales Insight Actions] in [!DNL Salesforce] {#sales-insight-actions-configuration-in-salesforce}

>[!PREREQUISITES]
>
>* [Installa](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/installation/install-marketo-sales-insight-package-in-salesforce-appexchange.md) o [Aggiorna](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md) il pacchetto Sales Insight nell&#39;istanza [!DNL Salesforce]
>* [Configura Marketo Sales Insight in [!DNL Salesforce] Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)

## Aggiungi nuovo sito remoto in [!DNL Salesforce] {#add-new-remote-site-in-salesforce}

1. In [!DNL Salesforce], fare clic su **[!UICONTROL Setup]**.

   ![](assets/msi-actions-configuration-in-salesforce-1.png)

1. Cercare &quot;[!UICONTROL remote site]&quot; e selezionare **[!UICONTROL Remote Site Settings]**.
   ![](assets/msi-actions-configuration-in-salesforce-2.png)

1. Fai clic su **[!UICONTROL New Remote Site]**.

   ![](assets/msi-actions-configuration-in-salesforce-3.png)

1. Immettere il nome del sito remoto (ad esempio &quot;MarketoSalesInsight1&quot;). Immettere l&#39;URL del sito remoto `https://ims-na1.adobelogin.com` e fare clic su **[!UICONTROL Save]**.

   ![](assets/msi-actions-configuration-in-salesforce-4.png)

1. Fare di nuovo clic su **[!UICONTROL New Remote Site]**.

   ![](assets/msi-actions-configuration-in-salesforce-4a.png)

1. Immettere il nome del sito remoto (ad esempio &quot;MarketoSalesInsight2&quot;). Immettere l&#39;URL del sito remoto `https://mkto-sales-connect.adobe.io` e fare clic su **[!UICONTROL Save]**.

## Abilitazione di [!DNL Sales Insight Actions] in CRM {#enabling-sales-insight-actions-across-the-crm}

1. In [!DNL Salesforce], fare clic sulla scheda **[!UICONTROL Marketo Sales Insight Config]**.

   ![](assets/msi-actions-configuration-in-salesforce-5.png)

   >[!NOTE]
   >
   >Se &quot;[!UICONTROL Marketo Sales Insight Config]&quot; non è visualizzato nella barra superiore, fare clic sul segno **+** e trovarlo in Tutte le schede.

1. Selezionare la casella di controllo **[!UICONTROL Enable MSI Actions]**.

   ![](assets/msi-actions-configuration-in-salesforce-6.png)

1. Immettere [!UICONTROL API Secret Key].

   ![](assets/msi-actions-configuration-in-salesforce-7.png)

   >[!NOTE]
   >
   >Se il tuo [!UICONTROL API Secrey Key] non è a portata di mano, puoi trovarlo seguendo i passaggi descritti in [questo articolo](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md).

1. Al termine, fai clic su **[!UICONTROL Save]**.

Questo attiverà automaticamente tutte le funzioni Azioni MSI descritte nell’articolo Panoramica delle funzioni.

>[!NOTE]
>
>È possibile disattivare tutte le funzioni Azioni MSI semplicemente deselezionando la casella di controllo &quot;Abilita azioni MSI&quot;.

## Governance delle azioni MSI {#msi-actions-governance}

1. Puoi disattivare le campagne di vendita e/o la scheda Attività nella sezione successiva. Questo sarà applicabile ai pannelli lead, contatto, account e opportunità.

   ![](assets/msi-actions-configuration-in-salesforce-8.png)

1. È possibile disattivare le azioni MSI deselezionando le funzionalità corrispondenti in [!UICONTROL Actions settings].

   ![](assets/msi-actions-configuration-in-salesforce-9.png)

>[!NOTE]
>
>Le impostazioni di governance sono applicabili a tutti gli utenti MSI.
