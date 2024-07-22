---
unique-page-id: 2360337
description: Creare e utilizzare un campo Stringa concatenata (formula) - Documenti Marketo - Documentazione del prodotto
title: Creare e utilizzare un campo Stringa concatenata (formula)
exl-id: 779fbc56-a913-422a-a778-d86cc3ed7d48
feature: Field Management
source-git-commit: 9181a599ae715e9ffcfd84d8316dfa1c094329a6
workflow-type: tm+mt
source-wordcount: '170'
ht-degree: 0%

---

# Creare e utilizzare un campo Stringa concatenata (formula) {#create-and-use-a-concatenated-string-formula-field}

È possibile combinare valori provenienti da più campi o creare un valore condizionale utilizzando un campo formula di Marketo Engage.

1. Vai all&#39;area **[!UICONTROL Amministratore]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-1.png)

1. Fare clic su **[!UICONTROL Gestione campi]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-2.png)

1. Fare clic su **[!UICONTROL Nuovo campo personalizzato]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-3.png)

1. Selezionare **[!UICONTROL Formula]** per **[!UICONTROL Tipo]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-4.png)

1. Immetti un **[!UICONTROL Nome]** per il campo, quindi fai clic su **[!UICONTROL Crea]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-5.png)

1. Trova e seleziona il campo formula, quindi fai clic su **[!UICONTROL Modifica regole]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-6.png)

1. Aggiungi due scelte e definiscili come nella schermata seguente.

   ![](assets/create-and-use-a-concatenated-string-formula-field-7.png)

   >[!TIP]
   >
   >Ulteriori informazioni sui [token per i passaggi del flusso](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/use-tokens-in-flow-steps.md).

1. Ora puoi aggiungere il campo formula come token in un messaggio e-mail.

   ![](assets/create-and-use-a-concatenated-string-formula-field-8.png)

>[!NOTE]
>
>I campi formula possono essere utilizzati nelle colonne Pagine di destinazione, E-mail ed Elenco avanzato. Le e-mail con campi formula possono _non_ essere inviate utilizzando una campagna batch. In questo scenario, utilizza un [token di script e-mail](/help/marketo/product-docs/email-marketing/general/using-tokens/create-an-email-script-token.md).

Ottimo lavoro! Ora hai un campo intelligente che sa quale formula di saluto includere in base al sesso. Divertitevi e diventate creativi.
