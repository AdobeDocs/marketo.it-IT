---
description: Utilizzo delle opzioni SMS in una campagna avanzata - Documentazione di Marketo - Documentazione del prodotto
title: Utilizzo delle opzioni SMS in una campagna avanzata
feature: Mobile Marketing
source-git-commit: efaf34e8113fc6364655ff01aa788aa62bdd31af
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 0%

---

# Utilizzo delle opzioni SMS in una campagna avanzata {#using-sms-options-in-a-smart-campaign}

Dopo di te [creare un messaggio SMS](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-an-sms-message-2.md){target="_blank"}, per ottenere i vantaggi desiderati, è necessario utilizzare i trigger e i filtri dell’elenco avanzato all’interno di una campagna avanzata.

>[!NOTE]
>
>Se stai cercando di inviare un messaggio SMS, abbiamo un [articolo specifico](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-an-sms-message.md){target="_blank"} per quello.

>[!PREREQUISITES]
>
>I trigger/filtri SMS vengono visualizzati solo se [Il servizio Vibes è stato abilitato](/help/marketo/product-docs/mobile-marketing/admin/add-vibes-as-a-launchpoint-service.md){target="_blank"}.

## Trigger SMS {#sms-triggers}

<table style="width:600px">
  <tr>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-1.png"></td>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-2.png"></td>
  </tr>
</table>

Di seguito sono riportati alcuni esempi:

Il **Mancato recapito messaggi SMS** trigger avvia un flusso, ad esempio l’invio di un’e-mail, quando un messaggio SMS viene recapitato.

Il **Abbonati all’elenco delle vibrazioni** attiva avvia un flusso quando una persona si abbona.

Il **Clic sul collegamento nel messaggio SMS** attiva avvia un flusso quando una persona fa clic su un collegamento nel messaggio SMS.

## Filtri SMS {#sms-filters}

<table style="width:600px">
  <tr>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-3.png"></td>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-4.png"></td>
  </tr>
</table>

Il **Abbonati all’elenco Vibes** il filtro trova chiunque abbia *sempre* Abbonati a Vibes. Sono incluse sia le persone cancellate che quelle cancellate, anche se le persone cancellate vengono omesse dal flusso. Questo filtro è più adatto per il reporting.

Per contro, la **Membro dell’elenco Vibes** risultati del filtro _chiunque_ attualmente abbonato a Vibes ed è più adatto per l’utilizzo in Campagne avanzate o elenchi.

>[!NOTE]
>
>Tutti i filtri SMS includono **Data di attività** per impostazione predefinita.

## Passaggi del flusso SMS {#sms-flow-steps}

È possibile scegliere tra tre passaggi del flusso SMS.

![](assets/using-sms-options-in-a-smart-campaign-5.png)

<table>
<tbody>
  <tr>
    <td style="width:20%"><b>Invia messaggio SMS</b></td>
    <td>Questa azione di flusso invia messaggi agli utenti di Marketo Smart List che sono abbonati a un elenco di abbonamenti Vibes con consenso dell’utente. Non avvia il processo di abbonamento. <a href="/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-an-sms-message.md">Ulteriori informazioni</a>.</td>
  </tr>

<tr>
    <td style="width:20%"><b>Iscriviti all’elenco delle vibrazioni</b></td>
    <td>Questa azione di flusso avvia il processo di abbonamento SMS tramite una campagna di acquisizione Vibes selezionata dall’utente. Vibes invia quindi un messaggio di conferma e il destinatario deve rispondere con "Y" entro 24 ore per confermare l’opt-in. Una volta che l’utente ha acconsentito, diventerà membro dell’elenco di iscrizioni Vibes associato.</td>
  </tr>
  <tr>
    <td style="width:20%"><b>Annulla iscrizione all’elenco delle vibrazioni</b></td>
    <td>Questa azione di flusso annulla l’abbonamento di ogni persona da un elenco di abbonamenti Vibes con consenso esplicito dell’utente. Quando un utente scrive "STOP" al codice, il record della persona viene aggiornato per indicare che non è più membro dell’elenco di abbonamento a Vibes.</td>
  </tr>
  </tbody>
</table>

>[!NOTE]
>
>Il **Iscriviti all’elenco delle vibrazioni** e **Annulla iscrizione all’elenco delle vibrazioni** i flussi hanno requisiti diversi. Per **Abbonati**, è necessario selezionare l’elenco Vibes e la campagna di acquisizione Vibes. Per **Annulla iscrizione**, è necessario solo l’elenco Vibes.

>[!MORELIKETHIS]
>
>* [Inviare un messaggio SMS](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-an-sms-message.md){target="_blank"}
>* [Definire un elenco avanzato per Smart Campaign | Trigger](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md){target="_blank"}
>* [Definire un elenco avanzato per Smart Campaign | Batch](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md){target="_blank"}
