---
unique-page-id: 14352514
description: In che modo Sales Connect gestisce la deduplicazione delle e-mail - Documenti Marketo - Documentazione del prodotto
title: Gestione della deduplicazione delle e-mail in Sales Connect
exl-id: 1f57d943-8439-4653-a4e7-6dac65b3312d
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 0%

---

# Gestione della deduplicazione delle e-mail in Sales Connect {#how-sales-connect-handles-email-de-duping}

Quando sei [caricamento di un file CSV](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md) In Sales Connect, tutti i contatti simili vengono uniti nel file CSV prima dell&#39;importazione.

Lo facciamo in base a un indirizzo e-mail simile. Quindi, se esistono due indirizzi e-mail identici, li uniamo in un unico contatto.

Se in seguito tenti di aggiungere/caricare manualmente lo stesso contatto, non verrà unito.

Se si tenta di aggiungere un contatto già presente nel database, non sarà possibile aggiungerlo.
