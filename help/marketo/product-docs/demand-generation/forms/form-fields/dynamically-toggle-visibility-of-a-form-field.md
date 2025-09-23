---
unique-page-id: 2949962
description: Attivazione/disattivazione dinamica della visibilità di un campo modulo - Documentazione di Marketo - Documentazione del prodotto
title: Attivazione/disattivazione dinamica della visibilità di un campo modulo
exl-id: 51b9283d-bfa1-4535-89ba-96c0ae2ea909
feature: Forms
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 8%

---

# Attivazione/disattivazione dinamica della visibilità di un campo modulo {#dynamically-toggle-visibility-of-a-form-field}

>[!PREREQUISITES]
>
>* [Aggiungi un elenco a discesa Paese al modulo](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md)

Una caratteristica molto interessante di Marketo Forms è la possibilità di nascondere/visualizzare dinamicamente i campi o [set di campi](/help/marketo/product-docs/demand-generation/forms/form-fields/add-a-fieldset-to-a-form.md).

>[!NOTE]
>
>**Esempio**
>
>In questo esempio, nascondiamo il campo **Stato** a meno che **Paese** non sia selezionato come &quot;Stati Uniti&quot;.

1. Vai a **[!UICONTROL Marketing Activities]**.

   ![](assets/login-marketing-activities-8.png)

1. Selezionare il modulo e fare clic su **[!UICONTROL Edit Form]**.

   ![](assets/editform-1.png)

1. Selezionare il campo che si desidera nascondere/visualizzare dinamicamente e fare clic sul collegamento per **[!UICONTROL Visibility Rules]**.

   ![](assets/image2014-9-15-15-3a16-3a0.png)

1. Trova e seleziona il campo in cui desideri creare una condizione.

   ![](assets/image2014-9-15-15-3a16-3a12.png)

1. Seleziona l&#39;operatore.

   >[!TIP]
   >
   >Non è male perché puoi scegliere corrispondenze sfocate come &quot;[!UICONTROL starts with]&quot;.

   ![](assets/image2014-9-15-15-3a16-3a50.png)

1. Seleziona i valori da cercare, quindi fai clic all’esterno del menu a discesa.

   ![](assets/image2014-9-15-15-3a17-3a4.png)

   >[!TIP]
   >
   >Puoi selezionare più valori facendo clic su di essi mentre il menu a discesa è aperto. Ad esempio, è possibile selezionare Stati Uniti e Canada.

   >[!NOTE]
   >
   >In precedenza il campo Paese era stato convertito in un tipo di campo elenco di selezione e [tutti i paesi sono stati aggiunti come valori](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md).

1. Fai clic su **[!UICONTROL Save]**.

   ![](assets/image2014-9-15-15-3a18-3a15.png)

Ed è tutto! Ora, quando gli utenti compilano questo modulo e selezionano Stati Uniti per Paese, il campo Stato viene visualizzato in modo dinamico con le scelte specificate.

>[!IMPORTANT]
>
>Il comportamento del campo modulo funzionerà senza problemi quando i valori dei campi vengono impostati/aggiornati tramite script personalizzato utilizzando [funzioni API](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/javascriptapi/forms-api-reference){target="_blank"} in Forms 2.0.
>
>I campi condizionali potrebbero non funzionare come previsto se i valori dei campi vengono modificati da script esterni diversi dall’API JavaScript di Forms 2.0.
