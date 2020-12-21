---
unique-page-id: 11378814
description: Elenchi account - Documenti Marketo - Documentazione prodotto
title: Elenchi account
translation-type: tm+mt
source-git-commit: e125f8469239a026aefb703fdb6ba99c32e33565
workflow-type: tm+mt
source-wordcount: '341'
ht-degree: 0%

---


# Elenchi account {#account-lists}

Un elenco di account è un insieme di account denominati che possono essere utilizzati per il targeting insieme. Gli elenchi di account consentono di eseguire il targeting di account denominati per settore, posizione o dimensione della società.

Oltre agli elenchi degli account, puoi anche creare elenchi di account dinamici generati dalle viste account CRM pubbliche. Una vista account CRM è un insieme di regole che funge da filtro per la visualizzazione degli account. Ad esempio, è possibile utilizzarlo per trovare account in cui il settore sanitario *e* Ricavi è superiore a $100M.

![](assets/one.png)

>[!NOTE]
>
>Gli elenchi di account creati in Marketing basato su account Marketo sono automaticamente disponibili quando si creano elenchi smart e campagne Web in [Web Personalization](/help/marketo/product-docs/web-personalization/using-web-segments/web-segments.md).

## Crea nuovo elenco account {#create-a-new-account-list}

1. Fare clic sul menu a discesa **Nuovo** e selezionare **Crea nuovo elenco account**.

   ![](assets/1a.png)

1. Assegna un nome all&#39;elenco e fai clic su **Crea**.

   ![](assets/three-0.png)

1. Dopo aver creato l&#39;elenco degli account, iniziate dall&#39;aggiunta di [account denominati ](/help/marketo/product-docs/account-based-marketing/target/named-accounts/add-an-existing-named-account-to-an-account-list.md)!

   >[!NOTE]
   >
   >Marketo visualizzerà solo approfondimenti per gli elenchi di account con un massimo di 2.000 account denominati.

## Creare un nuovo elenco account dinamico {#create-a-new-dynamic-account-list}

1. Fare clic sul menu a discesa **Nuovo** e selezionare **Crea nuovo elenco dinamico**.

   ![](assets/1.png)

1. Nella finestra di dialogo, seleziona una **Vista account CRM** dall&#39;elenco a discesa, oppure digita il nome per cercarla.

   ![](assets/image2017-7-18-9-48-23.png)

1. Fare clic su **Crea**.

   ![](assets/step4.jpg)

   >[!NOTE]
   >
   >In Salesforce, accertatevi di fornire all’utente di sincronizzazione le autorizzazioni per l’oggetto Visualizzazione elenco.

## Rinominare un elenco di account {#rename-an-account-list}

>[!NOTE]
>
>Questi passaggi si applicano solo agli elenchi degli account. _Gli elenchi di account_ dinamici utilizzano il nome delle relative viste account CRM associate.

1. Selezionate l&#39;account da rinominare, fate clic sul menu a discesa **Azioni elenco account** e selezionate **Rinomina elenco account**.

   ![](assets/three.png)

1. Immettete il nuovo nome e fate clic su **Rinomina**.

   ![](assets/four.png)

   >[!NOTE]
   >
   >La vista account CRM si sincronizza con l&#39;elenco degli account dinamici ogni 8 ore. Se non sono ancora sincronizzati, Marketo li sincronizzerà durante il ciclo successivo.

## Eliminare un elenco di account {#delete-an-account-list}

>[!NOTE]
>
>Questi passaggi sono gli stessi per gli elenchi di account e per gli elenchi di account dinamici.

1. Selezionate l&#39;account da eliminare, fate clic sul menu a discesa **Azioni elenco account** e selezionate **Elimina elenco account**.

   ![](assets/five.png)

1. Fare clic su **Elimina**.

   ![](assets/six.png)

>[!MORELIKETHIS]
>
>* [Aggiunta di un account denominato esistente a un elenco account](/help/marketo/product-docs/account-based-marketing/target/named-accounts/add-an-existing-named-account-to-an-account-list.md)
>* [Approfondimenti elenco account](/help/marketo/product-docs/account-based-marketing/measure/account-list-insights.md)

