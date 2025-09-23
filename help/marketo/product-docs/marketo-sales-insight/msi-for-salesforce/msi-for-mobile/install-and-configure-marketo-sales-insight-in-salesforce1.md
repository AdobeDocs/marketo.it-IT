---
unique-page-id: 7511512
description: Installare e configurare Marketo Sales Insight in Salesforce1 - Documentazione Marketo - Documentazione del prodotto
title: Installare e configurare Marketo Sales Insight in Salesforce1
exl-id: 9f26e90b-3199-4ef8-92bc-95e8bd81f1c5
feature: Marketo Sales Insights
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 7%

---

# Installa e configura [!DNL Marketo Sales Insight] in [!DNL Salesforce1] {#install-and-configure-marketo-sales-insight-in-salesforce}

>[!NOTE]
>
>Clienti esistenti, [Aggiorna il pacchetto MSI](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md) prima di continuare.

>[!PREREQUISITES]
>
>Se si dispone di Salesforce Enterprise/Unlimited:
>
>* [Passaggio 1 di 3: aggiunta di campi Marketo a [!DNL Salesforce] (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [Passaggio 2 di 3: creazione di un  [!DNL Salesforce] utente per Marketo (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
>* [Passaggio 3 di 3: connettere Marketo e [!DNL Salesforce] (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md)
>* [Configura [!DNL Marketo Sales Insight] in [!DNL Salesforce] Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)
>
>Se si dispone di Salesforce Professional:
>
>* [Configurare Marketo Sales Insight in Salesforce Professional Edition](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md)
>

>[!NOTE]
>
>[!DNL Marketo Sales Insight] in [!DNL Salesforce1] include: [!DNL Belementi di maggiore rilevanza], feed lead, momenti di interesse e Aggiungi a Marketo Campaign.

## Abilita l&#39;app mobile [!DNL Salesforce1] {#enable-the-salesforce1-mobile-app}

1. Fare clic su **[!DNL Setup]** e quindi su **[!DNL Mobile Administration]**.

   ![](assets/image2015-4-21-15-3a29-3a22.png)

1. Fai clic su **[!UICONTROL Salesforce1]**.

   ![](assets/image2015-4-21-15-3a30-3a51.png)

1. Fai clic su **[!UICONTROL Salesforce1 Settings]**.

   ![](assets/image2015-4-21-15-3a32-3a21.png)

1. Fai clic su **[!UICONTROL Enable the Salesforce1 mobile browser app]**.

   ![](assets/image2015-4-21-15-3a34-3a27.png)

1. Fai clic su **[!UICONTROL Save]**.

   ![](assets/image2015-4-21-15-3a42-3a48.png)

1. Seleziona **[!UICONTROL Mobile Administration]**.

   ![](assets/image2015-4-22-11-3a10-3a14.png)

1. Fai clic su **[!UICONTROL Manage the mobile navigation menu]**.

   ![](assets/image2015-4-22-11-3a13-3a10.png)

1. Selezionare **[!UICONTROL Marketo]** e **[!UICONTROL Add]** per le voci di menu **[!UICONTROL Selected]**.

   ![](assets/image2015-4-22-14-3a55-3a37.png)

1. Selezionare **[!UICONTROL Marketo]**, spostarlo **[!UICONTROL Up]** nell&#39;area desiderata e fare clic su **[!UICONTROL Save]**.

   ![](assets/image2015-4-22-17-3a20-3a56.png)

## Nascondi oggetto personalizzato Marketo obsoleto {#hide-outdated-marketo-custom-object}

1. Fai clic su **[!UICONTROL Setup]**.

   ![](assets/image2015-4-22-15-3a13-3a48.png)

1. Seleziona **[!UICONTROL Manage Users]**.

   ![](assets/image2015-5-5-11-3a13-3a45.png)

1. Seleziona **[!UICONTROL Profiles]**.

   ![](assets/image2015-5-5-11-3a15-3a21.png)

1. Fare clic per **[!UICONTROL Edit]** i profili desiderati.

   ![](assets/image2015-5-5-13-3a51-3a36.png)

1. In **[!UICONTROL Tab Settings]**, selezionare _first_ **[!UICONTROL Marketo]**.

   ![](assets/image2015-5-5-13-3a55-3a36.png)

1. Seleziona **[!UICONTROL Tab Hidden]**.

   ![](assets/image2015-5-5-14-3a2-3a29.png)

   >[!NOTE]
   >
   >Assicurati di nascondere la scheda Marketo per tutti i profili desiderati.

## Personalizza schede {#customize-tabs}

1. Fare clic su **+**.

   ![](assets/image2015-4-22-17-3a14-3a49.png)

1. Fai clic su **[!UICONTROL Customize My Tabs]**.

   ![](assets/image2015-4-22-17-3a16-3a22.png)

1. Selezionare **[!UICONTROL Marketo]** e **[!UICONTROL Add]** nelle schede selezionate.

   ![](assets/image2015-4-22-17-3a17-3a15.png)

1. Selezionare **[!UICONTROL Marketo]**, spostarlo **[!UICONTROL Up]** nell&#39;area desiderata e fare clic su **[!UICONTROL Save]**.

   ![](assets/image2015-4-22-18-3a29-3a47.png)

## Personalizza layout di pagina {#customize-page-layouts}

1. Fai clic su **[!UICONTROL Setup]**.

   ![](assets/image2015-4-22-17-3a26-3a56.png)

1. Fare clic su **[!UICONTROL Setup]**, digitare **[!UICONTROL Page Layouts]**, quindi fare clic su **[!UICONTROL Page Layouts]** in Lead.

   >[!NOTE]
   >
   >Ripeti i passaggi per ogni layout di pagina utilizzato dalla tua organizzazione (marketing, vendite, ecc.) per gli oggetti Contatto, Account e Opportunità.

   ![](assets/image2015-4-22-17-3a34-3a33.png)

1. Fare clic su **[!UICONTROL Edit]** per apportare modifiche al layout del lead.

   ![](assets/image2015-4-22-17-3a44-3a0.png)

1. Fare clic su **[!UICONTROL Visualforce Pages]** e quindi trascinare **[!UICONTROL Lead Mobile]** nella sezione Schede mobili.

   ![](assets/image2015-4-22-17-3a49-3a37.png)

1. Impostare Altezza su 66 e fare clic su **[!UICONTROL OK]**.

   ![](assets/image2015-4-22-17-3a52-3a15.png)

1. Fare clic su **[!UICONTROL Fields]** e trascinare **[!UICONTROL Add to Marketo Campaign]** nella sezione **[!UICONTROL Marketo Sales Insight]**.

   ![](assets/configure-step-6.png)

   >[!TIP]
   >
   >Digita &quot;Aggiungi a&quot; nella Ricerca rapida per facilitare la ricerca di Aggiungi a Marketo Campaign.

1. Fai clic su **[!UICONTROL Save]**.

   ![](assets/image2015-4-22-18-3a1-3a56.png)

Meno male! Installazione di [!DNL Marketo Sales Insight] per [!DNL Salesforce1] completata. Vada avanti e si dia una pacca sulla schiena.

>[!MORELIKETHIS]
>
>* [[!DNL Best Bets] in [!DNL Salesforce1]](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/best-bets-in-salesforce1.md)
>* [Momenti di interesse in [!DNL Salesforce1]](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/interesting-moments-in-salesforce1.md)
>* [Invia azioni e-mail e campagne Marketo e watchlist in [!DNL Salesforce1]](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/send-marketo-email-and-campaign-and-watchlist-actions-in-salesforce1.md)
