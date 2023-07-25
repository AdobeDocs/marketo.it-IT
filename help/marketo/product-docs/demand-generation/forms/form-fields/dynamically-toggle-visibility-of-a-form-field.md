---
unique-page-id: 2949962
description: Attivazione/disattivazione dinamica della visibilità di un campo modulo - Documentazione di Marketo - Documentazione del prodotto
title: Attivazione/disattivazione dinamica della visibilità di un campo modulo
exl-id: 51b9283d-bfa1-4535-89ba-96c0ae2ea909
feature: Forms
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '243'
ht-degree: 0%

---

# Attivazione/disattivazione dinamica della visibilità di un campo modulo {#dynamically-toggle-visibility-of-a-form-field}

>[!PREREQUISITES]
>
>* [Aggiungere una lista di selezione del paese al modulo](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md)

Una caratteristica molto interessante di Marketo Forms è la possibilità di nascondere/visualizzare dinamicamente i campi del modulo o [set di campi](/help/marketo/product-docs/demand-generation/forms/form-fields/add-a-fieldset-to-a-form.md).

>[!NOTE]
>
>**Esempio**
>
>In questo esempio, nascondiamo il **Stato** campo a meno che **Paese** viene selezionato come &quot;Stati Uniti&quot;.

1. Vai a **Attività di marketing**.

   ![](assets/login-marketing-activities-8.png)

1. Seleziona il modulo e fai clic su **Modifica modulo**.

   ![](assets/editform-1.png)

1. Seleziona il campo da nascondere/mostrare dinamicamente e fai clic sul collegamento per **Regole di visibilità**.

   ![](assets/image2014-9-15-15-3a16-3a0.png)

1. Trova e seleziona il campo in cui desideri creare una condizione.

   ![](assets/image2014-9-15-15-3a16-3a12.png)

1. Seleziona l’operatore.

   >[!TIP]
   >
   >Questo è bello perché puoi scegliere corrispondenze sfocate come &quot;inizia con&quot;.

   ![](assets/image2014-9-15-15-3a16-3a50.png)

1. Seleziona i valori da cercare, quindi fai clic all’esterno del menu a discesa.

   ![](assets/image2014-9-15-15-3a17-3a4.png)

   >[!TIP]
   >
   >Puoi selezionare più valori facendo clic su di essi mentre il menu a discesa è aperto. Ad esempio, è possibile selezionare Stati Uniti e Canada.

   >[!NOTE]
   >
   >Abbiamo precedentemente convertito il paese in un tipo di campo elenco di selezione e [ha aggiunto tutti i paesi come valori](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md).

1. Clic **Salva**.

   ![](assets/image2014-9-15-15-3a18-3a15.png)

Ed è tutto! Ora, quando gli utenti compilano questo modulo e selezionano Stati Uniti per Paese, il campo Stato viene visualizzato in modo dinamico con le scelte specificate.

>[!IMPORTANT]
>
>Il comportamento del campo modulo funziona perfettamente quando i valori dei campi vengono impostati/aggiornati tramite script personalizzato utilizzando [Funzioni API](https://developers.marketo.com/javascript-api/forms/){target="_blank"} in Forms 2.0.
>
>I campi condizionali potrebbero non funzionare come previsto se i valori dei campi vengono modificati da script esterni diversi dall’API JavaScript di Forms 2.0.
