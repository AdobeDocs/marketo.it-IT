---
unique-page-id: 11378713
description: Attivare Le Modifiche Agli Oggetti Personalizzati - Documentazione Di Marketo - Documentazione Del Prodotto
title: Disattivare le modifiche all’oggetto personalizzato
exl-id: a2a3d82f-33ae-4191-b114-dbbf944a66c8
feature: Custom Objects
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '179'
ht-degree: 6%

---

# Disattivare le modifiche all’oggetto personalizzato {#trigger-off-custom-object-changes}

>[!NOTE]
>
>Questa funzione è disponibile solo:
>
>* Da utilizzare solo con oggetti personalizzati di Marketo, non con oggetti personalizzati sincronizzati tramite l&#39;integrazione nativa di [!DNL Salesforce] o [!DNL Microsoft Dynamics]
>* Come attivatore, non come filtro
>
>Contatta il [Supporto Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) per richiedere l&#39;abilitazione dei trigger di modifica degli oggetti personalizzati.

Nell’elenco avanzato di una campagna avanzata, puoi attivare un’azione di flusso quando un oggetto personalizzato viene aggiunto a una persona o a un’azienda. Puoi anche creare un elenco avanzato che utilizza come attivatore una _modifica_ in un oggetto personalizzato. Ad esempio, utilizzalo per inviare un’e-mail quando il nome di un corso viene aggiornato.

>[!NOTE]
>
>Una voce del registro attività non viene creata quando viene modificato un record oggetto personalizzato.

1. In Marketo Engage, vai a **[!UICONTROL Marketing Activities]**.

   ![](assets/trigger-off-custom-object-changes-1.png)

1. Crea o apri una campagna avanzata esistente e seleziona l’elenco avanzato.

   ![](assets/trigger-off-custom-object-changes-2.png)

1. Cerca il trigger necessario e trascinalo sull’area di lavoro.

   ![](assets/trigger-off-custom-object-changes-3.png)

1. Seleziona [!UICONTROL trigger attribute].

   ![](assets/trigger-off-custom-object-changes-4.png)

1. È possibile impostare un vincolo.

   ![](assets/trigger-off-custom-object-changes-5.png)

1. Ed eccoti qui. La modifica viene salvata automaticamente.

   ![](assets/trigger-off-custom-object-changes-6.png)

   >[!NOTE]
   >
   >* [Creare un elenco avanzato](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)
   >* [Informazioni sugli oggetti personalizzati di Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
