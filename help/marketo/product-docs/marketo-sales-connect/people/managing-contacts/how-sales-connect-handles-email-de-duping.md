---
unique-page-id: 14352514
description: Come il servizio di vendita Connect gestisce la disattivazione delle e-mail - Documenti Marketo - Documentazione del prodotto
title: Gestione della disattivazione delle e-mail in Adobe Connect
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '104'
ht-degree: 0%

---


# Gestione della disattivazione delle e-mail da parte di Adobe Connect{#how-sales-connect-handles-email-de-duping}

Durante il [caricamento di un file CSV](http://docs.marketo.com/x/VADb) in Sales Connect, uniamo tutti i contatti simili nel CSV prima dell&#39;importazione.

Lo facciamo sulla base di un indirizzo e-mail simile. Quindi, se ci sono due indirizzi e-mail identici, li uniamo in un unico contatto.

Se successivamente tentate di aggiungere o caricare manualmente lo stesso contatto, non lo uniremo.

Se si tenta di aggiungere un contatto già presente nel database, non sarà possibile aggiungerlo.

