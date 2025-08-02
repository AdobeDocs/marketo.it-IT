---
unique-page-id: 4720810
description: Remarketing personalizzato in Google - Documentazione Marketo - Documentazione del prodotto
title: Remarketing personalizzato in Google
exl-id: cc733f43-161d-41e4-afdf-8b5217700810
feature: Web Personalization
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '225'
ht-degree: 2%

---

# Remarketing personalizzato in Google {#personalized-remarketing-in-google}

Il remarketing personalizzato consente di coinvolgere nuovamente gli utenti utilizzando i dati RTP e la potenza di Google Analytics grazie alla rete di visualizzazione Google.

>[!PREREQUISITES]
>
>* Completa la configurazione di [Retargeting con [!DNL Web Personalization] Dati](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* Consulta la documentazione di [Remarketing con Guida di Google Analytics](https://support.google.com/analytics/topic/2611283?hl=en&ref_topic=3413645).

## Creazione di un pubblico per il remarketing in Google {#creating-a-remarketing-audience-in-google}

1. Accedi al tuo Google Analytics. Fare clic su **[!UICONTROL Admin]**, **[!UICONTROL Account]**, **[!UICONTROL Property]**. Fare clic su **[!UICONTROL Audience Definitions]** e **[!UICONTROL Audiences]**.

   ![](assets/remarketing-ga-screenshots.jpg)

1. Fai clic su **[!UICONTROL +New Audience]**.

   ![](assets/image2015-1-15-17-3a26-3a40.png)

1. **[!UICONTROL Link Configuration]**: collega al tuo account [!DNL Google Adwords]. **[!UICONTROL Define Audience]**: fare clic su **[!UICONTROL Create New]**.

   ![](assets/image2015-1-15-17-3a32-3a4.png)

1. In Audience Builder, fai clic su **[!UICONTROL Sequences]** e **[!UICONTROL Find the RTP Data]** in [!UICONTROL Custom Dimensions], [!UICONTROL [!]UICONTROL Custom Variables], [!UICONTROL Events].

>[!TIP]
>
>Come trovare i dati RTP in Analytics per creare il tuo pubblico?
>
>In Google Analytics:
>
>* Variabili personalizzate: Organizzazione, Settore
>* Categoria evento: Segmento, Insightera-CTA, RTP-Remarketing
>* Etichetta evento: Nome segmento, Nome campagna, Nome pubblico segmentato
>
>In Google Universal Analytics:
>
>* Dimensioni personalizzate: organizzazione, settore, categoria (Fortune 500,1000, Global 2000), gruppo (Enterprise, SMB), elenco ABM (Named Account List)
>* Categoria evento: RTP-Segment, RTP-Campaign RTP-Remarketing
>* Etichetta evento: Nome segmento, Nome campagna, Nome pubblico segmentato

**Esempio di pubblico di remarketing dai dati del pubblico segmentato RTP**

1. Fare clic su **[!UICONTROL Sequences].**
1. Seleziona **[!UICONTROL Event Label].**
1. Immettere **[!UICONTROL Name of Segmented Audience]** (come appare nel protocollo RTP).
1. Fai clic su **[!UICONTROL Apply]**.

![](assets/image2015-2-10-14-3a51-3a43.png)

**Esempio di pubblico dai dati del settore RTP**

![](assets/image2015-1-15-17-3a36-3a5.png)

1. Fai clic su **[!UICONTROL Sequences]**.
1. Seleziona **[!UICONTROL RTP-Industry]**.
1. Immettere **Nome settore** (esempio: [!UICONTROL Financial Services], [!UICONTROL Education]...).
1. Fai clic su **[!UICONTROL Apply]**.
1. Immetti un **[!UICONTROL Audience Name]**. Fai clic su **[!UICONTROL Save]**.

![](assets/image2015-1-15-18-3a29-3a16.png)

## Crea una campagna pubblicitaria per il remarketing in [!DNL Google Adwords] {#create-a-remarketing-ad-campaign-in-google-adwords}

1. Accedi a **[!DNL Google Adwords]**. Fai clic su **[!UICONTROL Campaigns]**, seleziona **[!UICONTROL Display Network only]**.

   ![](assets/image2015-1-15-18-3a31-3a58.png)

1. Immetti **[!UICONTROL Campaign Name]**, Seleziona **[!UICONTROL Type Remarketing].**

   ![](assets/image2015-1-15-18-3a35-3a7.png)

1. Immettere **[!UICONTROL Ad Group Name],** immettere **[!UICONTROL Enhanced CPC]**, Selezionare **[!UICONTROL Remarketing List]**.

   ![](assets/image2015-1-15-18-3a51-3a57.png)

1. Fare clic su **[!UICONTROL Save]** e continuare.
1. Aggiungi un annuncio di testo o immagine e avvia la campagna di remarketing.

   ![](assets/image2015-1-15-18-3a47-3a21.png)

>[!MORELIKETHIS]
>
>* [Retargeting con [!DNL Web Personalization] Dati](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* [Remarketing personalizzato in [!DNL Facebook]](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md)
