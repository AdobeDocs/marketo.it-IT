---
unique-page-id: 10096675
description: Creare campagne figlio e risorse locali - Documenti Marketo - Documentazione del prodotto
title: Creare campagne figlio e risorse locali
exl-id: 272105e1-43d6-455c-a533-aae65e859384
source-git-commit: 40cfdddac66b7cd90e33bedf11888a7c5e3b38c9
workflow-type: tm+mt
source-wordcount: '688'
ht-degree: 1%

---

# Creare campagne figlio e risorse locali {#create-child-campaigns-and-local-assets}

>[!IMPORTANT]
>
>A partire da agosto 2022, ON24 non supporta più nuove integrazioni Marketo. Le informazioni contenute in questo articolo si applicano solo agli utenti esistenti.

Crea le tue campagne figlio e risorse locali utilizzando Design Studio.

## Pagina di destinazione e modulo {#landing-page-and-form}

Per garantire che le persone siano registrate correttamente con ON24, nel modulo Marketo devono essere inclusi i campi seguenti:

* Nome
* Cognome
* Indirizzo e-mail

È inoltre possibile inviare i campi seguenti a ON24:

* Nome dell&#39;azienda
* Professione

Con il passaggio di flusso appropriato aggiunto alla campagna di registrazione, le persone verranno inviate su ON24 e contrassegnate come registrate. È possibile aggiungere altri campi al modulo e le informazioni verranno acquisite in Marketo come parte del record di dettaglio della persona.

>[!CAUTION]
>
>Per una corretta integrazione, è necessario utilizzare un modulo Marketo per registrare le persone per l’evento, oppure un modulo non Marketo con l’integrazione API appropriata per inviare i dati di registrazione push a Marketo.

## E-mail e token URL {#emails-and-url-tokens}

Crea l’invito, la conferma, il follow-up e ringrazia le e-mail tramite Marketo.

## E-mail di conferma Marketo e token URL {#marketo-confirmation-email-and-url-token}

Utilizza Marketo per inviare l’e-mail di conferma dell’evento. Quando una persona si registra, riceve un URL univoco da utilizzare per accedere all’evento.

>[!NOTE]
>
>Per popolare l’e-mail di conferma con questo URL univoco, utilizza il seguente token nella tua e-mail: `{{member.webinar url}}`. Quando invii l’URL di conferma, questo token viene automaticamente risolto nell’URL di conferma univoco della persona.
>
>Imposta il tipo di e-mail di conferma su **Operativo** per garantire che le persone che si registrano ricevano le informazioni di conferma, anche se non sono abbonate.

>[!TIP]
>
>Puoi configurare ON24 per inviare e-mail di conferma, promemoria o follow-up. Consulta la sezione [Sito della Guida di ON24](https://www.on24.com/live-webcast-elite/) per ulteriori informazioni.

## Requisiti della campagna figlio di registrazione {#registration-child-campaign-requirements}

Gli eventi contengono una o più campagne figlie che lavorano tutte insieme per spostare le persone tra gli stati del programma e consentono di tenere traccia delle prestazioni dell’evento.

Esempi di campagne figlio sono una campagna di invito, una campagna di registrazione e campagne di follow-up.

>[!CAUTION]
>
>Affinché l&#39;adattatore possa svolgere il suo lavoro, DEVI creare una campagna di registrazione. Questa campagna deve essere attivata dalla persona che compila un modulo e il primo passaggio deve modificare lo stato del programma della persona in **Registrato**. La campagna invia quindi un’e-mail di conferma. Vedi il resto di questo articolo per i dettagli.

**Registrazione/conferma (Trigger Campaign)**

* Elenco avanzato
* Trigger basato su **Riempie il modulo**. Accertati di includere la pagina di destinazione in cui si trova il modulo utilizzando **Aggiungi vincolo**, soprattutto se lo stesso modulo viene utilizzato su più pagine di destinazione.

>[!CAUTION]
>
>È necessario utilizzare un modulo Marketo per registrare le persone per l’evento, o un modulo non Marketo con l’integrazione API corretta per inviare i dati di registrazione push a Marketo. Questo è fondamentale per il successo dell’integrazione con i partner evento.

>[!NOTE]
>
>Se utilizzi un modulo Marketo su una pagina di destinazione non Marketo, il trigger sarà **Riempie il modulo** con il nome del modulo.

![](assets/image2015-12-22-15-3a20-3a51.png)

**Flusso**

* **Cambia stato del programma** - Imposta su Webinar -> Registrato.

Questo passaggio di flusso è necessario come PRIMO PASSAGGIO FLUSSO durante la configurazione della campagna figlio. Quando lo stato del programma di una persona cambia in Registrato, Marketo invia le informazioni di registrazione a ON24. Nessun altro stato invierà la persona.

* **Invia e-mail** - E-mail di conferma. Imposta questo messaggio e-mail su **Operativo** in modo che le persone non abbonate che si sono registrate lo ricevano ancora.

La **Invia e-mail** Il passaggio di flusso DEVE essere il secondo passaggio. L’e-mail di conferma contiene la variabile `{{member.webinar url}}`, che viene popolato con informazioni inviate nuovamente a Marketo da ON24.

![](assets/image2015-12-22-15-3a29-3a50.png)

>[!NOTE]
>
>L’ordine di questi passaggi di flusso è importante a causa dell’ordine in cui le azioni vengono eseguite in Marketo. La **Cambia stato del programma** il passaggio invia la persona a ON24 per registrarsi e viene generato un URL univoco. Dopo che ciò si verifica, puoi inviare l’e-mail di conferma che include questo URL univoco utilizzando `{{member.webinar URL}}` token.
>
>Se la persona viene restituita con un errore di registrazione, non riceverà la conferma via e-mail.

Il passaggio successivo è: [verifica l’integrazione degli eventi ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/test-your-on24-event-integration.md).

>[!MORELIKETHIS]
>
>* [Informazioni sugli eventi dell&#39;adattatore Marketo ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md)
>* [Esempio di integrazione di eventi ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md)
>* [Informazioni sugli stati del programma webinar](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-webinar-program-statuses.md)

