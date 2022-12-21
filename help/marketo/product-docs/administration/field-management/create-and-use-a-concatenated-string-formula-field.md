---
unique-page-id: 2360337
description: Creare e utilizzare un campo stringa concatenata (Formula) - Marketo Docs - Documentazione del prodotto
title: Creare e utilizzare un campo stringa concatenata (formula)
exl-id: 779fbc56-a913-422a-a778-d86cc3ed7d48
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 0%

---

# Creare e utilizzare un campo stringa concatenata (formula) {#create-and-use-a-concatenated-string-formula-field}

È possibile combinare i valori provenienti da più campi o creare un valore condizionale utilizzando un campo Formula di Marketo.

1. Vai a **Amministratore** e fai clic su **Gestione dei campi**.

   ![](assets/image2014-9-19-9-3a44-3a58.png)

1. Fai clic su **Nuovo campo personalizzato**.

   ![](assets/image2014-9-19-9-3a45-3a8.png)

1. Seleziona **Formula** per **Tipo**.

   ![](assets/image2014-9-19-9-3a45-3a17.png)

1. Inserisci un **Nome** per il campo, fai clic su **Crea**.

   ![](assets/image2014-9-19-9-3a46-3a0.png)

1. Trova e seleziona il campo formula, quindi fai clic su **Modifica regole**.

   ![](assets/image2014-9-19-9-3a46-3a13.png)

1. Aggiungi due scelte e definiscile come la schermata sottostante.

   ![](assets/image2014-9-19-9-3a46-3a25.png)

   >[!TIP]
   >
   >Ulteriori informazioni [token per i passaggi di flusso](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md).

1. Ora puoi aggiungere il campo della formula come token in un messaggio e-mail.

   ![](assets/seven.png)

>[!NOTE]
>
>I campi Formula possono essere utilizzati nelle colonne delle pagine di destinazione, delle e-mail e degli elenchi avanzati (non vengono esportati). Le e-mail con campi formula possono **not** essere inviati utilizzando una campagna batch. Utilizza un [token di script e-mail](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md) in questo scenario.

Ottimo lavoro! Ora avete un campo intelligente che sa quale saluto includere in base al genere. Divertitevi con questo e diventate creativi.
