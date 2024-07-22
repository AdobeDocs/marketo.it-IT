---
unique-page-id: 10096675
description: Creazione di campagne secondarie e Assets locale - Documentazione di Marketo - Documentazione del prodotto
title: Creazione di campagne secondarie e Assets locale
exl-id: 272105e1-43d6-455c-a533-aae65e859384
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '665'
ht-degree: 1%

---

# Creazione di campagne secondarie e Assets locale {#create-child-campaigns-and-local-assets}

Crea le campagne secondarie e le risorse locali utilizzando Design Studio.

## Pagina di destinazione e modulo {#landing-page-and-form}

Per garantire la corretta registrazione delle persone con ON24, è necessario includere i campi seguenti nel modulo Marketo:

* Nome
* Cognome
* Indirizzo e-mail

È inoltre possibile inviare i campi seguenti a ON24:

* Nome della società
* Professione

Aggiungendo il passaggio corretto alla campagna di registrazione, le persone verranno inviate a ON24 e contrassegnate come registrate. È possibile aggiungere altri campi al modulo e le informazioni verranno acquisite in Marketo come parte del record dei dettagli della persona.

>[!CAUTION]
>
>Per una corretta integrazione, è necessario utilizzare un modulo Marketo per registrare le persone per l’evento oppure un modulo non Marketo con l’integrazione API appropriata per inviare i dati di registrazione a Marketo.

## E-mail e token URL {#emails-and-url-tokens}

Crea le e-mail di invito, conferma, follow-up e ringraziamento tramite Marketo.

## E-mail di conferma Marketo e token URL {#marketo-confirmation-email-and-url-token}

Utilizza Marketo per inviare l’e-mail di conferma per l’evento. Quando una persona si registra, riceve un URL univoco da utilizzare per inserire l’evento.

>[!NOTE]
>
>Per compilare l&#39;e-mail di conferma con questo URL univoco, utilizza il seguente token nell&#39;e-mail: `{{member.webinar url}}`. Quando invii l’URL di conferma, questo token si risolve automaticamente nell’URL di conferma univoco della persona.
>
>Imposta il tipo di e-mail di conferma su **Operativo** per garantire che le persone che si registrano ricevano le informazioni di conferma, anche se hanno annullato l&#39;abbonamento.

>[!TIP]
>
>Puoi configurare ON24 per inviare conferme, promemoria o e-mail di follow-up. Per ulteriori informazioni, visitare il sito della Guida [ON24](https://www.on24.com/live-webcast-elite/){target="_blank"}.

## Requisiti della campagna secondaria di registrazione {#registration-child-campaign-requirements}

Gli eventi contengono una o più campagne secondarie che lavorano tutte insieme per spostare le persone attraverso gli stati del programma e ti consentono di monitorare le prestazioni dell’evento.

Esempi di campagne per bambini sono le campagne di invito, di registrazione e di follow-up.

>[!CAUTION]
>
>Affinché l&#39;adattatore possa svolgere il proprio lavoro, È NECESSARIO creare una campagna di registrazione. Questa campagna deve essere attivata dalla persona che compila un modulo e il primo passaggio deve cambiare lo stato del programma della persona in **Registrato**. La campagna invia quindi un’e-mail di conferma. Per ulteriori informazioni, consulta il resto di questo articolo.

**Registrazione/Conferma (Attiva campagna)**

* Elenco avanzato
* Trigger basato su **Compila modulo**. Accertati di includere la pagina di destinazione in cui si trova il modulo utilizzando **Aggiungi vincolo**, soprattutto se lo stesso modulo viene utilizzato in più pagine di destinazione.

>[!CAUTION]
>
>È necessario utilizzare un modulo Marketo per registrare le persone per l’evento oppure un modulo non Marketo con l’integrazione API appropriata per inviare i dati di registrazione a Marketo. Ciò è fondamentale per il successo dell’integrazione dei partner di eventi.

>[!NOTE]
>
>Se utilizzi un modulo Marketo in una pagina di destinazione non Marketo, il trigger sarà **Compila modulo** con il nome del modulo.

![](assets/image2015-12-22-15-3a20-3a51.png)

**Flusso**

* **Modifica stato programma** - Imposta su Webinar -> Registrato.

Questo passaggio di flusso è necessario come PRIMO PASSAGGIO DI FLUSSO durante la configurazione della campagna figlio. Quando lo stato di un programma cambia in Registrato, Marketo invia le informazioni di registrazione a ON24. Nessun altro stato spingerà la persona oltre.

* **Invia e-mail** - Messaggio di conferma. Imposta questa e-mail su **Operativo** in modo che le persone non abbonate che si sono registrate possano ancora riceverla.

Il passaggio del flusso **Invia e-mail** DEVE essere il secondo passaggio. L&#39;e-mail di conferma contiene `{{member.webinar url}}`, che viene compilato con le informazioni inviate nuovamente a Marketo da ON24.

![](assets/image2015-12-22-15-3a29-3a50.png)

>[!NOTE]
>
>L’ordine di questi passaggi di flusso è importante a causa dell’ordine in cui vengono eseguite le azioni in Marketo. Il passaggio **Modifica stato programma** invia la persona a ON24 per la registrazione e viene generato un URL univoco. In seguito, potrai inviare l&#39;e-mail di conferma che include questo URL univoco utilizzando il token `{{member.webinar URL}}`.
>
>Se la persona viene restituita con un errore di registrazione, non riceverà l’e-mail di conferma.

Il passaggio successivo è [verificare l&#39;integrazione dell&#39;evento ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/test-your-on24-event-integration.md){target="_blank"}.

>[!MORELIKETHIS]
>
>* [Informazioni sugli eventi della scheda di rete Marketo ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
>* [Esempio di integrazione evento ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md){target="_blank"}
>* [Informazioni sugli stati dei programmi di webinar](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-webinar-program-statuses.md){target="_blank"}
