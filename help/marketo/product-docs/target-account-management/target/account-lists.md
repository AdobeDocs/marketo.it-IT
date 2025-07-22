---
unique-page-id: 11378814
description: '[!UICONTROL Account Lists] - Documentazione di Marketo - Documentazione del prodotto'
title: '[!UICONTROL Account Lists]'
exl-id: 31bb4341-d012-4239-8f40-10a07cd4c51c
feature: Target Account Management
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 0%

---

# [!UICONTROL Account Lists] {#account-lists}

Un elenco di account è un insieme di account denominati che possono essere oggetto di targeting. Gli elenchi di account consentono di eseguire il targeting degli account denominati per settore, posizione o dimensione dell’azienda.

Oltre agli elenchi di account, puoi anche creare elenchi di account dinamici generati dalle visualizzazioni account CRM pubbliche. Una visualizzazione account CRM è un insieme di regole che funge da filtro durante la visualizzazione degli account. Ad esempio, puoi utilizzarlo per trovare account in cui Industry is Healthcare *and* Revenue è superiore a $ 100 milioni.

![](assets/one.png)

>[!NOTE]
>
>Gli elenchi account creati in Marketo [!UICONTROL Target Account Management] sono automaticamente disponibili durante la creazione di elenchi avanzati e campagne Web in [Web Personalization](/help/marketo/product-docs/web-personalization/using-web-segments/web-segments.md).

## Crea un nuovo elenco account {#create-a-new-account-list}

1. Fare clic sul menu a discesa **[!UICONTROL New]** e selezionare **[!UICONTROL Create New Account List]**.

   ![](assets/1a.png)

1. Assegna un nome all&#39;elenco e fai clic su **[!UICONTROL Create]**.

   ![](assets/three-0.png)

1. Dopo aver creato l&#39;elenco degli account, inizia ad aggiungervi [account denominati](/help/marketo/product-docs/target-account-management/target/named-accounts/add-an-existing-named-account-to-an-account-list.md).

   >[!NOTE]
   >
   >In Marketo verranno visualizzate informazioni approfondite solo per gli elenchi di account con un massimo di 2.000 account denominati.

## Creare un nuovo elenco account dinamico {#create-a-new-dynamic-account-list}

1. Fare clic sul menu a discesa **[!UICONTROL New]** e selezionare **[!UICONTROL Create New Dynamic List]**.

   ![](assets/1.png)

1. Nella finestra di dialogo, seleziona una **Visualizzazione account CRM** dall&#39;elenco a discesa oppure digita il nome per cercarla.

   ![](assets/image2017-7-18-9-48-23.png)

1. Fai clic su **[!UICONTROL Create]**.

   ![](assets/step4.jpg)

   >[!NOTE]
   >
   >In Salesforce, assicurati di fornire all’utente di sincronizzazione le autorizzazioni per l’oggetto Visualizzazione elenco.

## Rinominare un elenco di account {#rename-an-account-list}

>[!NOTE]
>
>Questi passaggi si applicano solo agli elenchi di account. Gli elenchi di account _Dynamic_ utilizzano il nome delle visualizzazioni account CRM associate.

1. Selezionare l&#39;account che si desidera rinominare, fare clic sull&#39;elenco a discesa **[!UICONTROL Account List Actions]** e selezionare **[!UICONTROL Rename Account List]**.

   ![](assets/three.png)

1. Immettere il nuovo nome e fare clic su **[!UICONTROL Rename]**.

   ![](assets/four.png)

   >[!NOTE]
   >
   >La visualizzazione dell’account del sistema di gestione delle relazioni con i clienti viene sincronizzata con l’elenco degli account dinamici ogni 8 ore. Se non sono ancora sincronizzati, Marketo li sincronizzerà durante il ciclo successivo.

## Eliminare un elenco di account {#delete-an-account-list}

>[!NOTE]
>
>Questi passaggi sono gli stessi sia per gli elenchi account che per gli elenchi account dinamici.

1. Selezionare l&#39;account che si desidera eliminare, fare clic sull&#39;elenco a discesa **[!UICONTROL Account List Actions]** e selezionare **[!UICONTROL Delete Account List]**.

   ![](assets/five.png)

1. Fai clic su **[!UICONTROL Delete]**.

   ![](assets/six.png)

>[!MORELIKETHIS]
>
>* [Aggiungere un [!UICONTROL Named Account] esistente a un elenco account](/help/marketo/product-docs/target-account-management/target/named-accounts/add-an-existing-named-account-to-an-account-list.md)
>* [Informazioni elenco account](/help/marketo/product-docs/target-account-management/measure/account-list-insights.md)
