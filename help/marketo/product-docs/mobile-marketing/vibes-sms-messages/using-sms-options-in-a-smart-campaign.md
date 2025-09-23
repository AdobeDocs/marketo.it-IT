---
description: Utilizzo delle opzioni SMS in una campagna avanzata - Documentazione di Marketo - Documentazione del prodotto
title: Utilizzo delle opzioni SMS in una campagna avanzata
feature: Mobile Marketing
exl-id: 199b7cae-86d2-42fe-8934-10aa780f4454
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '406'
ht-degree: 3%

---

# Utilizzo delle opzioni SMS in una campagna avanzata {#using-sms-options-in-a-smart-campaign}

Dopo aver [creato un messaggio SMS](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-an-sms-message.md){target="_blank"}, è necessario utilizzare i trigger e i filtri dell&#39;elenco smart all&#39;interno di una campagna avanzata per ottenere i vantaggi.

>[!NOTE]
>
>Se stai cercando di inviare un messaggio SMS, abbiamo un [articolo specifico](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-an-sms-message.md){target="_blank"} per questo.

>[!PREREQUISITES]
>
>I trigger/filtri SMS vengono visualizzati solo se il servizio [Vibes è stato abilitato](/help/marketo/product-docs/mobile-marketing/admin/add-vibes-as-a-launchpoint-service.md){target="_blank"}.

## Trigger SMS {#sms-triggers}

<table style="width:600px">
  <tr>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-1.png"></td>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-2.png"></td>
  </tr>
</table>

Di seguito sono riportati alcuni esempi:

Il trigger **Messaggi SMS non recapitati** avvia un flusso, ad esempio l&#39;invio di un&#39;e-mail, quando un messaggio SMS non viene inviato.

Il trigger **Subscribes to Vibes List** avvia un flusso quando una persona si abbona.

Il trigger **Click Link in SMS Message** avvia un flusso quando una persona fa clic su un collegamento nel messaggio SMS.

## Filtri SMS {#sms-filters}

<table style="width:600px">
  <tr>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-3.png"></td>
    <td style="width:50%"><img src="assets/using-sms-options-in-a-smart-campaign-4.png"></td>
  </tr>
</table>

Il filtro **Abbonato all&#39;elenco Vibes** trova chiunque abbia *mai* abbonato a Vibes. Sono incluse sia le persone cancellate che quelle cancellate, anche se le persone cancellate vengono omesse dal flusso. Questo filtro è più adatto per il reporting.

Al contrario, il filtro **Membro dell&#39;elenco Vibes** trova *chiunque* è attualmente abbonato a Vibes ed è più adatto per l&#39;utilizzo in campagne o elenchi Smart.

>[!NOTE]
>
>Per impostazione predefinita, tutti i filtri SMS includono il vincolo **Data attività**.

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
>I flussi **Abbonati all&#39;elenco delle vibrazioni** e **Annulla abbonamento all&#39;elenco delle vibrazioni** hanno requisiti diversi. Per **Abbonati**, devi selezionare l&#39;elenco Vibes e la campagna di acquisizione Vibes. Per **Annulla sottoscrizione**, è necessario solo l&#39;elenco Vibes.

>[!MORELIKETHIS]
>
>* [Invia un messaggio SMS](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-an-sms-message.md){target="_blank"}
>* [Definisci elenco avanzato per Smart Campaign | Trigger](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md){target="_blank"}
>* [Definisci elenco avanzato per Smart Campaign | Batch](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-batch.md){target="_blank"}
