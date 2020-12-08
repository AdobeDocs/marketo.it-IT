---
unique-page-id: 1900554
description: Modificare l'HTML di un'e-mail - Documenti Marketo - Documentazione del prodotto
title: Modificare l’HTML di un messaggio e-mail
translation-type: tm+mt
source-git-commit: 1a29614ec938074902af201b2ffc11cfaa625f7a
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---


# Modificare l’HTML di un messaggio e-mail {#edit-an-emails-html}

A volte può essere necessario modificare l’HTML sottostante di un messaggio e-mail. A volte è possibile utilizzare un sistema esterno per progettare e creare il codice dell&#39;e-mail. In entrambi i casi, potete importare e/o modificare facilmente il codice dall’editor e-mail.

## Modifica HTML {#edit-html}

1. Selezionate il messaggio e-mail e fate clic su **Modifica bozza**.

   ![](assets/teamspidey.jpg)

1. Fate clic su **Modifica codice**.

   ![](assets/two-4.png)

1. Apportate eventuali modifiche. Al termine, fate clic su **Salva** .

   ![](assets/three-3.png)

   >[!NOTE]
   >
   >Cambia quello che vuoi. Potete sostituire l’intero HTML o apportare lievi modifiche.

1. Fate clic sul menu a discesa Azioni **** codice per scaricare il codice come file .html, inline the CSS (Inline the CSS) o validate l&#39;HTML.

   ![](assets/four-2.png)

   >[!NOTE]
   >
   >La procedura ottimale per le e-mail consiste nel rendere online tutti gli stili. Diversi client e-mail non supportano CSS all&#39;interno della `<head>` sezione.

## Interruzione di un’e-mail dal suo modello {#breaking-an-email-from-its-template}

Queste modifiche di codice non **interromperanno** un&#39;e-mail dal relativo modello:

* Modifica dei contenuti di qualsiasi modulo (inclusa l&#39;aggiunta di nuovi elementi all&#39;interno del modulo)
* Aggiunta di un nuovo modulo al contenitore
* Eliminazione di un modulo dal contenitore

* Modifica degli attributi mkto specifici (ad esempio &quot;mktoName&quot; o &quot;mktoImgUrl&quot;) di qualsiasi elemento esterno a un modulo
* Modifica dei contenuti di qualsiasi elemento (RTF, immagine, video, ecc.) all&#39;esterno di un modulo

Queste operazioni possono essere effettuate nell’editor di codice e **interromperanno** l’e-mail dal relativo modello:

* Modifica di elementi nel codice all&#39;esterno di un elemento o modulo
* Aggiunta o modifica di attributi non mkto (ad esempio, &quot;id&quot; o &quot;stile&quot;) di qualsiasi elemento esterno a un modulo
* Eliminazione di un elemento esterno a un modulo

## Codice di ricerca {#search-code}

Utilizzate la funzionalità Cerca codice per trovare e sostituire in modo efficiente il contenuto presente nel codice HTML del messaggio e-mail.

1. Nel codice del messaggio e-mail, fai clic su **Cerca codice**.

   ![](assets/five-2.png)

1. Inserite il testo da trovare e fate clic su **Trova successivo** per cercare in avanti o su **Trova precedente** per eseguire la ricerca all’indietro. È inoltre disponibile l’opzione **Sostituisci** e **Sostituisci tutto**.

   ![](assets/six-1.png)

1. Al termine, fate clic su **Chiudi** .

   ![](assets/seven.png)

   >[!NOTE]
   >
   >Il codice di ricerca è disponibile anche nell’editor [Modello e-](http://docs.marketo.com/display/DOCS/Create+a+New+Email+Template)mail.

È consigliabile continuare a modificare le e-mail utilizzando la funzionalità integrata di Marketo, ma questo editor di codice offre flessibilità se necessario.
