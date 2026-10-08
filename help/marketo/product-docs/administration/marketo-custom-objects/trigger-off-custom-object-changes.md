---
unique-page-id: 11378713
description: Come utilizzare i trigger di aggiunta o modifica di oggetti personalizzati in un elenco smart campaign per gli oggetti personalizzati di Marketo, con passaggi per aggiungere il trigger e impostare i vincoli.
title: Disattivare le modifiche all’oggetto personalizzato
exl-id: a2a3d82f-33ae-4191-b114-dbbf944a66c8
feature: Custom Objects
TQID: 'https://experienceleague.adobe.com/KjZuM-gPLIFa1umPF4pzN2OTak51i9I5TUcC7SacmZ8'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: d1d0a9cd-295d-4976-8c39-ddae266f240e
    internal-label: Administration
  - id: b3b8a63f-51fc-40f6-a7d2-a31c5d49fb45
    internal-label: Configuration
subfeature_v2:
  - id: ea4e3ff5-e7b9-4b4c-a5a0-dc27cc3f4275
    internal-label: Custom objects
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 9%
---
# Disattivare le modifiche all’oggetto personalizzato {#trigger-off-custom-object-changes}

>[!NOTE]
>
>Questa funzione è disponibile solo:
>
>* Da utilizzare solo con oggetti personalizzati di Marketo, non con oggetti personalizzati sincronizzati tramite l&#39;integrazione nativa di [!DNL Salesforce] o [!DNL Microsoft Dynamics]
>
>* Come attivatore, non come filtro
>
>Contattare il [Supporto Marketo](https://nation.marketo.com/t5/support/ct-p/Support) per attivare i trigger di modifica oggetti personalizzati.

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

1. La modifica viene salvata automaticamente.

   ![](assets/trigger-off-custom-object-changes-6.png)

   >[!NOTE]
   >
   >* [Creare un elenco avanzato](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)
   >* [Informazioni sugli oggetti personalizzati di Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)
