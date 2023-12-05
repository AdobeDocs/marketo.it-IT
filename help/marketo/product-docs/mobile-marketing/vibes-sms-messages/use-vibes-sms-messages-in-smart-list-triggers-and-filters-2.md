---
description: Utilizzare i messaggi Vibes SMS in Smart List Triggers and Filters - Marketo Docs - Documentazione del prodotto
title: Utilizzare i messaggi Vibes SMS in Smart List Triggers and Filters
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: cd09ad43c08855af63131aa385c4fd406c963926
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 0%

---

# Utilizzare i messaggi Vibes SMS in Smart List Triggers and Filters {#use-vibes-sms-messages-in-smart-list-triggers-and-filters}

Dopo di te [creare un messaggio Vibes SMS](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-a-vibes-sms-message.md){target="_blank"}, per ottenere i vantaggi desiderati, è necessario utilizzare i trigger e i filtri dell’elenco avanzato all’interno di una campagna avanzata. Ecco come.

1. In Il mio Marketo, fai clic su **Attività di marketing**.

   ![](assets/use-vibes-sms-messages-in-smart-list-triggers-and-filters-1.png)

1. Scegli una campagna avanzata in cui desideri utilizzare le risorse SMS. Trascina su un trigger. In questo esempio utilizziamo **Compila modulo**.

   ![](assets/fills-out-form-pull-over.jpg)

## Trigger SMS {#sms-triggers}

Sono disponibili altri trigger SMS. I trigger SMS vengono visualizzati solo se il servizio Vibes è abilitato.

INVIA UN MESSAGGIO SMS:

* Attività di marketing > scegli nuova campagna avanzata
   * Elenco avanzato > Scegli elenco Vibes filtro e logica corretta > Elenco Vibes: seleziona dall’elenco a discesa (elenco di database mobili sincronizzato dalla piattaforma Vibes)
      * Puoi perfezionare la segmentazione e utilizzare filtri e attivatori SMS ed e-mail all’interno di una campagna
      * Filtri Vibes: Abbonati all’elenco Vibes vs. Membri dell’elenco Vibes - La logica è coerente con l’e-mail
         * Abbonati all’elenco Vibes: i partecipanti che si sono iscritti a tale elenco anche se ora non sono iscritti.  - viene utilizzato principalmente per attività di marketing cross-channel
            * Nota: un messaggio SMS non invierà a nessuno che ha annullato l’abbonamento se non è incluso nell’elenco del database mobile di Vibes
         * Membro dell’elenco Vibes - abbonato attivo e confermato
         * Aggiunto all’elenco: gli elenchi Vibes non verranno compilati con questo filtro; è per gli elenchi Marketo

![](assets/new-sms-search2.png)

Di seguito sono riportati alcuni esempi:

Il **Mancato recapito messaggi SMS** trigger avvia un flusso, ad esempio l’invio di un’e-mail, quando un messaggio SMS viene recapitato.

![](assets/sms-message-bounces-real.jpg)

Il **Abbonati all’elenco delle vibrazioni** attiva avvia un flusso quando una persona si abbona.

![](assets/subscribes-to-vibes-list-real.jpg)

Il **Clic sul collegamento nel messaggio SMS** attiva avvia un flusso quando una persona fa clic su un collegamento nel messaggio SMS.

![](assets/clicks-link-in-sms-message.jpg)

## Filtri SMS {#sms-filters}

Puoi anche utilizzare i filtri Vibes negli elenchi avanzati. Il **Abbonati all’elenco Vibes** il filtro trova chiunque abbia *sempre* Abbonati a Vibes. Sono incluse sia le persone cancellate che quelle cancellate, anche se le persone cancellate vengono omesse dal flusso. Questo filtro è più adatto per il reporting.

![](assets/subscribed-to-vibes-list-filter-real.jpg)

Per contro, la **Membro dell’elenco Vibes** risultati del filtro _chiunque_ attualmente abbonato a Vibes ed è più adatto per l’utilizzo in Campagne avanzate o elenchi.

![](assets/image001.png)

>[!NOTE]
>
>Tutti i filtri SMS includono **Data di attività** per impostazione predefinita.

Dopo aver impostato i trigger e i filtri Vibes nell’elenco avanzato, puoi [definire il flusso](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/add-a-flow-step-for-sms.md).

>[!MORELIKETHIS]
>
>* [Definire un elenco avanzato per Smart Campaign | Attivatore](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
>* [Trovare e aggiungere filtri a un elenco avanzato](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)
