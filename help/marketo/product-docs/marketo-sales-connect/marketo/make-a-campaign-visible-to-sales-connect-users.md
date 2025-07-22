---
unique-page-id: 14745655
description: Rendere visibile una campagna agli utenti Sales Connect - Documenti Marketo - Documentazione del prodotto
title: Rendi una campagna visibile agli utenti Sales Connect
exl-id: 1fde53e3-2764-4e4b-897f-635b78534133
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '96'
ht-degree: 2%

---

# Rendi una campagna visibile a [!DNL Sales Connect] utenti {#make-a-campaign-visible-to-sales-connect-users}

Le campagne possono essere condivise solo se sono rese visibili. Ecco come farlo.

1. Seleziona (o crea) la campagna da condividere.

   ![](assets/make-a-marketing-campaign-visible-msc-1.png)

1. Fare clic sulla scheda **[!UICONTROL Smart List]**.

   ![](assets/make-a-marketing-campaign-visible-msc-2.png)

1. Aggiungi il trigger [!UICONTROL Campaign is Requested].

   ![](assets/make-a-marketing-campaign-visible-msc-3.png)

1. Per l&#39;origine, scegliere &quot;[!UICONTROL is]&quot; **[!UICONTROL Web Service API]**.

   ![](assets/make-a-marketing-campaign-visible-msc-4.png)

1. Fare clic sulla scheda **[!UICONTROL Flow]**.

   ![](assets/make-a-marketing-campaign-visible-msc-5.png)

1. Aggiungi l&#39;azione di flusso [!UICONTROL Interesting Moment].

   ![](assets/make-a-marketing-campaign-visible-msc-6.png)

1. Per [!UICONTROL Type], seleziona **[!UICONTROL Web]**.

   ![](assets/make-a-marketing-campaign-visible-msc-7.png)

1. Nella casella [!UICONTROL Description], scrivi un messaggio al team vendite. In questo esempio utilizziamo i token per specificare il modulo compilato.

   ![](assets/make-a-marketing-campaign-visible-msc-8.png)

1. Fare clic sulla scheda **[!UICONTROL Schedule]** e **[!UICONTROL Activate]** la campagna.

   ![](assets/make-a-marketing-campaign-visible-msc-9.png)
