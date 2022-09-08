---
unique-page-id: 10096677
description: Verifica dell’integrazione degli eventi ON24 - Documenti Marketo - Documentazione del prodotto
title: Verifica dell’integrazione degli eventi ON24
exl-id: 8326b81e-abf7-4615-9a0b-b0a579be8bb8
source-git-commit: 40cfdddac66b7cd90e33bedf11888a7c5e3b38c9
workflow-type: tm+mt
source-wordcount: '211'
ht-degree: 0%

---

# Verifica dell’integrazione degli eventi ON24 {#test-your-on-event-integration}

>[!IMPORTANT]
>
>A partire da agosto 2022, ON24 non supporta più nuove integrazioni Marketo. Le informazioni contenute in questo articolo si applicano solo agli utenti esistenti.

Verifica accuratamente l’integrazione degli eventi.

## Sequenza di test consigliata prima di eseguire la prima campagna {#recommended-test-sequence-before-running-your-first-campaign}

1. Compila il modulo di registrazione dell&#39;evento e utilizza un indirizzo e-mail valido per il test.
1. Conferma la visualizzazione del nome del test con un **Registrato** nella griglia di appartenenza dell&#39;evento Marketo.
1. Conferma che il nome del test venga visualizzato anche come **Registrato** in ON24.
1. Conferma che l’indirizzo e-mail valido utilizzato per registrare il nome del test abbia ricevuto un’e-mail di conferma all’evento e che l’URL univoco sia stato risolto nell’e-mail.

   >[!NOTE]
   >
   >È necessario utilizzare `{{member.webinar url}}` token nell’e-mail di conferma affinché l’URL univoco venga visualizzato nell’e-mail di ciascun dichiarante.

## Dopo l’evento {#after-the-event}

Ecco come vengono aggiornati i dati dopo l’evento:

* Marketo recupera i dati dei partecipanti da ON24 ogni notte.
* Una volta effettuata la sincronizzazione dei dati dei partecipanti tra Marketo e ON24, Marketo aggiorna lo stato di iscrizione a Partecipato, Partecipato on-demand o Nessun programma. Nell&#39;evento **Riepilogo** lo stato dell’evento viene aggiornato in **Evento completato**.

>[!MORELIKETHIS]
>
>* [Esempio di integrazione di eventi ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/example-on24-event-integration.md)
>* [Informazioni sugli eventi dell&#39;adattatore Marketo ON24](/help/marketo/product-docs/demand-generation/events/create-an-event/create-an-event-with-the-marketo-on24-adapter/understanding-marketo-on24-adapter-events.md)

