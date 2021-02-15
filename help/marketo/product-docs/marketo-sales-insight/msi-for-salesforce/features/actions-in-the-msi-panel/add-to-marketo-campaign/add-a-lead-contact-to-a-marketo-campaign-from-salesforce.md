---
unique-page-id: 10099167
description: Aggiunta di un lead/contatto a una campagna Marketo da Salesforce - Documenti Marketo - Documentazione del prodotto
title: Aggiunta di un lead/contatto a una campagna marketing da Salesforce
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '182'
ht-degree: 0%

---


# Aggiunta di un lead/contatto a una campagna marketing da Salesforce {#add-a-lead-contact-to-a-marketo-campaign-from-salesforce}

Puoi facilmente aggiungere lead o contatti alle campagne smart di Marketo direttamente da Salesforce. Ecco come, usare i lead.

1. In Salesforce, fare clic sulla scheda **Lead**.

   ![](assets/image2016-3-22-9-3a18-3a36.png)

1. Selezionate dall&#39;elenco a discesa l&#39;elenco delle persone da visualizzare e fate clic su **Go**.

   ![](assets/image2016-3-22-9-3a24-3a6.png)

   >[!NOTE]
   >
   >L&#39;elenco a discesa include Tutti i lead aperti o non letti, i lead visualizzati di recente, i lead di oggi e possono includere altre categorie.

1. Selezionate un lead dall’elenco per aprire il record.

   ![](assets/three.png)

1. Nel record, scorrete verso il basso fino all&#39;area Visiva marketing, fate clic sul menu a discesa **Azioni**, selezionate **Aggiungi a campagna marketing**, quindi fate clic su **Vai**.

   ![](assets/four.png)

1. Fai clic sul menu a discesa **Nome campagna**, seleziona la campagna Marketo desiderata, quindi fai clic su **Aggiungi a campagna marketing**.

   ![](assets/five.png)

   >[!NOTE]
   >
   >Affinché la campagna venga visualizzata nell&#39;elenco a discesa, utilizzate il trigger [**Campaign is Required**](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/using-smart-campaigns/setting-up-a-trigger-smart-campaign-for-sales-using-campaign-is-requested.md), con **Sales Insight** come origine, quando configurate la campagna.

Ed è tutto! La persona viene aggiunta alla campagna Marketo.
