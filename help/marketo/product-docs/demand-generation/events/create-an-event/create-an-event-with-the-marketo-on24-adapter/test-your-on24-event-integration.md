---
unique-page-id: 10096677
description: Verificare L'Integrazione Degli Eventi ON24 - Documenti Marketo - Documentazione Del Prodotto
title: Verificare l'integrazione degli eventi ON24
translation-type: tm+mt
source-git-commit: 5c9683c6b00ccbf9e9d606fd4513432c9872ad00
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 0%

---


# Verificare l&#39;integrazione degli eventi ON24 {#test-your-on-event-integration}

Assicuratevi di verificare accuratamente l&#39;integrazione degli eventi.

## Sequenza Di Test Consigliata Prima Di Eseguire La Prima Campagna {#recommended-test-sequence-before-running-your-first-campaign}

1. Compilate il modulo di registrazione dell&#39;evento e utilizzate un indirizzo e-mail valido per il test.
1. Confermate la visualizzazione del nome del test con uno stato **Registrato** nella griglia Appartenenza dell&#39;evento Marketo.
1. Confermate che il nome del test venga visualizzato anche come **Registrato** in ON24.
1. Confermate che l&#39;indirizzo e-mail valido usato per registrare il nome del test abbia ricevuto un messaggio e-mail di conferma all&#39;evento e che l&#39;URL univoco sia stato risolto nell&#39;e-mail.

   >[!NOTE]
   >
   >Affinché l’URL univoco possa essere visualizzato nell’e-mail di ciascun utente registrato, dovete usare il `{{member.webinar url}}` token nell’e-mail di conferma.

## Dopo l’evento {#after-the-event}

Di seguito è spiegato in che modo i dati vengono aggiornati dopo l’evento:

* Marketo recupera i dati dei partecipanti da ON24 ogni notte.
* Dopo la sincronizzazione dei dati dei partecipanti tra Marketo e ON24, Marketo aggiorna lo stato dell’iscrizione a Partecipante, Partecipato on-demand o Nessun evento. Nella scheda **Riepilogo** dell&#39;evento, lo stato dell&#39;evento viene aggiornato a **Evento completato**.

>[!NOTE]
>
>**Articoli correlati**
>
>* [Esempio di integrazione evento ON24](example-on24-event-integration.md)
>* [Informazioni sugli eventi dell&#39;adattatore Marketo ON24](understanding-marketo-on24-adapter-events.md)

>



