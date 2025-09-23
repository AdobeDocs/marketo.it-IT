---
unique-page-id: 7504923
description: Imposta [!DNL Google AdWords] conversioni nel modello dei ricavi con un account Manager - Documenti Marketo - Documentazione del prodotto
title: Imposta [!DNL Google AdWords] conversioni nel modello dei ricavi con un account Manager
exl-id: 8c9f50cf-0a8b-4f9a-a0bd-bb57eeac24cf
feature: Reporting, Revenue Cycle Analytics
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 1%

---

# Imposta [!DNL Google AdWords] conversioni nel modello dei ricavi con un account Manager {#set-google-adwords-conversions-in-the-revenue-model-with-a-manager-account}

Collega l&#39;account [!DNL Google AdWords] a Marketo per caricare automaticamente i dati di conversione offline da Marketo a [!DNL Google AdWords]. Quindi, dall&#39;interfaccia utente di [!DNL AdWords], potrai vedere facilmente quali clic hanno generato lead qualificati, opportunità e nuovi clienti (o qualsiasi fase dei ricavi desideri monitorare) dopo [aver aggiunto colonne personalizzate](https://support.google.com/adwords/answer/3073556) in [!DNL AdWords].

Se si dispone di più account [!DNL Google Adwords], è possibile utilizzare un account [[!DNL Google AdWords] Manager](https://www.google.com/adwords/manager-accounts/) (precedentemente noto come My Client Center) per integrarli con Marketo.

È possibile mappare [!DNL AdWords] conversioni offline in uno o più stadi in un modello dei ricavi. Esistono due modi:

* Azione fase
* Mappatura di [!DNL AdWords]

>[!PREREQUISITES]
>
>[Aggiungi [!DNL Google AdWords] come servizio Launchpoint con un account Manager](/help/marketo/product-docs/administration/additional-integrations/add-google-adwords-as-a-launchpoint-service-with-a-manager-account.md)

## Usa azione fase {#use-stage-action}

Mappa una conversione [!DNL AdWords] nelle azioni di staging.

1. Selezionare il passaggio da mappare a una conversione [!DNL AdWords].

   ![](assets/image2015-2-26-16-3a40-3a2.png)

1. Nel menu a discesa **[!UICONTROL Stage Actions]**, seleziona **[!UICONTROL Set AdWords Conversion]**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Imposta una conversione **[!DNL AdWords]**.

   >[!NOTE]
   >
   >È possibile selezionare una conversione [!DNL AdWords] diversa per ogni account figlio.

   ![](assets/image2015-3-27-17-3a16-3a37.png)

   Suggerimento: se non si dispone di [!DNL AdWords] conversioni, crearne una facendo clic su **[!UICONTROL +New Conversion]**.

   ![](assets/image2015-3-27-17-3a18-3a58.png)

1. Fai clic su **[!UICONTROL Save]**.

   ![](assets/image2015-3-27-17-3a21-3a15.png)

1. Dopo aver completato la mappatura di tutte le conversioni di [!DNL AdWords] in fasi di ricavi, torna alla pagina di riepilogo. Selezionare **[!UICONTROL Model Actions]** e scegliere **[!UICONTROL Approve Stages]**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

## Suggerimento pro: aggiungi una nuova conversione {#pro-tip-add-a-new-conversion}

Suggerimento pro! È possibile creare una nuova conversione offline di [!DNL AdWords] da Marketo.

>[!CAUTION]
>
>Per le nuove conversioni create da Marketo, l’impostazione &quot;ottimizzazione&quot; è abilitata. Ciò significa che le strategie di offerta di [!DNL AdWords] possono ottimizzare le offerte per tali conversioni. È possibile modificare questa impostazione dall&#39;account [!DNL AdWords].

1. Nel menu a discesa **[!UICONTROL Stage Actions]**, seleziona **[!UICONTROL Set AdWords Conversion]**.

   ![](assets/image2015-2-26-16-3a52-3a24.png)

1. Seleziona **[!UICONTROL New Conversion]**.

   ![](assets/image2015-3-27-17-3a23-3a13.png)

1. Immetti un **Nome conversione**. Fai clic su **[!UICONTROL Save]**.

   ![](assets/image2015-3-27-17-3a24-3a49.png)

   Eccellente! Questa nuova conversione verrà visualizzata nel tuo account [!DNL AdWords].

## Usa mappatura [!DNL AdWords] {#use-adwords-mapping}

È possibile associare tutte le fasi del modello alla conversione [!DNL AdWords] in un&#39;unica posizione utilizzando [!DNL AdWords] Mapping.

1. Seleziona **[!UICONTROL Edit AdWords Mappings]**.

   ![](assets/image2015-2-26-17-3a3-3a29.png)

1. Selezionare l&#39;account **[!DNL AdWords]desiderato** e la conversione **[!DNL AdWords]desiderata** per ogni fase che si desidera monitorare.

   ![](assets/image2015-3-27-17-3a30-3a15.png)

1. Dopo aver mappato le fasi, fare clic su **[!UICONTROL Save]**.

   ![](assets/image2015-3-27-17-3a30-3a48.png)

1. Dopo aver completato la mappatura di tutte le conversioni di [!DNL AdWords] in fasi di ricavi, torna alla pagina di riepilogo. Selezionare **[!UICONTROL Model Actions]** e scegliere **[!UICONTROL Approve Stages]**.

   ![](assets/image2015-2-27-12-3a20-3a20.png)

Per visualizzare i dati di conversione offline, dovrai accedere al tuo account [!DNL AdWords]. È consigliabile utilizzare la funzionalità [Colonne personalizzate](https://support.google.com/adwords/answer/3073556) per creare colonne di conteggio delle conversioni per ogni conversione offline importata da Marketo.
