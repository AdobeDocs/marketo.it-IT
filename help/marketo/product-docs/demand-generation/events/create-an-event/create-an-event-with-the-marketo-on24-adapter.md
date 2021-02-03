---
unique-page-id: 10096656
description: Creazione di un evento con l'adattatore Marketo ON24 - Marketo Docs - Documentazione del prodotto
title: Creazione di un evento con l'adattatore Marketo ON24
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '296'
ht-degree: 0%

---


# Creazione di un evento con la scheda Marketo ON24 {#create-an-event-with-the-marketo-on-adapter}

## Prima di iniziare {#before-you-begin}

È necessario avere familiarità con i blocchi di generazione e con la sequenza consigliata per la creazione di eventi in Marketo. È inoltre necessario avere una conoscenza approfondita dei seguenti concetti di Marketo:

* [Programmi Marketo, ](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md) eventi e differenze tra di essi
* [Canali](/help/marketo/product-docs/administration/tags/create-a-program-channel.md)
* [Risorse locali](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-local-assets-in-a-program.md)
* [Campagne ](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md) figlio e stati  [del programma](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md)

>[!NOTE]
>
>Per ulteriori informazioni sulle API di Marketo, consultare la [documentazione API di Marketo](https://developers.marketo.com/documentation/rest/).

## Prerequisiti {#prerequisites}

Per utilizzare l&#39;integrazione Marketo ON24 sono necessari i seguenti requisiti:

* **Iscrizione a webcast**  ON24 - Se non disponete di un&#39;iscrizione corrente, contattate direttamente ON24. **NOTA**: ON24 Hosted Edition è richiesto. ON24 Event Management non è richiesto.

* **Diritti di amministratore su ON24** - Sarà necessario utilizzare questo connettore e creare ospiti nel sistema ON24.
* **Credenziali**  di connessione ON24: per abilitare l&#39;integrazione, è necessario immettere queste informazioni in Markech: Nome utente, password, ID client e chiave client. Contattate il vostro Account Manager ON24 o il servizio di assistenza ON24 se avete bisogno di aiuto per le vostre credenziali.
* **Modulo**  di registrazione - Utilizzate un modulo Marketo o un modulo non Marketo insieme all&#39;API appropriata per garantire che i dati di registrazione e le informazioni di registrazione vengano passati a Marketo.
* **Campagna**  figlio per la registrazione - Una campagna figlio per la registrazione all’evento Marketo deve essere creata e configurata correttamente per il corretto funzionamento dell’integrazione con il partner evento.

## Flusso di processo {#process-flow}

Per creare un evento con la scheda Marketo On24, effettuate le seguenti operazioni:

1. [Inserisci le tue credenziali ON24 in Marketo](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/enter-your-on24-credentials-in-marketo.md)
1. [Creazione di un evento webinar in ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-your-webinar-event-in-on24.md)
1. [Configurare le impostazioni evento e sincronizzare il marketing con il webinar](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md)
1. [Creare campagne figlio e risorse locali](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-child-campaigns-and-local-assets.md)
1. [Verificare l&#39;integrazione degli eventi ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/test-your-on24-event-integration.md)
1. [Esempio di integrazione evento ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md)
1. [Informazioni sugli stati del programma webinar](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-webinar-program-statuses.md)
1. [Aggiornamenti alla registrazione degli eventi ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/on24-event-registration-updates.md)
