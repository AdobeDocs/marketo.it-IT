---
description: Generazione di domande - Documentazione di Marketo - Documentazione del prodotto
title: Generazione di domande
feature: Dynamic Chat
exl-id: 05e0fd4c-b8e0-47de-8ca8-d4ba07d6a06a
source-git-commit: 6bdac72f0b9831ba830d842cabffbd0f114325fb
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%

---

# Generazione di domande {#question-generation}

Visualizza tutte le attività e i relativi dettagli pertinenti, ad esempio quando sono state generate, il numero totale di domande, lo stato di approvazione e altro ancora.

## Genera domande {#generate-questions}

1. In IA generativa, fai clic su **[!UICONTROL Risposte assistite]**.

   ![](assets/question-generation-1.png)

1. Clic **[!UICONTROL Genera domande]**.

   ![](assets/question-generation-2.png)

1. Assegna un nome all’attività e inserisci un URL di origine (fino a 10) dal quale verrà estratto tutto il contenuto. Immettere gli argomenti/parole chiave desiderati e premere Invio sulla tastiera. Al termine, fai clic su **[!UICONTROL Genera]**.

   ![](assets/question-generation-3.png)

   >[!IMPORTANT]
   >
   >Affinché il Marketo Engage possa raschiare il contenuto dagli URL forniti, devi prima inserire nell&#39;elenco Consentiti alcuni indirizzi IP. Per evitare che il contenuto venga rimosso dagli URL forniti, devi prima diversi indirizzi IP. [Per ulteriori informazioni, consulta di seguito](#ip-addresses-to-allowlist).

1. In base al contenuto, la generazione di domande e risposte può richiedere fino a 30 minuti. Clic **[!UICONTROL OK]**.

   ![](assets/question-generation-4.png)

   >[!TIP]
   >
   >Premi Aggiorna per visualizzare lo stato più recente della generazione delle domande.

   ![](assets/question-generation-5.png)

## Scaricare domande e risposte {#download-questions-and-responses}

>[!NOTE]
>
>Le domande e le risposte generate sono visualizzabili anche in [Libreria di risposte](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/response-library.md).

1. Trova l’attività desiderata e fai clic sull’icona Scarica accanto al nome.

   ![](assets/question-generation-6.png)

1. Individua la cartella dei download nel browser e seleziona il file. Questo aspetto può variare a seconda del browser utilizzato.

   ![](assets/question-generation-7.png)

1. Nel file di Excel, **[!DNL Task details]** mostra solo questo, vari dettagli sull’attività, comprese istruzioni su come aggiungere/modificare domande e/o risposte.

   ![](assets/question-generation-8.png)

   >[!NOTE]
   >
   >Se decidi di aggiungere/modificare domande e/o risposte in blocco, [scopri come ricaricarli qui](/help/marketo/product-docs/demand-generation/dynamic-chat/generative-ai/response-library.md).

1. Il **[!DNL Q&Rs]** fornisce ulteriori dettagli, incluse le domande e le risposte generate.

   ![](assets/question-generation-9.png)

## Indirizzi IP da Inserire nell&#39;elenco Consentiti per l accesso {#ip-addresses-to-allowlist}

Per abilitare l’estrazione dei contenuti dagli URL web durante la generazione di domande e risposte, individua la tua regione di seguito e assicurati che l’indirizzo IP associato sia inserito nell&#39;elenco Consentiti dal team web.

<table width="450">
<thead>
  <tr>
    <th>Nord America</th>
    <th>Europa</th>
    <th>APAC</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>13 68 17 252</td>
    <td>20 105 150 224</td>
    <td>20 213 91 77</td>
  </tr>
</tbody>
</table>
