---
unique-page-id: 2360337
description: Creare e utilizzare un campo stringa concatenata (Formula) - Documenti Marketo - Documentazione del prodotto
title: Creare e utilizzare un campo stringa concatenata (formula)
translation-type: tm+mt
source-git-commit: 7b18fee7e376d6101cbeec45a3fcbaf1104c1bd0
workflow-type: tm+mt
source-wordcount: '172'
ht-degree: 0%

---


# Creare e utilizzare un campo stringa concatenata (formula) {#create-and-use-a-concatenated-string-formula-field}

È possibile combinare i valori provenienti da più campi o creare un valore condizionale utilizzando un campo Formula di Marketo.

1. Vai a **Amministratore** e fai clic su **Gestione campi**.

   ![](assets/image2014-9-19-9-3a44-3a58.png)

1. Fare clic su **Nuovo campo personalizzato**.

   ![](assets/image2014-9-19-9-3a45-3a8.png)

1. Selezionare **Formula** per **Tipo**.

   ![](assets/image2014-9-19-9-3a45-3a17.png)

1. Immetti un **Nome** per il campo, quindi fai clic su **Crea**.

   ![](assets/image2014-9-19-9-3a46-3a0.png)

1. Trova e seleziona il campo della formula, quindi fai clic su **Modifica regole**.

   ![](assets/image2014-9-19-9-3a46-3a13.png)

1. Aggiungi due scelte e definiscile come la schermata sottostante.

   ![](assets/image2014-9-19-9-3a46-3a25.png)

   >[!TIP]
   >
   >Ulteriori informazioni sui [token per i passaggi di flusso](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md).

1. Ora puoi aggiungere il campo della formula come token in un messaggio e-mail.

   ![](assets/seven.png)

>[!NOTE]
>
>I campi Formula possono essere utilizzati nelle colonne delle pagine di destinazione, delle e-mail e degli elenchi avanzati (non vengono esportati). Le e-mail con campi formula possono **non** essere inviate utilizzando una campagna batch. In questo scenario, utilizza un [token di script e-mail](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md).

Ottimo lavoro! Ora avete un campo intelligente che sa quale saluto includere in base al genere. Divertitevi con questo e diventate creativi.
