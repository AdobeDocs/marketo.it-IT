---
description: Utilizzare le opzioni SMS in Smart List Triggers and Filters - Marketo Docs - Documentazione del prodotto
title: Utilizzare le opzioni SMS in Trigger e filtri di elenchi avanzati
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: 8e56b571a34451d6b0436dc041efaf0fd575db36
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 0%

---

# Utilizzare le opzioni SMS in Trigger e filtri di elenchi avanzati {#use-sms-options-in-smart-list-triggers-and-filters}

NUOVO DOCUMENTO

Dopo di te [creare un messaggio SMS](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-an-sms-message.md){target="_blank"}, per ottenere i vantaggi desiderati, è necessario utilizzare i trigger e i filtri dell’elenco avanzato all’interno di una campagna avanzata.

>[!PREREQUISITES]
>
>I trigger/filtri SMS vengono visualizzati solo se [Il servizio Vibes è stato abilitato](/help/marketo/product-docs/mobile-marketing/admin/add-vibes-as-a-launchpoint-service.md).

## Trigger SMS {#sms-triggers}

<table>
  <tr>
    <td><img src="assets/use-sms-options-in-smart-list-triggers-and-filters-1.png"></td>
    <td><img src="assets/use-sms-options-in-smart-list-triggers-and-filters-2.png"></td>
  </tr>
</table>

Di seguito sono riportati alcuni esempi:

Il **Mancato recapito messaggi SMS** trigger avvia un flusso, ad esempio l’invio di un’e-mail, quando un messaggio SMS viene recapitato.

Il **Abbonati all’elenco delle vibrazioni** attiva avvia un flusso quando una persona si abbona.

Il **Clic sul collegamento nel messaggio SMS** attiva avvia un flusso quando una persona fa clic su un collegamento nel messaggio SMS.

## Filtri SMS {#sms-filters}

<table>
  <tr>
    <td><img src="assets/use-sms-options-in-smart-list-triggers-and-filters-3.png"></td>
    <td><img src="assets/use-sms-options-in-smart-list-triggers-and-filters-4.png"></td>
  </tr>
</table>

È inoltre possibile utilizzare i filtri Vibes negli elenchi avanzati. Il **Abbonati all’elenco Vibes** il filtro trova chiunque abbia *sempre* Abbonati a Vibes. Sono incluse sia le persone cancellate che quelle cancellate, anche se le persone cancellate vengono omesse dal flusso. Questo filtro è più adatto per il reporting.

Per contro, la **Membro dell’elenco Vibes** risultati del filtro _chiunque_ attualmente abbonato a Vibes ed è più adatto per l’utilizzo in Campagne avanzate o elenchi.

>[!NOTE]
>
>Tutti i filtri SMS includono **Data di attività** per impostazione predefinita.

Dopo aver impostato i trigger e i filtri Vibes nell’elenco avanzato, puoi [definire il flusso](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/add-a-flow-step-for-sms.md).

>[!MORELIKETHIS]
>
>* [Inviare un messaggio SMS](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/send-an-sms-message.md)
>* [Definire un elenco avanzato per Smart Campaign | Attivatore](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
>* [Trovare e aggiungere filtri a un elenco avanzato](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)
