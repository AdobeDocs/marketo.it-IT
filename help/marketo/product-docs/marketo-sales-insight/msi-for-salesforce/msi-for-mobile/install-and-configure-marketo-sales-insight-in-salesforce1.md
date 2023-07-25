---
unique-page-id: 7511512
description: Installare e configurare Marketo Sales Insight in Salesforce1 - Documentazione Marketo - Documentazione del prodotto
title: Installare e configurare Marketo Sales Insight in Salesforce1
exl-id: 9f26e90b-3199-4ef8-92bc-95e8bd81f1c5
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---

# Installare e configurare Marketo Sales Insight in Salesforce1 {#install-and-configure-marketo-sales-insight-in-salesforce}

>[!NOTE]
>
>Clienti esistenti, per favore [Aggiornamento del pacchetto MSI](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/upgrading/upgrading-your-msi-package.md) prima di continuare.

>[!PREREQUISITES]
>
>Se hai Salesforce Enterprise/Unlimited:
>
>* [Passaggio 1 di 3: aggiunta di campi Marketo a Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-1-of-3-add-marketo-fields-to-salesforce-enterprise-unlimited.md)
>* [Passaggio 2 di 3: creare un utente Salesforce per Marketo (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-2-of-3-create-a-salesforce-user-for-marketo-enterprise-unlimited.md)
>* [Passaggio 3 di 3: Connessione di Marketo e Salesforce (Enterprise/Unlimited)](/help/marketo/product-docs/crm-sync/salesforce-sync/setup/enterprise-unlimited-edition/step-3-of-3-connect-marketo-and-salesforce-enterprise-unlimited.md)
>* [Configurare Marketo Sales Insight in Salesforce Enterprise/Unlimited](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-enterprise-unlimited.md)
>
>Se si dispone di Salesforce Professional:
>
>* [Configurare Marketo Sales Insight in Salesforce Professional Edition](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/configuration/configure-marketo-sales-insight-in-salesforce-professional-edition.md)
>

>[!NOTE]
>
>Marketo Sales Insight in Salesforce1 include: elementi di maggiore rilevanza, feed di lead, momenti di interesse e Aggiungi a Marketo Campaign.

## Abilitare l’app mobile Salesforce1 {#enable-the-salesforce1-mobile-app}

1. Clic **Configurazione** e poi **Amministrazione dispositivi mobili**.

   ![](assets/image2015-4-21-15-3a29-3a22.png)

1. Clic **Salesforce1**.

   ![](assets/image2015-4-21-15-3a30-3a51.png)

1. Clic **Impostazioni Salesforce1**.

   ![](assets/image2015-4-21-15-3a32-3a21.png)

1. Clic **Abilita l’app del browser mobile Salesforce1**.

   ![](assets/image2015-4-21-15-3a34-3a27.png)

1. Clic **Salva**.

   ![](assets/image2015-4-21-15-3a42-3a48.png)

1. Seleziona **Amministrazione dispositivi mobili**.

   ![](assets/image2015-4-22-11-3a10-3a14.png)

1. Clic **Gestire il menu di navigazione mobile**.

   ![](assets/image2015-4-22-11-3a13-3a10.png)

1. Seleziona **Marketo** e **Aggiungi** al **Selezionato** voci di menu.

   ![](assets/image2015-4-22-14-3a55-3a37.png)

1. Seleziona **Marketo**, spostalo **Su** nell&#39;area desiderata, quindi fare clic su **Salva**.

   ![](assets/image2015-4-22-17-3a20-3a56.png)

## Nascondi oggetto personalizzato Marketo obsoleto {#hide-outdated-marketo-custom-object}

1. Clic **Configurazione**.

   ![](assets/image2015-4-22-15-3a13-3a48.png)

1. Seleziona **Gestisci utenti**.

   ![](assets/image2015-5-5-11-3a13-3a45.png)

1. Seleziona **Profili**.

   ![](assets/image2015-5-5-11-3a15-3a21.png)

1. Fai clic per **modifica** eventuali profili desiderati.

   ![](assets/image2015-5-5-13-3a51-3a36.png)

1. Sotto **Impostazioni scheda**, seleziona la _primo_ **Marketo**.

   ![](assets/image2015-5-5-13-3a55-3a36.png)

1. Seleziona **Scheda nascosta**.

   ![](assets/image2015-5-5-14-3a2-3a29.png)

   >[!NOTE]
   >
   >Assicurati di nascondere la scheda Marketo per tutti i profili desiderati.

## Personalizza schede {#customize-tabs}

1. Clic **+**.

   ![](assets/image2015-4-22-17-3a14-3a49.png)

1. Clic **Personalizza schede personali**.

   ![](assets/image2015-4-22-17-3a16-3a22.png)

1. Seleziona **Marketo** e **Aggiungi** alle schede selezionate.

   ![](assets/image2015-4-22-17-3a17-3a15.png)

1. Seleziona **Marketo**, spostalo **Su** nell&#39;area desiderata, quindi fare clic su **Salva**.

   ![](assets/image2015-4-22-18-3a29-3a47.png)

## Personalizza layout di pagina {#customize-page-layouts}

1. Clic **Configurazione**.

   ![](assets/image2015-4-22-17-3a26-3a56.png)

1. Clic **Configurazione**, tipo **Layout di pagina** e fai clic su **Layout di pagina** in Lead.

   >[!NOTE]
   >
   >Ripeti i passaggi per ogni layout di pagina utilizzato dalla tua organizzazione (marketing, vendite, ecc.) per gli oggetti Contact, Account e Opportunity.

   ![](assets/image2015-4-22-17-3a34-3a33.png)

1. Clic **Modifica** per apportare modifiche al layout del lead.

   ![](assets/image2015-4-22-17-3a44-3a0.png)

1. Clic **Visualforce Pages** e quindi trascina **Cellulare lead** nella sezione Schede mobili.

   ![](assets/image2015-4-22-17-3a49-3a37.png)

1. Impostate Altezza (Height) a 66 e fate clic su **OK**.

   ![](assets/image2015-4-22-17-3a52-3a15.png)

1. Clic **Campi** e trascina **Aggiungi a Marketo Campaign** al **Insight sulla vendita di Marketo** sezione.

   ![](assets/configure-step-6.png)

   >[!TIP]
   >
   >Digita &quot;Aggiungi a&quot; nella Ricerca rapida per facilitare la ricerca di Aggiungi a Marketo Campaign.

1. Clic **Salva**.

   ![](assets/image2015-4-22-18-3a1-3a56.png)

Meno male! Installazione di Marketo Sales Insight per Salesforce1 completata. Vada avanti e si dia una pacca sulla schiena.

>[!MORELIKETHIS]
>
>* [Elementi di maggiore rilevanza in Salesforce1](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/best-bets-in-salesforce1.md)
>* [Momenti interessanti in Salesforce1](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/interesting-moments-in-salesforce1.md)
>* [Inviare azioni e-mail e campagne Marketo e watchlist in Salesforce1](/help/marketo/product-docs/marketo-sales-insight/msi-for-salesforce/msi-for-mobile/send-marketo-email-and-campaign-and-watchlist-actions-in-salesforce1.md)
