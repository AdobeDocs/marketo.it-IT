---
unique-page-id: 2949962
description: Attiva/disattiva dinamicamente la visibilità di un campo modulo - Documenti Marketo - Documentazione prodotto
title: Attiva/disattiva dinamicamente la visibilità di un campo modulo
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '211'
ht-degree: 0%

---


# Attiva/disattiva dinamicamente la visibilità di un campo modulo {#dynamically-toggle-visibility-of-a-form-field}

>[!PREREQUISITES]
>
>* [Aggiungere un elenco di selezione paese al modulo](../../../../product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md)

>



Una caratteristica davvero interessante dei moduli Marketo è che è possibile nascondere o mostrare in modo dinamico i campi dei moduli o [fieldsets](add-a-fieldset-to-a-form.md).

>[!NOTE]
>
>**Esempio**
>
>In questo esempio, è possibile nascondere il campo **State** a meno che **Country** non sia selezionato come &quot;Stati Uniti&quot;.

1. Andate a **Marketing** **Activities**.

   ![](assets/login-marketing-activities-8.png)

1. Selezionare il modulo e fare clic su **Modifica** **Modulo**.

   ![](assets/editform-1.png)

1. Selezionare il campo che si desidera nascondere o mostrare in modo dinamico e fare clic sul collegamento per **Visibilità** **Regole**.

   ![](assets/image2014-9-15-15-3a16-3a0.png)

1. Trovare e selezionare il campo da creare intorno a una condizione.

   ![](assets/image2014-9-15-15-3a16-3a12.png)

1. Selezionare l&#39;operatore.

   >[!TIP]
   >
   >Questo è fantastico perché potete scegliere corrispondenze sfocate come &quot;inizia con&quot;.

   ![](assets/image2014-9-15-15-3a16-3a50.png)

1. Selezionare i valori da cercare, quindi fare clic all&#39;esterno dell&#39;elenco a discesa.

   ![](assets/image2014-9-15-15-3a17-3a4.png)

   >[!TIP]
   >
   >È possibile selezionare più valori facendo clic su di essi mentre il menu a discesa è aperto. Ad esempio, potete selezionare Stati Uniti e Canada.

   >[!NOTE]
   >
   >In precedenza abbiamo convertito il Paese in un tipo di campo di selezione e [aggiunto tutti i paesi come valori](../../../../product-docs/demand-generation/forms/form-actions/add-a-country-picklist-to-your-form.md).

1. Fare clic su **Salva**.

   ![](assets/image2014-9-15-15-3a18-3a15.png)

Ed è tutto! Quando gli utenti compilano il modulo e selezionano Stati Uniti per Paese, il campo Stato viene visualizzato in modo dinamico con le opzioni specificate.

>[!NOTE]
>
>**Tubo profondo**
>
>Per saperne di più su [moduli](http://docs.marketo.com/display/docs/forms)?

