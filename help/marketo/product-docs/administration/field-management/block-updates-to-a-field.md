---
unique-page-id: 2360291
description: Blocco degli aggiornamenti di un campo - Marketo Docs - Documentazione del prodotto
title: Blocca aggiornamenti di un campo
exl-id: 763097a3-cfa0-4df7-bfd1-40332b8dda1e
source-git-commit: 2776969be44ba1a3d795e99986d10cf0470fb9e9
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 0%

---

# Blocca aggiornamenti di un campo {#block-updates-to-a-field}

Il blocco degli aggiornamenti a un campo consente di scrivere una sola volta nel campo e quindi di mantenere il valore originale per la durata del campo. Può essere utile per un campo come Origine persona.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

1. Vai a **Amministratore** area.

   ![](assets/block-updates-to-a-field-1.png)

1. Fai clic su **Gestione dei campi**.

   ![](assets/block-updates-to-a-field-2.png)

1. Trova il campo, selezionalo, quindi sotto **Azioni campo**, fai clic su **Aggiornamenti dei campi di blocco**.

   ![](assets/block-updates-to-a-field-3.png)

   >[!NOTE]
   >
   >Puoi bloccare gli aggiornamenti di [Campi personalizzati membri del programma](/help/marketo/product-docs/core-marketo-concepts/programs/working-with-programs/program-member-custom-fields.md) anche.

1. Seleziona la **Sorgenti di input** si desidera bloccare e fare clic su **Applica**.

   ![](assets/block-updates-to-a-field-4.png)

   >[!CAUTION]
   >
   >Durante l’importazione di un elenco, lo stato di un campo bloccato nell’anteprima importazione viene visualizzato solo se il campo viene riconosciuto automaticamente da Marketo in base al nome del campo corrispondente _esattamente_ (o se sono stabiliti degli alias). Se il campo viene selezionato manualmente dal menu a discesa Campo Marketo, lo stato bloccato non verrà visualizzato nell’anteprima di importazione, ma il blocco dell’aggiornamento a tale campo verrà comunque implementato.
