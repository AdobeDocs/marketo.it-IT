---
unique-page-id: 11378713
description: Attivazione Delle Modifiche Degli Oggetti Personalizzati - Documenti Marketo - Documentazione Del Prodotto
title: Attiva modifiche a oggetti personalizzati
translation-type: tm+mt
source-git-commit: f865630638e7c0fe6ac2a449e196a7de4fbfeea1
workflow-type: tm+mt
source-wordcount: '196'
ht-degree: 0%

---


# Attivazione delle modifiche dell&#39;oggetto personalizzato {#trigger-off-custom-object-changes}

>[!NOTE]
>
>Questa funzione è disponibile solo:
>
>* Per i clienti dell&#39;infrastruttura Orion
>* Da utilizzare solo con oggetti personalizzati Marketo, non con oggetti personalizzati sincronizzati tramite l&#39;integrazione nativa di Salesforce o Microsoft Dynamics
>* Come trigger, non come filtro

>
>
Contattare il supporto [Marketo](https://nation.marketo.com/t5/Support/ct-p/Support) per avere attivati attivatori di modifica oggetti personalizzati.

Nell&#39;elenco smart di una campagna, puoi attivare un&#39;azione di flusso quando un oggetto personalizzato viene aggiunto a una persona o una società. È inoltre possibile creare un elenco smart che utilizza come trigger *change* in un oggetto personalizzato. Ad esempio, utilizzatelo per inviare un messaggio e-mail quando il nome di un corso viene aggiornato.

>[!NOTE]
>
>Una voce del registro attività non viene creata quando viene modificato un record oggetto personalizzato.

1. In Marketo, passare a **Attività di marketing.**

   ![](assets/image2016-7-25-15-3a49-3a52.png)

1. Create o aprite una Smart Campaign esistente e selezionate l&#39;Elenco avanzato.

   ![](assets/image2016-7-25-16-3a9-3a19.png)

1. Cercare il trigger desiderato e trascinarlo sul quadro.

   ![](assets/image2016-7-25-16-3a16-3a43.png)

1. Selezionare l&#39;attributo di attivazione.

   ![](assets/image2016-7-25-16-3a21-3a42.png)

1. Facoltativamente, impostare un vincolo.

   ![](assets/image2016-9-6-14-3a25-3a22.png)

1. Ed eccoci qui. La modifica viene salvata automaticamente.

   ![](assets/image2016-9-6-14-3a25-3a54.png)

   >[!NOTE]
   >
   >* [Creare un elenco avanzato](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/create-a-smart-list.md)
   >* [Informazioni sugli oggetti personalizzati Marketo](/help/marketo/product-docs/administration/marketo-custom-objects/understanding-marketo-custom-objects.md)

