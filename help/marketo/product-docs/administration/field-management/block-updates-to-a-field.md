---
unique-page-id: 2360291
description: Blocca aggiornamenti a un campo - Documenti Marketo - Documentazione prodotto
title: Blocca aggiornamenti a un campo
translation-type: tm+mt
source-git-commit: f865630638e7c0fe6ac2a449e196a7de4fbfeea1
workflow-type: tm+mt
source-wordcount: '159'
ht-degree: 0%

---


# Blocca aggiornamenti a un campo {#block-updates-to-a-field}

Il blocco degli aggiornamenti a un campo consente di scrivere sul campo una sola volta e di mantenere il valore originale per la durata del campo. Questo può essere utile per un campo come Origine persona.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

1. Accedete a **Admin** e fate clic su **Field Management**.

   ![](assets/image2014-9-24-13-3a54-3a40.png)

1. Trovare il campo, selezionarlo, quindi in **Azioni campo** fare clic su **Blocca aggiornamenti campo**.

   ![](assets/two-1.png)

1. Selezionare le **Origini di input** che si desidera bloccare e fare clic su **Applica**.

   ![](assets/image2014-9-24-13-3a55-3a16.png)

   >[!CAUTION]
   >
   >Durante l&#39;importazione di un elenco, lo stato di un campo bloccato nell&#39;anteprima di importazione viene visualizzato solo se il campo viene riconosciuto automaticamente da Marketo in base al nome del campo corrispondente a _esattamente_ (o se sono stabiliti degli alias). Se il campo viene selezionato manualmente dal menu a discesa Campo Marketo, lo stato bloccato non viene visualizzato nell’anteprima di importazione, ma il blocco degli aggiornamenti a tale campo viene comunque implementato.
