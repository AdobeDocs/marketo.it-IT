---
description: In che modo le azioni di approfondimento sulle vendite gestiscono la rimozione delle e-mail - Documenti Marketo - Documentazione del prodotto
title: In che modo le azioni di approfondimento sulle vendite gestiscono la deduplicazione delle e-mail
exl-id: 40b01f7f-df50-4bd2-ac35-4c4e4f80915e
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '107'
ht-degree: 0%

---

# In Che Modo Le Azioni Di Insight Sulle Vendite Gestiscono La Deduplicazione Delle E-Mail? {#how-does-sales-insight-actions-handle-email-de-duping}

Quando sei [caricamento di un file CSV](/help/marketo/product-docs/marketo-sales-insight/actions/people/managing-contacts/import-contacts-via-csv.md) nelle azioni di approfondimento sulle vendite, uniamo tutti i contatti simili nel file CSV prima dell’importazione.

Lo facciamo in base a un indirizzo e-mail simile. Quindi, se esistono due indirizzi e-mail identici, li uniamo in un unico contatto.

Se in seguito tenti di aggiungere/caricare manualmente lo stesso contatto, non verrà unito.

Se si tenta di aggiungere un contatto già presente nel database, non sarà possibile aggiungerlo.
