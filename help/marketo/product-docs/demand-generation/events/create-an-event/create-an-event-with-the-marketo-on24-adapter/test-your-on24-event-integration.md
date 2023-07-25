---
unique-page-id: 10096677
description: Test dell'integrazione degli eventi ON24 - Documentazione Marketo - Documentazione del prodotto
title: Test dell'integrazione degli eventi ON24
exl-id: 8326b81e-abf7-4615-9a0b-b0a579be8bb8
feature: Events
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 0%

---

# Test dell&#39;integrazione degli eventi ON24 {#test-your-on-event-integration}

Verifica a fondo l’integrazione dell’evento.

## Sequenza Di Test Consigliata Prima Di Eseguire La Prima Campagna {#recommended-test-sequence-before-running-your-first-campaign}

1. Compila il modulo di registrazione dell’evento e utilizza un indirizzo e-mail valido per il test.
1. Conferma la visualizzazione del nome del test con un **Registrato** stato nella griglia di iscrizione dell’evento Marketo.
1. Conferma che il nome del test sia visualizzato anche come **Registrato** in ON24.
1. Conferma che l’indirizzo e-mail valido utilizzato per registrare il nome del test abbia ricevuto un’e-mail di conferma all’evento e che l’URL univoco sia stato risolto nell’e-mail.

   >[!NOTE]
   >
   >È necessario utilizzare il `{{member.webinar url}}` token nell’e-mail di conferma affinché l’URL univoco venga visualizzato nell’e-mail di ciascun registrante.

## Dopo l’evento {#after-the-event}

Ecco come vengono aggiornati i dati dopo lo svolgimento dell’evento:

* Marketo recupera i dati dei partecipanti da ON24 ogni notte.
* Una volta sincronizzati i dati dei partecipanti tra Marketo e ON24, Marketo aggiorna lo stato di iscrizione a Partecipazione avvenuta, Partecipazione avvenuta su richiesta o Non presenziata. Nel campo **Riepilogo** , lo stato dell’evento viene aggiornato a **Evento - Completato**.

>[!MORELIKETHIS]
>
>* [Esempio di integrazione di eventi ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md){target="_blank"}
>* [Informazioni sugli eventi delle schede di rete Marketo ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
