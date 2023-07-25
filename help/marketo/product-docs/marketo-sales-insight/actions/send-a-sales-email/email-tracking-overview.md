---
description: Panoramica sul tracciamento e-mail - Documentazione di Marketo - Documentazione del prodotto
title: Panoramica del tracciamento e-mail
exl-id: 89437d22-d739-45ea-8a2e-046a7de80379
feature: Sales Insight Actions
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# Panoramica del tracciamento e-mail {#email-tracking-overview}

## Funzionamento del tracciamento delle risposte {#how-reply-tracking-works}

Il tracciamento delle risposte viene eseguito osservando un ID messaggio presente in ogni e-mail inviata. Ogni e-mail contiene un ID messaggio univoco che ci consente di avere alcuni dei migliori tracciamenti delle risposte in giro.

>[!PREREQUISITES]
>
>Connessione al server e-mail: Sales Connect deve essere collegato alla tua casella in entrata in modo da sapere quando è arrivata una nuova risposta. È necessario che l&#39;account Sales Connect sia connesso a Gmail. Se utilizzi Outlook, dovremo eseguire l’integrazione con il server di Exchange.

Se Sales Connect non riesce a tenere traccia della risposta del potenziale cliente all’e-mail, non potrà interrompere una campagna basata sul rilevamento delle risposte o registrare la risposta a Salesforce. Cosa significa che un indirizzo e-mail può rispondere?

Ciò significa che se invii un’e-mail a flynn@flynnsarcade.com e lui risponde con kevinf@flynnsarcade.com, saremo in grado di tenere traccia della risposta. Inoltre, se invii un’e-mail a flynn@flynnsarcade.com e CC alan@encom.com e Alan ti risponde, la risposta verrà rilevata e la campagna verrà terminata.

## Come tenere traccia degli allegati e-mail {#how-to-track-your-email-attachments}

Sales Connect offre il tracciamento degli allegati (.doc, .ppt, .pdf) per consentirti di vedere quando sono stati aperti/scaricati e vedere quali pagine sta cercando il destinatario. È possibile utilizzare la funzionalità degli allegati tracciabili di entrambi [applicazione web](https://toutapp.com/login) e Gmail (o Google Apps).

>[!NOTE]
>
>Il tracciamento degli allegati è disponibile solo per i piani del team (a partire dal piano di avvio g3startup).

**Come inviare il primo allegato tracciabile**

1. Componi un messaggio e-mail o modifichi un modello, quindi fai clic su **Contenuto** pulsante.

1. Carica l’allegato e invialo. Supportiamo PDF, documenti Word e presentazioni Powerpoint.

1. Seleziona **Aggiungi a e-mail**.

1. Clic **Invia** e accendi il tuo feed live. Potrai visualizzare i destinatari all’apertura e scorrere la pagina tra gli allegati.

>[!TIP]
>
>Se non si desidera tenere traccia di un allegato, è sufficiente fare clic su Allega file per non tenere traccia dell&#39;allegato.

## Funzionamento del tracciamento delle visualizzazioni {#how-view-tracking-works}

Tieni traccia delle aperture delle e-mail inserendo un’immagine invisibile all’interno delle e-mail inviate.

Se qualcuno risponde alla tua e-mail ma Sales Connect dice che non è stata visualizzata, è probabile che il destinatario non abbia abilitato le immagini all’interno del proprio client e-mail (ad esempio, fai clic sul messaggio &quot;fai clic qui per scaricare le immagini&quot; nell’e-mail).

Alcuni suggerimenti per ottenere statistiche di tracciamento migliori sulle e-mail:

* Includi un’immagine nelle e-mail (come un logo) in modo che il destinatario sia invitato a consentire alle immagini di visualizzare il messaggio.
* Includi un collegamento come invito all’azione nell’e-mail.

## E-mail di prova non visualizzata {#test-email-not-showed-as-viewed}

Anche se hai inviato il messaggio a un altro indirizzo e-mail, non ti registreremo visualizzando le e-mail che ti sei inviato nel feed live. Il tracciamento è basato su dispositivi; finché utilizzi un computer con cui hai effettuato l’accesso a Sales Connect, questa attività verrà filtrata.

Il motivo? Sales Connect è intelligente, e i nostri utenti attivi non ci perdonerebbero mai se le loro informazioni comparissero nell&#39;attività Live Feed ogni volta che guardavano un&#39;e-mail inviata.
