---
unique-page-id: 2360291
description: Blocco degli aggiornamenti di un campo - Marketo Docs - Documentazione del prodotto
title: Blocca aggiornamenti di un campo
exl-id: 763097a3-cfa0-4df7-bfd1-40332b8dda1e
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 0%

---

# Blocca aggiornamenti a un campo {#block-updates-to-a-field}

Il blocco degli aggiornamenti a un campo consente di scrivere una sola volta nel campo e quindi di mantenere il valore originale per la durata del campo. Può essere utile per un campo come Origine persona.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

1. Vai a **Amministratore** e fai clic su **Gestione campi**.

   ![](assets/image2014-9-24-13-3a54-3a40.png)

1. Trova il campo, selezionalo, quindi in **Azioni campo** fai clic su **Blocca aggiornamenti campo**.

   ![](assets/two-1.png)

   >[!NOTE]
   >
   >È possibile bloccare anche gli aggiornamenti a [Campi personalizzati dei membri del programma](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md).

1. Selezionare le **Origini di input** che si desidera bloccare e fare clic su **Applica**.

   ![](assets/image2014-9-24-13-3a55-3a16.png)

   >[!CAUTION]
   >
   >Durante l’importazione di un elenco, lo stato di un campo bloccato nell’anteprima importazione viene visualizzato solo se il campo viene riconosciuto automaticamente da Marketo in base al nome del campo corrispondente _esattamente_ (o se sono stabiliti alias). Se il campo viene selezionato manualmente dal menu a discesa Campo Marketo, lo stato bloccato non verrà visualizzato nell’anteprima di importazione, ma il blocco dell’aggiornamento a tale campo verrà comunque implementato.
