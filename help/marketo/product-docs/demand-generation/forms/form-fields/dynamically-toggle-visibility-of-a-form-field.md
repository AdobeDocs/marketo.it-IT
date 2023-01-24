---
unique-page-id: 2949962
description: Attivare o disattivare dinamicamente la visibilità di un campo modulo - Documenti Marketo - Documentazione del prodotto
title: Attiva/disattiva dinamicamente la visibilità di un campo modulo
exl-id: 51b9283d-bfa1-4535-89ba-96c0ae2ea909
source-git-commit: 0aa754bb3fb9057aaec87dc41743711fb15f8d62
workflow-type: tm+mt
source-wordcount: '243'
ht-degree: 0%

---

# Attiva/disattiva dinamicamente la visibilità di un campo modulo {#dynamically-toggle-visibility-of-a-form-field}

>[!PREREQUISITES]
>
>* [Aggiungere una lista di selezione per paese al modulo](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md)


Una caratteristica davvero interessante dei moduli Marketo è che è possibile nascondere/mostrare dinamicamente i campi del modulo o [fielset](/help/marketo/product-docs/demand-generation/forms/form-fields/add-a-fieldset-to-a-form.md).

>[!NOTE]
>
>**Esempio**
>
>In questo esempio, nascondiamo il **Stato** campo a meno che **Paese** viene selezionato come &quot;Stati Uniti&quot;.

1. Vai a **Attività di marketing**.

   ![](assets/login-marketing-activities-8.png)

1. Seleziona il modulo e fai clic su **Modifica modulo**.

   ![](assets/editform-1.png)

1. Seleziona il campo da nascondere o mostrare dinamicamente e fai clic sul collegamento per **Regole di visibilità**.

   ![](assets/image2014-9-15-15-3a16-3a0.png)

1. Trova e seleziona il campo intorno al quale desideri creare una condizione.

   ![](assets/image2014-9-15-15-3a16-3a12.png)

1. Seleziona l’operatore .

   >[!TIP]
   >
   >Questo è fantastico perché puoi scegliere fiamme corrispondenze come &quot;inizia con&quot;.

   ![](assets/image2014-9-15-15-3a16-3a50.png)

1. Seleziona i valori da cercare, quindi fai clic all’esterno del menu a discesa.

   ![](assets/image2014-9-15-15-3a17-3a4.png)

   >[!TIP]
   >
   >È possibile selezionare più valori facendo clic su di essi mentre il menu a discesa è aperto. Ad esempio, è possibile selezionare Stati Uniti e Canada.

   >[!NOTE]
   >
   >Precedentemente il paese è stato convertito in un tipo di campo elenco di selezione e [ha aggiunto tutti i paesi come valori](/help/marketo/product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md).

1. Fai clic su **Salva**.

   ![](assets/image2014-9-15-15-3a18-3a15.png)

Ed è tutto! Ora, quando gli utenti compilano il modulo e selezionano Stati Uniti per paese, il campo Stato verrà visualizzato in modo dinamico con le opzioni specificate.

>[!IMPORTANT]
>
>Il comportamento del campo del modulo funzionerà senza problemi quando i valori dei campi vengono impostati/aggiornati tramite script personalizzati utilizzando [Funzioni API](https://developers.marketo.com/javascript-api/forms/){target="_blank"} in Forms 2.0.
>
>I campi condizionali potrebbero non funzionare come previsto se i valori dei campi vengono modificati da script esterni diversi dall’API JavaScript Forms 2.0.
