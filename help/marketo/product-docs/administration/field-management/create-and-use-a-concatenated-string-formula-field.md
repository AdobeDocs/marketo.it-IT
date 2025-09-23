---
unique-page-id: 2360337
description: Creare e utilizzare un campo Stringa concatenata (formula) - Documenti Marketo - Documentazione del prodotto
title: Creare e utilizzare un campo (formula) Stringa concatenata
exl-id: 779fbc56-a913-422a-a778-d86cc3ed7d48
feature: Field Management
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 13%

---

# Creare e utilizzare un campo (formula) Stringa concatenata {#create-and-use-a-concatenated-string-formula-field}

È possibile combinare valori provenienti da più campi o creare un valore condizionale utilizzando un campo formula di Marketo Engage.

1. Passa alla schermata **[!UICONTROL Admin]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-1.png)

1. Fai clic su **[!UICONTROL Field Management]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-2.png)

1. Fai clic su **[!UICONTROL New Custom Field]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-3.png)

1. Selezionare **[!UICONTROL Formula]** per **[!UICONTROL Type]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-4.png)

1. Immetti **[!UICONTROL Name]** per il campo, quindi fai clic su **[!UICONTROL Create]**.

   ![](assets/create-and-use-a-concatenated-string-formula-field-5.png)

1. Trovare e selezionare il campo formula, quindi fare clic su **[!UICONTROL Edit Rules]**.

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
