---
unique-page-id: 11378814
description: Elenchi account - Documentazione di Marketo - Documentazione del prodotto
title: Elenchi account
exl-id: 31bb4341-d012-4239-8f40-10a07cd4c51c
feature: Target Account Management
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '343'
ht-degree: 0%

---

# Elenchi account {#account-lists}

Un elenco di account è un insieme di account denominati che possono essere oggetto di targeting. Gli elenchi di account consentono di eseguire il targeting degli account denominati per settore, posizione o dimensione dell’azienda.

Oltre agli elenchi di account, puoi anche creare elenchi di account dinamici generati dalle visualizzazioni account CRM pubbliche. Una visualizzazione account CRM è un insieme di regole che funge da filtro durante la visualizzazione degli account. Ad esempio, puoi utilizzarlo per trovare account in cui Industry is Healthcare *and* Revenue è superiore a $ 100 milioni.

![](assets/one.png)

>[!NOTE]
>
>Gli elenchi account creati in Gestione account di Marketo Target sono automaticamente disponibili quando si creano elenchi avanzati e campagne Web in [Web Personalization](/help/marketo/product-docs/web-personalization/using-web-segments/web-segments.md).

## Crea un nuovo elenco account {#create-a-new-account-list}

1. Fai clic sul menu a discesa **Nuovo** e seleziona **Crea nuovo elenco account**.

   ![](assets/1a.png)

1. Assegna un nome all&#39;elenco e fai clic su **Crea**.

   ![](assets/three-0.png)

1. Dopo aver creato l&#39;elenco degli account, inizia ad aggiungervi [account denominati](/help/marketo/product-docs/target-account-management/target/named-accounts/add-an-existing-named-account-to-an-account-list.md).

   >[!NOTE]
   >
   >In Marketo verranno visualizzate informazioni approfondite solo per gli elenchi di account con un massimo di 2.000 account denominati.

## Creare un nuovo elenco account dinamico {#create-a-new-dynamic-account-list}

1. Fai clic sul menu a discesa **Nuovo** e seleziona **Crea nuovo elenco dinamico**.

   ![](assets/1.png)

1. Nella finestra di dialogo, seleziona una **Visualizzazione account CRM** dall&#39;elenco a discesa oppure digita il nome per cercarla.

   ![](assets/image2017-7-18-9-48-23.png)

1. Fai clic su **Crea**.

   ![](assets/step4.jpg)

   >[!NOTE]
   >
   >In Salesforce, assicurati di fornire all’utente di sincronizzazione le autorizzazioni per gli oggetti Vista a elenco.

## Rinominare un elenco di account {#rename-an-account-list}

>[!NOTE]
>
>Questi passaggi si applicano solo agli elenchi di account. Gli elenchi di account _Dynamic_ utilizzano il nome delle visualizzazioni account CRM associate.

1. Selezionare l&#39;account che si desidera rinominare, fare clic sull&#39;elenco a discesa **Azioni elenco account** e selezionare **Rinomina elenco account**.

   ![](assets/three.png)

1. Immettere il nuovo nome e fare clic su **Rinomina**.

   ![](assets/four.png)

   >[!NOTE]
   >
   >La visualizzazione dell’account del sistema di gestione delle relazioni con i clienti viene sincronizzata con l’elenco degli account dinamici ogni 8 ore. Se non sono ancora sincronizzati, Marketo li sincronizzerà durante il ciclo successivo.

## Eliminare un elenco di account {#delete-an-account-list}

>[!NOTE]
>
>Questi passaggi sono gli stessi sia per gli elenchi account che per gli elenchi account dinamici.

1. Selezionare l&#39;account da eliminare, fare clic sull&#39;elenco a discesa **Azioni elenco account** e selezionare **Elimina elenco account**.

   ![](assets/five.png)

1. Fare clic su **Elimina**.

   ![](assets/six.png)

>[!MORELIKETHIS]
>
>* [Aggiungere un account denominato esistente a un elenco di account](/help/marketo/product-docs/target-account-management/target/named-accounts/add-an-existing-named-account-to-an-account-list.md)
>* [Informazioni elenco account](/help/marketo/product-docs/target-account-management/measure/account-list-insights.md)
