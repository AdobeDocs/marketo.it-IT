---
unique-page-id: 10096677
description: Test dell'integrazione degli eventi ON24 - Documentazione Marketo - Documentazione del prodotto
title: Test dell'integrazione degli eventi ON24
exl-id: 8326b81e-abf7-4615-9a0b-b0a579be8bb8
feature: Events
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '183'
ht-degree: 0%

---

# Test dell&#39;integrazione degli eventi ON24 {#test-your-on-event-integration}

Verifica a fondo l’integrazione dell’evento.

## Sequenza Di Test Consigliata Prima Di Eseguire La Prima Campagna {#recommended-test-sequence-before-running-your-first-campaign}

1. Compila il modulo di registrazione dell’evento e utilizza un indirizzo e-mail valido per il test.
1. Conferma che il nome del test venga visualizzato con lo stato **Registrato** nella griglia di appartenenza dell&#39;evento Marketo.
1. Conferma che il nome del test sia visualizzato anche come **Registrato** in ON24.
1. Conferma che l’indirizzo e-mail valido utilizzato per registrare il nome del test abbia ricevuto un’e-mail di conferma all’evento e che l’URL univoco sia stato risolto nell’e-mail.

   >[!NOTE]
   >
   >Devi utilizzare il token `{{member.webinar url}}` nell&#39;e-mail di conferma affinché l&#39;URL univoco venga visualizzato nell&#39;e-mail di ogni registrante.

## Dopo l’evento {#after-the-event}

Ecco come vengono aggiornati i dati dopo lo svolgimento dell’evento:

* Marketo recupera i dati dei partecipanti da ON24 ogni notte.
* Una volta sincronizzati i dati dei partecipanti tra Marketo e ON24, Marketo aggiorna lo stato di iscrizione a [!UICONTROL Attended], [!UICONTROL Attended On-demand] o [!UICONTROL No Show]. Nella scheda **[!UICONTROL Summary]** dell&#39;evento, lo stato dell&#39;evento è aggiornato a **[!UICONTROL Event Complete]**.

>[!MORELIKETHIS]
>
>* [Esempio di integrazione evento ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md){target="_blank"}
>* [Informazioni sugli eventi della scheda di rete Marketo ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md){target="_blank"}
