---
solution: Marketo Engage
product: marketo
title: Frammenti personalizzabili
description: Scopri come personalizzare i frammenti rendendo modificabili alcuni dei loro campi.
level: Beginner, Intermediate
feature: Email Designer
role: User
exl-id: 3e0232c7-13bd-49e2-b7c7-cd389b5f0704
source-git-commit: cc6c04ca8a72f6efb0bec93cba084fe2993f53f0
workflow-type: tm+mt
source-wordcount: '409'
ht-degree: 1%

---

# Frammenti personalizzabili {#customizable-fragments}

I frammenti utilizzati in un’e-mail o in un modello e-mail sono bloccati per impostazione predefinita a causa dell’ereditarietà. Ciò significa che eventuali modifiche apportate a un frammento vengono propagate automaticamente a tutte le risorse in cui viene utilizzato il frammento. Con i frammenti personalizzabili, campi specifici all’interno di un frammento possono essere definiti come modificabili quando il frammento viene aggiunto a un’e-mail o a un modello e-mail. Supponiamo ad esempio di avere un frammento con un banner, del testo e un pulsante. È possibile designare come modificabili alcuni campi, ad esempio l’URL di destinazione dell’immagine o del pulsante. Questo consente agli utenti di modificare questi elementi quando incorporano il frammento nel modello e-mail/e-mail, offrendo un’esperienza personalizzata senza influire sul frammento originale.

Sfruttando frammenti personalizzabili, puoi gestire e personalizzare in modo efficiente i contenuti senza creare blocchi di contenuto completamente nuovi o interrompere l’ereditarietà dal frammento originale. In questo modo, le modifiche apportate a livello di frammento vengono comunque propagate, consentendo al contempo la necessaria personalizzazione a livello di e-mail/modello e-mail.

I frammenti visivi e di espressione possono essere contrassegnati come personalizzabili. Per istruzioni dettagliate su come procedere con ciascun tipo di frammento, consulta le sezioni seguenti.

## Aggiungere campi modificabili nei frammenti visivi {#visual}

Per rendere modificabili parti di un frammento visivo, effettua le seguenti operazioni:

>[!NOTE]
>
>I campi modificabili possono essere aggiunti ai componenti **image**, **text** e **button**. Per i componenti di **HTML**, i campi modificabili vengono aggiunti utilizzando l&#39;editor di personalizzazione, in modo simile ai frammenti di espressione. [Scopri come aggiungere un campo modificabile nei componenti e nei frammenti di espressione di HTML](#expression)

1. Apri la schermata di modifica del contenuto del frammento.

1. Seleziona il componente nel frammento in cui desideri configurare i campi modificabili.

1. Il riquadro delle proprietà del componente viene visualizzato sul lato destro. Selezionare la scheda **[!UICONTROL Editable fields]**, quindi attivare/disattivare l&#39;opzione **[!UICONTROL Enable edition]**.

1. Tutti i campi che possono essere modificati per il componente selezionato sono elencati nel riquadro. I campi disponibili per la modifica dipendono dal tipo di componente selezionato.

   Nell’esempio seguente, è consentita la modifica dell’URL del pulsante &quot;Fai clic qui&quot;.

   ![](assets/fragment-param-enable.png){width="800" zoomable="yes"}

1. Fare clic su **[!UICONTROL Overview]** per controllare tutti i campi modificabili e i relativi valori predefiniti.

   In questo esempio, il campo URL del pulsante viene visualizzato con il valore predefinito definito nel componente. Questo valore sarà personalizzabile dagli utenti dopo che avranno aggiunto il frammento al loro contenuto.

   ![](assets/fragment-param-preview.png){width="800" zoomable="yes"}

1. Al termine, salva le modifiche.

Dopo aver aggiunto il frammento in un messaggio e-mail, gli utenti potranno personalizzare tutti i campi modificabili configurati nel frammento.
<!--
## Add editable fields in HTML components and expression fragments {#expression}

To make portions of an HTML component or an expression fragment editable, you must use a specific syntax in the expression editor. This involves declaring a _variable_ with a default value that users can override after adding the fragment to their content.

For example, suppose you want to create a fragment to add to your emails, and allow users to customize a specific color used in different locations, such as frames or buttons' background colors. When creating your fragment, you need to declare a variable with a _unique ID_ (e.g., "color"), and call it at the desired locations in the fragment content where you want to apply this color. When adding the fragment to their content, users will be able to customize the color used wherever the variable is referenced.

For HTML components, only specific elements can become editable fields. Expand the section below for more information.

+++Editable elements in HTML components:

The elements below can become editable fields in an HTML component:

* A portion of text
* A full URL for link or image (doesn't work with portion of a URL)
* Entire CSS property (doesn't work with partial property)

For example, in the code below, each element highlighted in red can become a property:

![](assets/fragment-html.png){width="500" zoomable="yes"}

+++
-->
>[!MORELIKETHIS]
>
>[Frammenti](/help/marketo/product-docs/email-marketing/email-designer/fragments.md){target="_blank"}
