---
unique-page-id: 10098759
description: Scopri come testare l’integrazione di Facebook Lead Ads per dispositivi mobili con Marketo. Verifica correttamente gli invii di annunci lead dalla sincronizzazione mobile.
title: Testare gli annunci sponsorizzati di Facebook per l’integrazione per dispositivi mobili con Marketo
exl-id: 0c381c53-f97a-4e1d-b44d-5ee6521ac990
feature: Integrations
TQID: https://experienceleague.adobe.com/VrGVY61VlAmqLgSm6r2lCFHed5Cqn88mojgKZpP9-Lg
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b13bd2ad-8e65-49e5-9691-2a0d31067b35id: c5f60233-d5ea-4453-a799-0ad258b4d399
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 192
ht-degree: 5%

---

# Test [!DNL Facebook] annunci lead per l&#39;integrazione mobile con Marketo {#test-facebook-lead-ads-for-mobile-integration-with-marketo}

Dopo aver creato l’annuncio lead, devi testarlo.

>[!PREREQUISITES]
>
>È necessario [configurare l&#39;integrazione [!UICONTROL Facebook Lead Ads]](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md).

1. In [!UICONTROL Facebook Power Editor], selezionare una campagna, un annuncio e fare clic su **[!UICONTROL Edit]**.

1. In **[!UICONTROL Links]**, fare clic sul collegamento **[!UICONTROL View on mobile app]**.

   ![](assets/image2016-5-13-15-3a2-3a38.png)

1. Verrà inviata una nuova notifica all&#39;account [!DNL Facebook] a cui è possibile accedere sul dispositivo mobile con l&#39;account autorizzato. Fai clic su **[!UICONTROL OK]**.

   ![](assets/image2016-3-11-8-3a35-3a7.png)

1. Sul tuo dispositivo mobile, tocca **[!UICONTROL Notifications]** nell&#39;app mobile [!DNL Facebook].

   ![](assets/image2016-3-11-8-3a38-3a35.png)

1. In Notifiche, toccare **[!UICONTROL Your ad is ready to preview]**.

   ![](assets/image2016-3-11-8-3a41-3a59.png)

1. Invia l’unità di prova degli annunci lead toccando il Call to action e compilando il modulo creato.

   ![](assets/image2016-3-11-8-3a52-3a20.png)

   >[!NOTE]
   >
   >Questo è un esempio che utilizza un Call to action Ulteriori informazioni. Il Call to action dell&#39;unità annuncio lead potrebbe essere diverso.

1. Dopo aver inviato il modulo, [crea un elenco smart in Marketo](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md) come parte di un programma o nel database principale che utilizza il filtro **[!UICONTROL Filled Out Facebook Lead Ads Form]**. Inserire il nome del modulo lead annuncio del modulo inviato.

   ![](assets/image2016-3-11-8-3a59-3a34.png)

1. A questo punto, fare clic sulla scheda Lead per verificare che la sincronizzazione funzioni correttamente.

   ![](assets/image2016-3-11-15-3a27-3a54.png)

>[!NOTE]
>
>[Configura [!UICONTROL Facebook Lead Ads]](/help/marketo/product-docs/demand-generation/facebook/set-up-facebook-lead-ads.md)
