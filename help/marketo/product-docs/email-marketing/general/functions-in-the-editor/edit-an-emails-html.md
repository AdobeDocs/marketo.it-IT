---
unique-page-id: 1900554
description: Modificare il HTML di un’e-mail - Documentazione di Marketo - Documentazione del prodotto
title: Modificare il HTML di un’e-mail
exl-id: 9dc8e44d-d9da-4bc2-950f-3ffbb976f5d5
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---

# Modificare il HTML di un’e-mail {#edit-an-emails-html}

A volte può essere necessario modificare il HTML sottostante di un’e-mail. A volte puoi utilizzare un sistema esterno per progettare e generare il codice dell’e-mail. In entrambi i casi, puoi importare e/o modificare facilmente il codice dall’editor e-mail.

## Modifica HTML {#edit-html}

1. Seleziona l&#39;e-mail e fai clic su **Modifica bozza**.

   ![](assets/teamspidey.jpg)

1. Fare clic su **Modifica codice**.

   ![](assets/two-4.png)

1. Apporta le modifiche necessarie. Al termine, fai clic su **Salva**.

   ![](assets/three-3.png)

   >[!NOTE]
   >
   >Cambia quello che vuoi. È possibile sostituire l&#39;intero HTML o apportare modifiche minori.

1. Fai clic sul menu a discesa **Azioni codice** per scaricare il codice come file .html, allineare il file CSS o convalidare il HTML.

   ![](assets/four-2.png)

   >[!NOTE]
   >
   >La best practice per le e-mail è di allineare tutti gli stili. Diversi client di posta elettronica non supportano CSS nella sezione `<head>`.

## Interruzione di un’e-mail dal relativo modello {#breaking-an-email-from-its-template}

Queste modifiche al codice **non** interrompono un&#39;e-mail dal relativo modello:

* Modifica del contenuto di qualsiasi modulo (inclusa l’aggiunta di nuovi elementi all’interno del modulo)
* Aggiunta di un nuovo modulo al contenitore
* Eliminazione di un modulo dal contenitore

* Modifica degli attributi specifici di mkto (ad esempio, &quot;mktoName&quot; o &quot;mktoImgUrl&quot;) di qualsiasi elemento al di fuori di un modulo
* Modifica del contenuto di qualsiasi elemento (testo formattato, immagine, video, ecc.) all&#39;esterno di un modulo

Le operazioni che è possibile eseguire nell&#39;editor di codice **interromperanno** l&#39;e-mail dal relativo modello:

* Modifica di elementi nel codice all&#39;esterno di un elemento o di un modulo
* Aggiunta o modifica di attributi non mkto (ad esempio, &quot;id&quot; o &quot;style&quot;) di qualsiasi elemento al di fuori di un modulo
* Eliminazione di un elemento esterno a un modulo

## Cerca codice {#search-code}

Utilizza la funzionalità Search Code per trovare e sostituire in modo efficiente il contenuto all’interno del codice HTML dell’e-mail.

1. Nel codice dell&#39;e-mail, fai clic su **Cerca codice**.

   ![](assets/five-2.png)

1. Immetti ciò che desideri trovare e fai clic su **Trova successivo** per cercare in avanti o su **Trova precedente** per cercare all&#39;indietro. Hai anche la possibilità di **Sostituire** e **Sostituire Tutto**.

   ![](assets/six-1.png)

1. Al termine, fai clic su **Chiudi**.

   ![](assets/seven.png)

   >[!NOTE]
   >
   >Il codice di ricerca è disponibile anche nell&#39;[editor modelli e-mail](/help/marketo/product-docs/email-marketing/general/email-editor-2/create-an-email-template.md).

È consigliabile continuare a modificare le e-mail utilizzando la funzionalità integrata di Marketo, ma questo editor di codice offre flessibilità in caso di necessità.
