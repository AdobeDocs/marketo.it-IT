---
unique-page-id: 10096656
description: Creazione di un evento con l'adattatore Marketo ON24 - Documentazione Marketo - Documentazione del prodotto
title: Creazione di un evento con l'adattatore Marketo ON24
exl-id: a240ff72-b12f-4e3a-8e14-94fddb02f944
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 0%

---

# Creazione di un evento con l&#39;adattatore Marketo ON24 {#create-an-event-with-the-marketo-on-adapter}

Devi acquisire familiarità con i blocchi predefiniti e la sequenza consigliata per la creazione di eventi in Marketo. Dovresti anche avere una conoscenza operativa dei seguenti concetti di Marketo:

* [Programmi Marketo](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md){target="_blank"} nonché Eventi e differenze tra di essi
* [Canali](/help/marketo/product-docs/administration/tags/create-a-program-channel.md){target="_blank"}
* [Risorse locali](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-local-assets-in-a-program.md){target="_blank"}
* [Campagne figlie](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md){target="_blank"} and [Program Statuses](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md){target="_blank"}

>[!NOTE]
>
>Consulta la sezione [Documentazione API di Marketo](https://developers.marketo.com/documentation/rest/){target="_blank"} per ulteriori informazioni sulle API di Marketo.

## Prerequisiti {#prerequisites}

Per utilizzare l&#39;integrazione Marketo ON24 sono necessari i seguenti elementi:

* **Abbonamento a webcast ON24** - Se non disponi di un abbonamento corrente, contatta direttamente ON24. **NOTA**: ON24 Hosted Edition è obbligatorio. Gestione degli eventi ON24 non richiesta.

* **Diritti di amministratore per ON24** - È necessario utilizzare questo connettore per creare ospiti nel sistema ON24.
* **Credenziali di connessione ON24** - Immetti queste informazioni in Marketo per abilitare l’integrazione: Nome utente, Password, ID client e Chiave client. Contatta il tuo Account Manager ON24 o il Supporto ON24 se hai bisogno di assistenza con le tue credenziali.
* **Modulo di registrazione** : utilizza un modulo Marketo o non Marketo insieme all’API appropriata per garantire che i dati di registrazione e le informazioni sul registrante vengano passati a Marketo.
* **Campagna secondaria di registrazione** - Affinché l’integrazione Partner eventi funzioni, è necessario creare e configurare correttamente una campagna figlio di registrazione nell’evento Marketo.

## Flusso di processo {#process-flow}

Per creare un evento con l&#39;adattatore Marketo On24, eseguire la procedura seguente:

1. [Creare un evento webinar in ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-your-webinar-event-in-on24.md){target="_blank"}
1. [Configurare le impostazioni degli eventi e sincronizzare Marketo con il webinar](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md){target="_blank"}
1. [Creare campagne secondarie e risorse locali](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-child-campaigns-and-local-assets.md){target="_blank"}
1. [Test dell&#39;integrazione degli eventi ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/test-your-on24-event-integration.md){target="_blank"}
1. [Esempio di integrazione di eventi ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md){target="_blank"}
1. [Informazioni sugli stati dei programmi di webinar](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-webinar-program-statuses.md){target="_blank"}
1. [Aggiornamenti alla registrazione dell&#39;evento ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/on24-event-registration-updates.md){target="_blank"}
