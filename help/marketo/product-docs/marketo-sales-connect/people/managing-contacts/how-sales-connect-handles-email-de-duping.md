---
unique-page-id: 14352514
description: Comprendere come Sales Connect gestisce la deduplicazione delle e-mail. Scopri come unire o gestire i contatti duplicati durante la sincronizzazione.
title: Gestione della deduplicazione delle e-mail in Sales Connect
exl-id: 1f57d943-8439-4653-a4e7-6dac65b3312d
feature: Marketo Sales Connect
TQID: https://experienceleague.adobe.com/gO6I2rCotAEDOGQNdRleeJbqMIix1wQizZe84JZSLPs
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: c5f60233-d5ea-4453-a799-0ad258b4d399
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 107
ht-degree: 6%

---

# Gestione della deduplicazione delle e-mail in [!DNL Sales Connect] {#how-sales-connect-handles-email-de-duping}

Quando [carichi un file CSV](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md) in [!DNL Sales Connect], tutti i contatti simili vengono uniti nel file CSV prima dell&#39;importazione.

Lo facciamo in base a un indirizzo e-mail simile. Quindi, se esistono due indirizzi e-mail identici, li uniamo in un unico contatto.

Se in seguito tenti di aggiungere/caricare manualmente lo stesso contatto, non verrà unito.

Se si tenta di aggiungere un contatto già presente nel database, non sarà possibile aggiungerlo.
