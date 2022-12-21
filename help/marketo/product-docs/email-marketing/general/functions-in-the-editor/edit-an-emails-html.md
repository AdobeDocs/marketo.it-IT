---
unique-page-id: 1900554
description: Modificare un HTML di un’e-mail - Documenti Marketo - Documentazione del prodotto
title: Modificare un HTML di e-mail
exl-id: 9dc8e44d-d9da-4bc2-950f-3ffbb976f5d5
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---

# Modificare un HTML di e-mail {#edit-an-emails-html}

A volte può essere necessario modificare il HTML sottostante di un’e-mail. A volte puoi utilizzare un sistema esterno per progettare e creare il codice della tua e-mail. In entrambi i casi, puoi importare e/o modificare facilmente il codice dall’editor e-mail.

## Modifica HTML {#edit-html}

1. Seleziona l’e-mail e fai clic su **Modifica bozza**.

   ![](assets/teamspidey.jpg)

1. Fai clic su **Modifica codice**.

   ![](assets/two-4.png)

1. Apporta eventuali modifiche. Fai clic su **Salva** al termine.

   ![](assets/three-3.png)

   >[!NOTE]
   >
   >Cambia quello che vuoi. È possibile sostituire l’intero HTML o apportare modifiche minori.

1. Fai clic sul pulsante **Azioni codice** elenco a discesa per scaricare il codice come file .html, inline your CSS o convalidare HTML.

   ![](assets/four-2.png)

   >[!NOTE]
   >
   >La best practice per le e-mail è quella di rendere inline tutti gli stili. Diversi client e-mail non supportano CSS all’interno di `<head>` sezione .

## Interruzione di un’e-mail dal relativo modello {#breaking-an-email-from-its-template}

Queste modifiche al codice **non** interrompi un’e-mail dal relativo modello:

* Modifica del contenuto di qualsiasi modulo (inclusa l’aggiunta di nuovi elementi all’interno del modulo)
* Aggiunta di un nuovo modulo al contenitore
* Eliminazione di un modulo dal contenitore

* Modifica degli attributi specifici di mkto (ad esempio, &quot;mktoName&quot; o &quot;mktoImgUrl&quot;) di qualsiasi elemento al di fuori di un modulo
* Modifica del contenuto di qualsiasi elemento (testo RTF, immagine, video, ecc.) fuori da un modulo

Queste operazioni possono essere eseguite nell&#39;editor di codice **sarà** interrompi l’e-mail dal relativo modello:

* Modifica di qualsiasi elemento nel codice all’esterno di un elemento o modulo
* Aggiunta o modifica di attributi non mkto (ad esempio, &quot;id&quot; o &quot;style&quot;) di qualsiasi elemento al di fuori di un modulo
* Eliminazione di un elemento esterno a un modulo

## Codice di ricerca {#search-code}

Utilizza la funzionalità Cerca codice per trovare e sostituire in modo efficiente il contenuto all’interno del codice HTML dell’e-mail.

1. Nel codice dell’e-mail, fai clic su **Codice di ricerca**.

   ![](assets/five-2.png)

1. Inserisci gli elementi da trovare e fai clic su **Trova successivo** per cercare in avanti o **Trova precedente** per cercare all&#39;indietro. Hai anche la possibilità di **Sostituisci** e **Sostituisci tutto**.

   ![](assets/six-1.png)

1. Fai clic su **Chiudi** al termine.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >Il codice di ricerca è disponibile anche nel [Editor modelli e-mail](/help/marketo/product-docs/email-marketing/general/email-editor-2/create-an-email-template.md).

È consigliabile continuare a modificare le e-mail utilizzando la funzionalità integrata di Marketo, ma questo editor di codice offre flessibilità se necessario.
