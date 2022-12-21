---
unique-page-id: 14352514
description: Gestione di Sales Connect per lo smantellamento delle e-mail - Documenti Marketo - Documentazione del prodotto
title: Gestione di Sales Connect per la disattivazione delle e-mail
exl-id: 1f57d943-8439-4653-a4e7-6dac65b3312d
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '100'
ht-degree: 0%

---

# Gestione di Sales Connect per la disattivazione delle e-mail {#how-sales-connect-handles-email-de-duping}

Quando sei [caricamento di un CSV](/help/marketo/product-docs/marketo-sales-connect/people/managing-contacts/import-contacts-via-csv.md) file in Sales Connect, uniamo tutti i contatti simili nel CSV prima dell&#39;importazione.

Lo facciamo in base ad un indirizzo e-mail simile. Quindi, se ci sono due indirizzi e-mail identici, li uniamo in un unico contatto.

Se in seguito tenti di aggiungere/caricare manualmente lo stesso contatto, non lo uniremo.

Se tenti di aggiungere un contatto già presente nel database, non potrai aggiungerlo.
