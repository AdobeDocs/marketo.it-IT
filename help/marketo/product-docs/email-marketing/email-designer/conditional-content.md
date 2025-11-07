---
solution: Marketo Engage
product: marketo
title: Contenuto condizionale
description: Utilizza il contenuto condizionale nelle e-mail per visualizzare in modo dinamico il contenuto in base al destinatario.
level: Beginner, Intermediate
feature: Email Designer
source-git-commit: 6b9f6d4b276115e1f3f3dac73eb64e5358a76516
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 2%

---

# Contenuto condizionale {#conditional-content}

Il contenuto condizionale consente di controllare dinamicamente il contenuto visualizzato da ciascun pubblico. Utilizza le segmentazioni esistenti per determinare cosa vede un destinatario in base a criteri predefiniti.

>[!PREREQUISITES]
>
>Avere almeno una segmentazione [creata](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/create-a-segmentation.md) e [approvata](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/approve-a-segmentation.md).

## Aggiungere contenuto condizionale {#add-conditional-content}

1. Apri l&#39;e-mail desiderata e fai clic su **Modifica contenuto e-mail**.

   ![](assets/conditional-content-1.png)

1. Seleziona il contenuto da rendere condizionale (in questo esempio, stiamo scegliendo l’immagine dell’intestazione). Fare clic sull&#39;icona _Abilita contenuto condizionale_.

   ![](assets/conditional-content-2.png)

1. La casella di evidenziazione diventa arancione. A sinistra, fai clic sull&#39;icona _Seleziona condizione_ (![](assets/icon-select-condition.png)) per definire la variante.

   ![](assets/conditional-content-3.png){width="700" zoomable="yes"}

1. Scegli il segmento desiderato e fai clic su **Seleziona**.

   ![](assets/conditional-content-4.png)

1. Fai clic sull&#39;icona _Modifica immagine_ per sostituire l&#39;immagine esistente per la variante. Scegli l&#39;origine della nuova immagine. In questo esempio, stiamo scegliendo la libreria _Immagini e file_ nella sottoscrizione Marketo Engage.

   ![](assets/conditional-content-5.png)

1. Scegli l&#39;immagine applicabile e fai clic su **Seleziona**.

   ![](assets/conditional-content-6.png){width="600" zoomable="yes"}

1. Viene visualizzata la nuova immagine. È consigliabile rinominare la variante per facilitarne l’identificazione. Fai clic sui puntini di sospensione e seleziona **Rinomina**.

   >[!NOTE]
   >
   >Fai clic sui puntini di sospensione per visualizzare anche la condizione definita della variante e duplicarla. Se disponi di più varianti, diventa disponibile un’opzione di eliminazione. Se disponi di una sola variante, il modo per eliminarla consiste nel fare nuovamente clic sull&#39;icona _Abilita contenuto condizionale_ (ora al passaggio del mouse sull&#39;icona _Disabilita contenuto condizionale_).

   ![](assets/conditional-content-7.png){width="600" zoomable="yes"}

1. Per aggiungere altre varianti (facoltativo), fai clic su **Aggiungi variante** e segui gli stessi passaggi.

   ![](assets/conditional-content-8.png)

1. Al termine, ogni variante visualizza il contenuto selezionato.

   ![](assets/conditional-content-9.gif)

1. I destinatari visualizzano il contenuto in base alle regole definite in ciascun segmento. Nell&#39;esempio precedente, tutti coloro che hanno il &quot;calcio&quot; elencato nel campo Marketo Engage _Sport preferito_ vedranno l&#39;immagine del calcio.

>[!MORELIKETHIS]
>
>* [Definisci regole segmento](/help/marketo/product-docs/personalization/segmentation-and-snippets/segmentation/define-segment-rules.md)
>* [Crea un campo personalizzato in Marketo](/help/marketo/product-docs/administration/field-management/create-a-custom-field-in-marketo.md)
