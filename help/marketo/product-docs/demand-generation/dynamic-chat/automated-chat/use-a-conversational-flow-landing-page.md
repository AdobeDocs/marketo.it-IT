---
description: Utilizzare una pagina di destinazione per il flusso conversazionale - Documentazione di Marketo - Documentazione del prodotto
title: Utilizzare una pagina di destinazione del flusso per conversazioni
hide: true
hidefromtoc: true
feature: Dynamic Chat
source-git-commit: 5ef17e8c3988706a4d95332312ffb035f35bb269
workflow-type: tm+mt
source-wordcount: '226'
ht-degree: 0%

---

# Utilizzare una pagina di destinazione del flusso per conversazioni{#use-a-conversational-flow-landing-page}

L’incorporazione di un flusso conversazionale di Dynamic Chat direttamente in una pagina di destinazione del Marketo Engage consente ai visitatori di pianificare una riunione attraverso il Dynamic Chat senza dover compilare un modulo o interagire con un chatbot.

>[!PREREQUISITES]
>
>Creare un semplice [Flusso conversazionale](/help/marketo/product-docs/demand-generation/dynamic-chat/automated-chat/create-a-conversational-flow.md) che contiene solo un **Prenotazione riunione** Card.

## Pagine di destinazione guidate {#guided-landing-pages}

Incorpora il seguente codice nel modello di pagina di destinazione guidata: `<div class="mktoConversation" id="exampleConversation" mktoName= "Example Conversation"></div>`.

Apri il modello Pagina di destinazione guidata nell’editor e seleziona il segnaposto Flusso conversazionale.

Fare clic sull&#39;elenco a discesa Flusso conversazionale e selezionare il CF creato nel passo 1.

Mantieni sempre tipo di consegna come **In linea**. Clic **Inserisci**.

Il flusso conversazionale appena immesso verrà visualizzato come elemento a destra.

SCHERMATA

>[!NOTE]
>
>In questo momento, il flusso conversazionale non viene visualizzato nella finestra di anteprima principale.

## Pagine di destinazione in formato libero {#free-form-landing-pages}

Testo


NOTE DA STEVE MEETING

lp guidato, nuovo id div per modello, scegli flusso conv

freeform lp, icona porta - attenzione: aggiungi nota - quando inserisci cf nell’editor, non viene visualizzata un’anteprima (nemmeno un segnaposto) - &quot;non visualizzerai un’anteprima&quot; - nella barra laterale viene visualizzato che cf si trova nella pagina - il pl guidato lo elenca come elemento - usa &quot;in questo momento&quot; per spiegare - la funzione va in onda forse settimana del 22°

