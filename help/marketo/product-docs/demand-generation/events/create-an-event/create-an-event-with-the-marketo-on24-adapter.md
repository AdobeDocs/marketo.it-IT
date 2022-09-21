---
unique-page-id: 10096656
description: Creare un evento con l'adattatore Marketo ON24 - Marketo Docs - Documentazione del prodotto
title: Creare un evento con l'adattatore Marketo ON24
exl-id: a240ff72-b12f-4e3a-8e14-94fddb02f944
source-git-commit: 0c6c119f5be6e2ac3db7d99f7e8623d8aaa3555c
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Creare un evento con l&#39;adattatore Marketo ON24 {#create-an-event-with-the-marketo-on-adapter}

È necessario avere familiarità con i blocchi predefiniti e la sequenza consigliata per la creazione di eventi in Marketo. È inoltre necessario disporre di conoscenze pratiche sui seguenti concetti di Marketo:

* [Programmi Marketo](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md){target=&quot;_blank&quot;} così come gli eventi e le differenze tra loro
* [Canali](/help/marketo/product-docs/administration/tags/create-a-program-channel.md){target=&quot;_blank&quot;}
* [Risorse locali](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-local-assets-in-a-program.md){target=&quot;_blank&quot;}
* [Campagne per bambini](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md){target=&quot;_blank&quot;} e [Stati del programma](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md){target=&quot;_blank&quot;}

>[!NOTE]
>
>Fai riferimento alla [Documentazione API di Marketo](https://developers.marketo.com/documentation/rest/){target=&quot;_blank&quot;} per ulteriori informazioni sulle API Marketo.

## Prerequisiti {#prerequisites}

Per utilizzare l’integrazione Marketo ON24 sono necessari i seguenti requisiti:

* **Iscrizione ai webcast ON24** - Se non si dispone di un abbonamento corrente, contattare direttamente ON24. **NOTA**: ON24 Hosted Edition è richiesto. ON24 Event Management non è richiesto.

* **Diritti di amministratore su ON24** - Avrete bisogno di questo per utilizzare questo connettore e creare ospiti nel sistema ON24.
* **Credenziali di connessione ON24** - Devi inserire queste informazioni in Marketo per abilitare l’integrazione: Nome utente, password, ID client e chiave client. Contatta il tuo Account Manager ON24 o il supporto ON24 se hai bisogno di aiuto con le tue credenziali.
* **Modulo di registrazione** - Utilizza un modulo Marketo o un modulo non Marketo insieme all’API appropriata per garantire che i dati di registrazione e le informazioni sul dichiarante vengano trasmessi a Marketo.
* **Campagna bambini di registrazione** - È necessario creare e configurare correttamente una campagna figlio di registrazione nell’evento Marketo affinché l’integrazione dei partner eventi funzioni correttamente.

## Flusso dei processi {#process-flow}

Segui questi passaggi per creare un evento con l&#39;adattatore Marketo On24:

1. [Crea il tuo evento webinar in ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-your-webinar-event-in-on24.md){target=&quot;_blank&quot;}
1. [Configurare le impostazioni evento e sincronizzare Marketo con il webinar](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md){target=&quot;_blank&quot;}
1. [Creare campagne figlio e risorse locali](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-child-campaigns-and-local-assets.md){target=&quot;_blank&quot;}
1. [Verifica dell’integrazione degli eventi ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/test-your-on24-event-integration.md){target=&quot;_blank&quot;}
1. [Esempio di integrazione di eventi ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md){target=&quot;_blank&quot;}
1. [Informazioni sugli stati del programma webinar](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-webinar-program-statuses.md){target=&quot;_blank&quot;}
1. [Aggiornamenti alla registrazione degli eventi ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/on24-event-registration-updates.md){target=&quot;_blank&quot;}
