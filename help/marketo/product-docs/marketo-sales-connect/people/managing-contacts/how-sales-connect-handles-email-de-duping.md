---
unique-page-id: 14352514
description: Comprendere come Sales Connect gestisce la deduplicazione delle e-mail. Scopri come unire o gestire i contatti duplicati durante la sincronizzazione.
title: Gestione della deduplicazione delle e-mail in Sales Connect
exl-id: 1f57d943-8439-4653-a4e7-6dac65b3312d
feature: Marketo Sales Connect
source-git-commit: 15427eacd2fc42a02f6a4c59d9102bacba02e57b
workflow-type: tm+mt
source-wordcount: '103'
ht-degree: 5%

---

# Gestione della deduplicazione delle e-mail in [!DNL Sales Connect] {#how-sales-connect-handles-email-de-duping}

Quando [carichi un file CSV](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md) in [!DNL Sales Connect], tutti i contatti simili vengono uniti nel file CSV prima dell&#39;importazione.

Lo facciamo in base a un indirizzo e-mail simile. Quindi, se esistono due indirizzi e-mail identici, li uniamo in un unico contatto.

Se in seguito tenti di aggiungere/caricare manualmente lo stesso contatto, non verrà unito.

Se si tenta di aggiungere un contatto già presente nel database, non sarà possibile aggiungerlo.
