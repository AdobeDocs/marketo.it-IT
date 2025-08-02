---
description: Libreria di risposte - Documentazione di Marketo - Documentazione del prodotto
title: Libreria risposte
feature: Dynamic Chat
exl-id: 774346fa-f633-48e8-a489-999404b6070b
source-git-commit: 26573c20c411208e5a01aa7ec73a97e7208b35d5
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 0%

---

# Libreria risposte {#response-library}

In un&#39;unica posizione, visualizzare tutte le domande, il loro stato di approvazione e i nomi/argomenti delle attività assegnati.

## Aggiungi manualmente una domanda {#manually-add-a-question}

1. In IA generativa fare clic su **[!UICONTROL Assisted responses]**.

   ![](assets/response-library-1.png)

1. Fare clic sulla scheda **[!UICONTROL Response library]**.

   ![](assets/response-library-2.png)

1. Fai clic su **[!UICONTROL Add question]**.

   ![](assets/response-library-3.png)

1. Inserisci la domanda e la risposta. Assegna un argomento e aggiungi un URL facoltativo che gli utenti possono condividere con i visitatori. Al termine, fai clic su **[!UICONTROL Save]**.

   ![](assets/response-library-4.png)

1. Fai clic su Aggiorna e la nuova domanda viene visualizzata nella parte superiore con lo stato di &quot;[!UICONTROL Processing]&quot;.

   ![](assets/response-library-5.png)

1. Dopo alcuni minuti, aggiorna di nuovo e lo stato diventa &quot;Approvato&quot;.

   ![](assets/response-library-6.png)

## Modificare una singola domanda/risposta {#generate-a-new-question}

>[!NOTE]
>
>Per impostazione predefinita, a tutte le domande e risposte generate viene assegnato lo stato &quot;[!UICONTROL need review]&quot;. Solo &quot;[!UICONTROL approved]&quot; domande e risposte sono rese disponibili ai visitatori di chat.

1. In **[!UICONTROL Response library]**, fare clic sulla domanda desiderata.

   ![](assets/response-library-7.png)

1. Apportare le modifiche desiderate e fare clic su **[!UICONTROL Save]**.

   ![](assets/response-library-8.png)

## Modifica e caricamento in blocco di domande/risposte {#bulk-edit-and-upload-questions-responses}

Di seguito sono riportate le istruzioni su come apportare modifiche in blocco nel [file di Excel scaricato](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/question-generation.md#download-questions-and-responses){target="_blank"}. Possono essere visualizzate anche nella scheda Dettagli attività del file.

<table>
<thead>
  <tr>
    <th>Azione</th>
    <th>Istruzioni</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Modificare una domanda</td>
    <td>Immettere la nuova domanda nella colonna "editQuestion" (colonna H)</td>
  </tr>
  <tr>
    <td>Modificare una risposta</td>
    <td>Immettere la nuova risposta nella colonna "editResponse" (colonna I)</td>
  </tr>
  <tr>
    <td>Aggiungi una nuova domanda</td>
    <td>Immettere la nuova domanda nella colonna "editQuestion" (colonna H) e lasciare il campo questionResponse vuoto. È inoltre necessario immettere un argomento appropriato nella colonna "topic" (colonna C) e un URL di origine nella colonna "sourceUr!"</td>
  </tr>
  <tr>
    <td>Aggiungi una domanda e una risposta</td>
    <td>Immettere la nuova domanda nella colonna "editQuestion" (colonna H), la nuova risposta nella colonna "editResponse" (colonna I) e lasciare il campo questionResponseld vuoto. È inoltre necessario immettere un argomento appropriato nella colonna "topic" (colonna C)</td>
  </tr>
</tbody>
</table>

1. Dopo aver apportato le modifiche nel file, torna alla scheda **[!UICONTROL Response library]** e fai clic su **[!UICONTROL Upload responses]**.

   ![](assets/response-library-9.png)

1. Immettere il nome dell&#39;attività applicabile. Trascina e rilascia il file o cercalo sul dispositivo e selezionalo. Al termine, fai clic su **[!UICONTROL Save]**.

   ![](assets/response-library-10.png)

1. Viene visualizzata la conferma e tutto è pronto.

   ![](assets/response-library-11.png)

## Filtra le domande {#filter-your-questions}

Per impostazione predefinita, le domande sono elencate in ordine per ora/data di creazione, con quelle più recenti visualizzate per prime. Se stai cercando una domanda specifica, applica dei filtri per restringere la ricerca. Filtra per argomenti, nome dell&#39;attività e/o stato di approvazione.

![](assets/response-library-12.png)
