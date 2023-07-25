---
unique-page-id: 2360337
description: Creare e utilizzare un campo Stringa concatenata (formula) - Documenti Marketo - Documentazione del prodotto
title: Creare e utilizzare un campo Stringa concatenata (formula)
exl-id: 779fbc56-a913-422a-a778-d86cc3ed7d48
feature: Field Management
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '173'
ht-degree: 0%

---

# Creare e utilizzare un campo Stringa concatenata (formula) {#create-and-use-a-concatenated-string-formula-field}

È possibile combinare valori provenienti da più campi o creare un valore condizionale utilizzando un campo Formula di Marketo.

1. Vai a **[!UICONTROL Amministratore]** area.

   ![](assets/create-and-use-a-concatenated-string-formula-field-1.png)

1. Clic **[!UICONTROL Gestione dei campi]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-2.png)

1. Clic **[!UICONTROL Nuovo campo personalizzato]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-3.png)

1. Seleziona **[!UICONTROL Formula]** per **[!UICONTROL Tipo]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-4.png)

1. Immetti un **[!UICONTROL Nome]** per il campo, quindi fai clic su **[!UICONTROL Crea]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-5.png)

1. Individuare e selezionare il campo formula, quindi fare clic su **[!UICONTROL Modifica regole]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-6.png)

1. Aggiungi due scelte e definiscili come nella schermata seguente.

   ![](assets/create-and-use-a-concatenated-string-formula-field-7.png)

   >[!TIP]
   >
   >Ulteriori informazioni su [token per le fasi del flusso](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md).

1. Ora puoi aggiungere il campo formula come token in un messaggio e-mail.

   ![](assets/create-and-use-a-concatenated-string-formula-field-8.png)

>[!NOTE]
>
>I campi formula possono essere utilizzati nelle colonne delle pagine di destinazione, delle e-mail e dell’elenco avanzato (non vengono esportati). Le e-mail con campi formula possono _non_ essere inviato utilizzando una campagna batch. Utilizza un [token di script e-mail](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md) in questo scenario.

Ottimo lavoro! Ora hai un campo intelligente che sa quale formula di saluto includere in base al sesso. Divertitevi e diventate creativi.
