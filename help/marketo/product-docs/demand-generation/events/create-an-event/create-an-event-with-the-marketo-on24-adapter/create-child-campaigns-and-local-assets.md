---
unique-page-id: 10096675
description: Creazione di campagne figlio e risorse locali - Documenti Marketo - Documentazione prodotto
title: Creare campagne figlio e risorse locali
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---


# Crea campagne figlio e risorse locali {#create-child-campaigns-and-local-assets}

Create le campagne figlio e le risorse locali utilizzando Design Studio.

## Pagina di destinazione e modulo {#landing-page-and-form}

Per garantire che le persone siano registrate correttamente con ON24, nel modulo Marketo devono essere inclusi i seguenti campi:

* Nome
* Cognome
* Indirizzo e-mail

È inoltre possibile inviare i campi seguenti a ON24:

* Nome società
* Titolo processo

Con il passaggio di flusso corretto aggiunto alla campagna di registrazione, le persone verranno spinti su ON24 e contrassegnati come registrati. È possibile aggiungere altri campi al modulo e le informazioni verranno acquisite in Marketo come parte del record di dettagli delle persone.

>[!CAUTION]
>
>Per una corretta integrazione, è necessario utilizzare un modulo Marketo per registrare le persone per l&#39;evento, oppure un modulo non Marketo con l&#39;integrazione API corretta per inviare i dati di registrazione a Marketo.

## E-mail e token URL {#emails-and-url-tokens}

Crea l&#39;invito, la conferma, il follow-up e le e-mail di ringraziamento tramite Marketo.

## E-mail di conferma di Marketo e token URL {#marketo-confirmation-email-and-url-token}

Utilizzate Marketo per inviare l&#39;e-mail di conferma dell&#39;evento. Quando una persona si registra, riceve un URL univoco da utilizzare per partecipare all&#39;evento.

>[!NOTE]
>
>**Promemoria**
>
>Per compilare il messaggio e-mail di conferma con questo URL univoco, utilizzate il seguente token nel messaggio e-mail: `{{member.webinar url}}`. Quando inviate l’URL di conferma, questo token viene automaticamente risolto nell’URL di conferma univoco della persona.
>
>Impostate il tipo di messaggio e-mail di conferma su **Operativo** per assicurare che le persone che si sono registrate ricevano le informazioni di conferma, anche se non sono state sottoscritte.

>[!TIP]
>
>Puoi configurare ON24 per inviare messaggi di conferma, promemoria o e-mail di follow-up. Per ulteriori informazioni, vedere il [sito della Guida di ON24](http://webcastelitehelp.on24.com).

## Requisiti della campagna figlio di registrazione {#registration-child-campaign-requirements}

Gli eventi contengono una o più campagne figlie che lavorano tutte insieme per spostare le persone attraverso gli stati del programma e consentono di monitorare le prestazioni dell&#39;evento.

Esempi di campagne figlio sono una campagna di inviti, una campagna di registrazione e campagne di follow-up.

>[!CAUTION]
>
>Affinché l&#39;adattatore possa svolgere il proprio lavoro, dovete creare una campagna di registrazione. Questa campagna deve essere attivata dalla persona che compila il modulo e il primo passaggio deve modificare lo stato del programma della persona in **Registered**. La campagna invia quindi un messaggio e-mail di conferma. Consultate il resto di questo articolo per i dettagli.

**Registrazione/conferma (Trigger Campaign)**

* Smart List
* Trigger basato su **Riempie il modulo**. Assicurarsi di includere la pagina di destinazione su cui si trova il modulo utilizzando **Aggiungi vincolo**, soprattutto se lo stesso modulo è utilizzato su più pagine di destinazione.

>[!CAUTION]
>
>È necessario utilizzare un modulo Marketo per registrare le persone per l&#39;evento, oppure un modulo non Marketo con l&#39;integrazione API appropriata per inviare i dati di registrazione push a Marketo. Ciò è fondamentale per il successo dell’integrazione del partner evento.

>[!NOTE]
>
>Se si utilizza un modulo Marketo su una pagina di destinazione non Marketo, l&#39;attivatore sarà **Compilare il modulo** con il nome del modulo.

![](assets/image2015-12-22-15-3a20-3a51.png)

**Flusso**

* **Modifica stato**  programma - Impostato su Webinar -> Registrato.

Questo passaggio di flusso è richiesto come FIRST FLOW STEP (PASSAGGIO FLUSSO PRIMO) durante la configurazione della campagna figlio. Quando lo stato del programma di una persona cambia in Registrato, Marketo invia le informazioni di registrazione a ON24. Nessun altro stato farà passare la persona.

* **Invia e-mail**  - E-mail di conferma. Impostate questo messaggio e-mail su **Operativo** in modo che gli utenti non iscritti che si sono registrati lo ricevano comunque.

Il passaggio di flusso **Invia e-mail** DEVE essere il secondo passaggio. L&#39;e-mail di conferma contiene la `{{member.webinar url}}`, che viene compilata con le informazioni inviate a Marketo da ON24.

![](assets/image2015-12-22-15-3a29-3a50.png)

>[!NOTE]
>
>L&#39;ordine di questi passaggi di flusso è importante a causa dell&#39;ordine in cui vengono eseguite le azioni in Marketo. Il passaggio **Modifica stato programma** invia la persona a ON24 per registrarsi e viene generato un URL univoco. In seguito, potete inviare l&#39;e-mail di conferma che include questo URL univoco utilizzando il token `{{member.webinar URL}}`.
>
>Se la persona viene restituita con un errore di registrazione, non riceverà la conferma e-mail.

Il passaggio successivo è [verificare l&#39;integrazione degli eventi ON24](test-your-on24-event-integration.md).

>[!MORELIKETHIS]
>
>* [Informazioni sugli eventi dell&#39;adattatore Marketo ON24](understanding-marketo-on24-adapter-events.md)
>* [Esempio di integrazione evento ON24](example-on24-event-integration.md)
>* [Informazioni sugli stati del programma webinar](understanding-webinar-program-statuses.md)
>* [Verificare l&#39;integrazione degli eventi ON24](test-your-on24-event-integration.md)

>



