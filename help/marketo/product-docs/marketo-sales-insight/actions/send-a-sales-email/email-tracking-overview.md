---
description: Panoramica sul tracciamento e-mail - Documenti Marketo - Documentazione del prodotto
title: Panoramica sul tracciamento e-mail
hide: true
hidefromtoc: true
exl-id: 89437d22-d739-45ea-8a2e-046a7de80379
source-git-commit: fda1bf51d4016a61c41be9acba4771db1797a552
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# Panoramica sul tracciamento e-mail {#email-tracking-overview}

## Come funziona il tracciamento delle risposte {#how-reply-tracking-works}

Il tracciamento della risposta viene eseguito guardando un ID messaggio presente in ogni e-mail inviata. Ogni e-mail contiene un ID messaggio univoco che ci consente di ottenere uno dei migliori risultati di tracciamento delle risposte.

>[!PREREQUISITES]
>
>Connessione con server e-mail: È necessario collegare la rete di vendita alla Posta in arrivo in modo da sapere quando è arrivata una nuova risposta. Sarà necessario che il tuo account Sales Connect sia collegato a Gmail. Se utilizzi Outlook, sarà necessario eseguire l’integrazione con il server di Exchange.

Se Sales Connect non è in grado di tenere traccia della risposta del potenziale cliente all’e-mail, non sarà in grado di interrompere una campagna in base al rilevamento delle risposte o al registro che risponde a Salesforce. Cosa intendiamo per indirizzo e-mail che può rispondere?

Ciò significa che se invii un’e-mail a flynn@flynnsarcade.com e risponde con kevinf@flynnsarcade.com, saremo in grado di tenere traccia della risposta. Inoltre, se invii un&#39;e-mail a flynn@flynnsarcade.com e CC alan@encom.com e Alan ti scrive di nuovo, rileverà anche la risposta e terminerà la campagna.

## Come tenere traccia degli allegati e-mail {#how-to-track-your-email-attachments}

Sales Connect offre il tracciamento dei tuoi allegati (.doc, .ppt, .pdf) in modo da poter vedere quando sono stati aperti/scaricati e vedere quali pagine il destinatario sta guardando. Ti permetteremo di utilizzare la nostra funzione di allegati tracciabili da entrambi i [applicazione web](https://toutapp.com/login) e Gmail (o app Google).

>[!NOTE]
>
>Il tracciamento degli allegati è disponibile solo per i piani del nostro team (a partire dal nostro piano di avvio g3).

**Come inviare il tuo primo allegato rintracciabile**

1. Componi un messaggio e-mail o modifica un modello, quindi fai clic sul pulsante **Contenuto** pulsante .

1. Carica l&#39;allegato e invialo. Supportiamo PDF, documenti Word e presentazioni Powerpoint.

1. Seleziona **Aggiungi a e-mail**.

1. Fai clic su **Invia** e attiva il tuo Live Feed. Visualizzerai i destinatari quando si aprono e sfogliano gli allegati.

>[!TIP]
>
>Se non desideri tenere traccia di un allegato, fai clic su Allega file e questo allegato non verrà tracciato.

## Come funziona il tracciamento delle viste {#how-view-tracking-works}

Le e-mail vengono tracciate inserendo un’immagine invisibile all’interno delle e-mail inviate.

Se qualcuno risponde alla tua e-mail ma Sales Connect dice che non è stata visualizzata, le probabilità sono che il destinatario non abbia abilitato immagini all&#39;interno del proprio client e-mail (ad esempio, fai clic sul messaggio &quot;fai clic qui per scaricare immagini&quot; nell&#39;e-mail).

Alcuni suggerimenti per migliorare il tracciamento delle statistiche sulle e-mail:

* Includi un’immagine nelle e-mail (come un logo) in modo che il destinatario sia invitato a abilitare le immagini per visualizzare il messaggio.
* Includi un collegamento come chiamata all’azione nell’e-mail.

## E-mail di test non visualizzata come visualizzata {#test-email-not-showed-as-viewed}

Anche se hai inviato il messaggio a un altro indirizzo e-mail, non ti registreremo quando visualizzi le e-mail che hai inviato a te stesso nel feed live. Il nostro tracciamento è basato su dispositivi; se utilizzi un computer con cui hai effettuato l’accesso a Sales Connect, escluderemo tale attività.

La ragione? Sales Connect è intelligente e i nostri utenti attivi non ci perdonerebbero mai se le loro informazioni venissero inserite nell&#39;attività Live Feed ogni volta che guardavano un&#39;e-mail che hanno inviato.
