---
unique-page-id: 11378713
description: Attivazione di modifiche agli oggetti personalizzati - Documenti Marketo - Documentazione del prodotto
title: Attiva modifiche a oggetti personalizzati
exl-id: a2a3d82f-33ae-4191-b114-dbbf944a66c8
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 0%

---

# Attiva modifiche a oggetti personalizzati {#trigger-off-custom-object-changes}

>[!NOTE]
>
>Questa funzione è disponibile solo:
>
>* Per i clienti dell&#39;infrastruttura Orion
>* Da utilizzare solo con oggetti personalizzati Marketo, non con oggetti personalizzati sincronizzati tramite l’integrazione nativa Salesforce o Microsoft Dynamics
>* Come attivatore, non come filtro

>
>
Contatta il [Supporto Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) per abilitare i trigger di modifica degli oggetti personalizzati.

Nell’elenco smart di una campagna intelligente, puoi attivare un’azione di flusso quando un oggetto personalizzato viene aggiunto a una persona o a un’azienda. È inoltre possibile creare un elenco smart che utilizza come attivatore una *modifica* in un oggetto personalizzato. Ad esempio, utilizzalo per inviare un’e-mail quando il nome di un corso viene aggiornato.

>[!NOTE]
>
>Una voce del registro attività non viene creata quando viene modificato un record oggetto personalizzato.

1. In Marketo, vai a **Attività di marketing.**

   ![](assets/image2016-7-25-15-3a49-3a52.png)

1. Crea o apri una Smart Campaign esistente e seleziona l’Elenco avanzato.

   ![](assets/image2016-7-25-16-3a9-3a19.png)

1. Cerca il trigger desiderato e trascinalo sull’area di lavoro.

   ![](assets/image2016-7-25-16-3a16-3a43.png)

1. Seleziona l’attributo trigger.

   ![](assets/image2016-7-25-16-3a21-3a42.png)

1. Facoltativamente, impostare un vincolo.

   ![](assets/image2016-9-6-14-3a25-3a22.png)

1. Ed eccovi qui. La modifica viene salvata automaticamente.

   ![](assets/image2016-9-6-14-3a25-3a54.png)

   >[!NOTE]
   >
   >* [Creare un elenco avanzato](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)
   >* [Informazioni sugli oggetti personalizzati Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)

