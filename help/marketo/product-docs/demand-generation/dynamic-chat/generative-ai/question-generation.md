---
description: Scopri come generare domande per Dynamic Chat utilizzando gli URL e gli argomenti di origine. Crea risposte basate sull’intelligenza artificiale e tieni traccia dello stato delle attività nelle risposte assistite.
title: Generazione della domanda
feature: Dynamic Chat
exl-id: 05e0fd4c-b8e0-47de-8ca8-d4ba07d6a06a
TQID: https://experienceleague.adobe.com/aNb02vSBYXLUd-bGqvbbTB6IXSL6IY-8KCozGeZjZsI
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 307
ht-degree: 4%

---

# Generazione della domanda {#question-generation}

Visualizza tutte le attività e i relativi dettagli pertinenti, ad esempio quando sono state generate, il numero totale di domande, lo stato di approvazione e altro ancora.

## Genera domande {#generate-questions}

1. In IA generativa fare clic su **[!UICONTROL Assisted responses]**.

   ![](assets/question-generation-1.png)

1. Fai clic su **[!UICONTROL Generate questions]**.

   ![](assets/question-generation-2.png)

1. Assegna un nome all’attività e inserisci un URL di origine (fino a 10) dal quale verrà estratto tutto il contenuto. Immettere gli argomenti/parole chiave desiderati e premere Invio sulla tastiera. Al termine, fare clic su **[!UICONTROL Generate]**.

   ![](assets/question-generation-3.png)

   >[!IMPORTANT]
   >
   >Per garantire che Marketo Engage possa raschiare il contenuto dagli URL forniti, devi prima inserire nell&#39;elenco Consentiti diversi indirizzi IP. In questo caso, è necessario che l’utente che ha eseguito l’operazione sia in grado di eseguire l’operazione di raschiamento di un determinato contenuto dagli URL forniti. In questo caso, è necessario innanzitutto  diversi indirizzi IP. [Per ulteriori dettagli, vedere di seguito](#ip-addresses-to-allowlist).

   >[!NOTE]
   >
   >I siti e le pagine devono essere pubblici (ovvero non nascosti dietro un accesso) affinché le loro informazioni possano essere raschiate.

1. In base al contenuto, la generazione di domande e risposte può richiedere fino a 30 minuti. Fai clic su **[!UICONTROL OK]**.

   ![](assets/question-generation-4.png)

   >[!TIP]
   >
   >Premi Aggiorna per visualizzare lo stato più recente della generazione delle domande.

   ![](assets/question-generation-5.png)

## Scaricare domande e risposte {#download-questions-and-responses}

>[!NOTE]
>
>Le domande e le risposte generate sono visualizzabili anche nella [Libreria risposte](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/response-library.md).

1. Trova l’attività desiderata e fai clic sull’icona Scarica accanto al nome.

   ![](assets/question-generation-6.png)

1. Individua la cartella dei download nel browser e seleziona il file. Questo aspetto può variare a seconda del browser utilizzato.

   ![](assets/question-generation-7.png)

1. Nel file di Excel, **[!DNL Task details]** mostra vari dettagli sull&#39;attività, incluse istruzioni su come aggiungere o modificare domande e risposte.

   ![](assets/question-generation-8.png)

   >[!NOTE]
   >
   >Se decidi di aggiungere/modificare domande e/o risposte in blocco, [scopri come ricaricarle qui](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/response-library.md).

1. La scheda **[!DNL Q&Rs]** fornisce ulteriori dettagli, incluse le domande e le risposte generate.

   ![](assets/question-generation-9.png)

## Indirizzi IP da Inserire nell&#39;elenco Consentiti per l accesso {#ip-addresses-to-allowlist}

Per abilitare l’estrazione dei contenuti dagli URL web durante la generazione di domande e risposte, individua la tua area geografica di seguito e verifica che l’indirizzo IP ad esso associato sia inserito nell&#39;elenco Consentiti dal team web.

<table width="450">
<thead>
  <tr>
    <th>America del Nord</th>
    <th>Europa</th>
    <th>APAC</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>13.68.17.252</td>
    <td>20.105.150.224</td>
    <td>20.213.91.77</td>
  </tr>
</tbody>
</table>
