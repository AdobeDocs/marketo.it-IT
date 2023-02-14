---
unique-page-id: 11378713
description: Attivazione di modifiche agli oggetti personalizzati - Documenti Marketo - Documentazione del prodotto
title: Attiva modifiche a oggetti personalizzati
exl-id: a2a3d82f-33ae-4191-b114-dbbf944a66c8
source-git-commit: 99b11e17e9c2255a19c658b166e7b38c45cf1001
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
>Contattare [Supporto Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) per abilitare i trigger di modifica oggetti personalizzati.

Nell’elenco smart di una campagna intelligente, puoi attivare un’azione di flusso quando un oggetto personalizzato viene aggiunto a una persona o a un’azienda. È inoltre possibile creare un elenco avanzato che utilizzi un *cambiare* in un oggetto personalizzato come attivatore. Ad esempio, utilizzalo per inviare un’e-mail quando il nome di un corso viene aggiornato.

>[!NOTE]
>
>Una voce del registro attività non viene creata quando viene modificato un record oggetto personalizzato.

1. In Marketo, vai a **Attività di marketing.**

   ![](assets/trigger-off-custom-object-changes-1.png)

1. Crea o apri una Smart Campaign esistente e seleziona l’Elenco avanzato.

   ![](assets/trigger-off-custom-object-changes-2.png)

1. Cerca il trigger desiderato e trascinalo sull’area di lavoro.

   ![](assets/trigger-off-custom-object-changes-3.png)

1. Seleziona l’attributo trigger.

   ![](assets/trigger-off-custom-object-changes-4.png)

1. Facoltativamente, impostare un vincolo.

   ![](assets/trigger-off-custom-object-changes-5.png)

1. Ed eccovi qui. La modifica viene salvata automaticamente.

   ![](assets/trigger-off-custom-object-changes-6.png)

   >[!NOTE]
   >
   >* [Creare un elenco avanzato](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)
   >* [Informazioni sugli oggetti personalizzati Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)

