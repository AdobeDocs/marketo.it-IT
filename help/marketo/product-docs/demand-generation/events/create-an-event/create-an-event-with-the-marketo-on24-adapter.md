---
unique-page-id: 10096656
description: Creazione di un evento con l'adattatore Marketo ON24 - Documentazione Marketo - Documentazione del prodotto
title: Creazione di un evento con la scheda Marketo ON24
exl-id: a240ff72-b12f-4e3a-8e14-94fddb02f944
feature: Events
source-git-commit: 2b610cc3486b745212b0b1f36018a83214d7ecd7
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 0%

---

# Creazione di un evento con la scheda Marketo ON24 {#create-an-event-with-the-marketo-on-adapter}

Devi acquisire familiarità con i blocchi predefiniti e la sequenza consigliata per la creazione di eventi in Marketo. Dovresti anche avere una conoscenza operativa dei seguenti concetti di Marketo:

* [Programmi di Marketo](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-programs.md){target="_blank"}, eventi e differenze
* [Canali](/help/marketo/product-docs/administration/tags/create-a-program-channel.md){target="_blank"}
* [Assets locale](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/understanding-local-assets-in-a-program.md){target="_blank"}
* [Campagne secondarie](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md){target="_blank"} e [Stati programma](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/program-flow-actions/change-program-status.md){target="_blank"}

>[!NOTE]
>
>Per ulteriori informazioni sulle API di Marketo, consulta la [documentazione delle API di Marketo](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/rest/rest-api){target="_blank"}.

## Prerequisiti {#prerequisites}

Per utilizzare l&#39;integrazione Marketo ON24 sono necessari i seguenti elementi:

* **Abbonamento a webcast ON24** - Se non disponi di un abbonamento corrente, contatta direttamente ON24. **NOTA**: è richiesta l&#39;edizione in hosting ON24. Gestione degli eventi ON24 non richiesta.

* **Diritti di amministratore per ON24** - Per utilizzare questo connettore e creare guest nel sistema ON24 è necessario.
* **Credenziali di connessione ON24** - Immettere queste informazioni in Marketo per abilitare l&#39;integrazione: Nome utente, Password, ID client e Chiave client. Contatta il tuo Account Manager ON24 o il Supporto ON24 se hai bisogno di assistenza con le tue credenziali.
* **Modulo di registrazione**: utilizza un modulo Marketo o un modulo non Marketo insieme all&#39;API appropriata per garantire che i dati di registrazione e le informazioni del registrante vengano passati a Marketo.
* **Campagna figlio di registrazione** - Una campagna figlio di registrazione nell&#39;evento Marketo deve essere creata e configurata correttamente affinché l&#39;integrazione Partner eventi funzioni.

## Flusso di processo {#process-flow}

Per creare un evento con l&#39;adattatore Marketo On24, eseguire la procedura seguente:

1. [Crea il tuo evento webinar in ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-your-webinar-event-in-on24.md){target="_blank"}
1. [Configurare le impostazioni degli eventi e sincronizzare Marketo con il webinar](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/configure-event-settings-and-sync-marketo-with-your-webinar.md){target="_blank"}
1. [Creazione di campagne secondarie e Assets locale](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/create-child-campaigns-and-local-assets.md){target="_blank"}
1. [Verifica l&#39;integrazione dell&#39;evento ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/test-your-on24-event-integration.md){target="_blank"}
1. [Esempio di integrazione evento ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md){target="_blank"}
1. [Informazioni sugli stati dei programmi di webinar](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-webinar-program-statuses.md){target="_blank"}
1. [Aggiornamenti registrazione eventi ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/on24-event-registration-updates.md){target="_blank"}
