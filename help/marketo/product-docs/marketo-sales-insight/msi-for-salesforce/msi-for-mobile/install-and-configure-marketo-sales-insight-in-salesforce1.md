---
unique-page-id: 7511512
description: Installazione e configurazione di Marketing Sales Insight in Salesforce1 - Marketo Docs - Documentazione prodotto
title: Installazione e configurazione di Marketing Sales Insight in Salesforce1
translation-type: tm+mt
source-git-commit: 972cf9769ac751d9abfd5665975703dcd07930f0
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---


# Installazione e configurazione di Marketing Sales Insight in Salesforce1 {#install-and-configure-marketo-sales-insight-in-salesforce}

>[!NOTE]
>
>I clienti esistenti devono [aggiornare il pacchetto MSI](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md) prima di continuare.

>[!PREREQUISITES]
>
>Se disponi di Salesforce Enterprise/Unlimited:
>
>* [Passaggio 1 di 3: Aggiungi campi Marketo a Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [Passaggio 2 di 3: Crea un utente Salesforce per Marketo (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
>* [Passaggio 3 di 3: Connect Marketo e Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md)
>* [Configurare Marketing Sales Insight in Salesforce Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)

>
>
Se disponete di Salesforce Professional:
>
>* [Configurare Marketing Sales Insight in Salesforce Professional Edition](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md)

>



>[!NOTE]
>
>Marketing Sales Insight in Salesforce1 include: Migliori Scommesse, Feed lead, Momenti interessanti e Aggiungi alla campagna Marketo.

## Abilita l&#39;app mobile Salesforce1 {#enable-the-salesforce1-mobile-app}

1. Fare clic su **Setup**, quindi su **Mobile Administration**.

   ![](assets/image2015-4-21-15-3a29-3a22.png)

1. Fare clic su **Salesforce1**.

   ![](assets/image2015-4-21-15-3a30-3a51.png)

1. Fare clic su **Impostazioni Salesforce1**.

   ![](assets/image2015-4-21-15-3a32-3a21.png)

1. Fai clic su **Abilita l&#39;app browser mobile Salesforce1**.

   ![](assets/image2015-4-21-15-3a34-3a27.png)

1. Fare clic su **Salva**.

   ![](assets/image2015-4-21-15-3a42-3a48.png)

1. Selezionare **Mobile Administration**.

   ![](assets/image2015-4-22-11-3a10-3a14.png)

1. Fare clic su **Gestisci il menu di navigazione mobile**.

   ![](assets/image2015-4-22-11-3a13-3a10.png)

1. Selezionare **Marketo** e **Aggiungi** alle voci di menu **Selezionato**.

   ![](assets/image2015-4-22-14-3a55-3a37.png)

1. Selezionare **Marketo**, spostarlo **Su** nell&#39;area desiderata e fare clic su **Salva**.

   ![](assets/image2015-4-22-17-3a20-3a56.png)

## Nascondi oggetto personalizzato Marketo obsoleto {#hide-outdated-marketo-custom-object}

1. Fare clic su **Setup**.

   ![](assets/image2015-4-22-15-3a13-3a48.png)

1. Selezionare **Gestisci utenti**.

   ![](assets/image2015-5-5-11-3a13-3a45.png)

1. Selezionare **Profili**.

   ![](assets/image2015-5-5-11-3a15-3a21.png)

1. Fare clic per **modificare** i profili desiderati.

   ![](assets/image2015-5-5-13-3a51-3a36.png)

1. In **Impostazioni scheda**, selezionare il _primo_ **Marketo**.

   ![](assets/image2015-5-5-13-3a55-3a36.png)

1. Selezionare **Tab Hidden**.

   ![](assets/image2015-5-5-14-3a2-3a29.png)

   >[!NOTE]
   >
   >Assicuratevi di nascondere la scheda Marketo per tutti i profili desiderati!

## Personalizza schede {#customize-tabs}

1. Fare clic su **+**.

   ![](assets/image2015-4-22-17-3a14-3a49.png)

1. Fare clic su **Personalizza schede**.

   ![](assets/image2015-4-22-17-3a16-3a22.png)

1. Selezionare **Marketo** e **Aggiungi** alle schede selezionate.

   ![](assets/image2015-4-22-17-3a17-3a15.png)

1. Selezionare **Marketo**, spostarlo **Su** nell&#39;area desiderata e fare clic su **Salva**.

   ![](assets/image2015-4-22-18-3a29-3a47.png)

## Personalizzare i layout di pagina {#customize-page-layouts}

1. Fare clic su **Setup**.

   ![](assets/image2015-4-22-17-3a26-3a56.png)

1. Fare clic su **Setup**, digitare **Layout di pagina**, quindi fare clic su **Layout di pagina** in Lead.

   >[!NOTE]
   >
   >Ripetete i passaggi per ogni layout di pagina utilizzato dalla vostra azienda (marketing, vendite, ecc.) per gli oggetti Contatto, Account e Opportunità.

   ![](assets/image2015-4-22-17-3a34-3a33.png)

1. Fate clic su **Modifica** per apportare modifiche al layout lead.

   ![](assets/image2015-4-22-17-3a44-3a0.png)

1. Fare clic su **Visualforce Pages**, quindi trascinare **Lead Mobile** nella sezione Mobile Card.

   ![](assets/image2015-4-22-17-3a49-3a37.png)

1. Cambia l&#39;altezza in 66 e fai clic su **OK**.

   ![](assets/image2015-4-22-17-3a52-3a15.png)

1. Fare clic su **Campi** e trascinare **Aggiungi a campagna marketing** nella sezione **Visione vendite marketing**.

   ![](assets/configure-step-6.png)

   >[!TIP]
   >
   >Digita &quot;Aggiungi a&quot; nella ricerca rapida per facilitare la ricerca di Aggiungi a campagna marketing.

1. Fare clic su **Salva**.

   ![](assets/image2015-4-22-18-3a1-3a56.png)

Fooh! Hai finalmente finito di installare Marketing Marketing Insight for Salesforce1! Andate avanti e datevi una pacca sulla schiena.

>[!MORELIKETHIS]
>
>* [Best Bets in Salesforce1](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/best-bets-in-salesforce1.md)
>* [Momenti interessanti in Salesforce1](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/interesting-moments-in-salesforce1.md)
>* [Invia e-mail di Marketo e campagne e liste di controllo in Salesforce1](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/send-marketo-email-and-campaign-and-watchlist-actions-in-salesforce1.md)

