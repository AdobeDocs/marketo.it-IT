---
description: Utilizzare i messaggi Vibes SMS in Smart List Triggers and Filters - Marketo Docs - Documentazione del prodotto
title: Utilizzare i messaggi Vibes SMS in Smart List Triggers and Filters
hide: true
hidefromtoc: true
feature: Mobile Marketing
source-git-commit: fee2d692acd8d54f2e308e2d5edc9876d13d5a4d
workflow-type: tm+mt
source-wordcount: '411'
ht-degree: 0%

---

# Utilizzare i messaggi Vibes SMS in Smart List Triggers and Filters {#use-vibes-sms-messages-in-smart-list-triggers-and-filters}

Dopo aver [creato un messaggio SMS Vibes](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/create-a-vibes-sms-message.md){target="_blank"}, è necessario utilizzare i trigger e i filtri dell&#39;elenco smart all&#39;interno di una campagna avanzata per ottenere i vantaggi. Ecco come.

1. In Il mio Marketo, fai clic su **Attività di marketing**.

   ![](assets/use-vibes-sms-messages-in-smart-list-triggers-and-filters-1.png)

1. Scegli una campagna avanzata in cui desideri utilizzare le risorse SMS. Trascina su un trigger. In questo esempio stiamo utilizzando **Compila modulo**.

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

Il trigger **Messaggi SMS non recapitati** avvia un flusso, ad esempio l&#39;invio di un&#39;e-mail, quando un messaggio SMS non viene inviato.

![](assets/sms-message-bounces-real.jpg)

Il trigger **Subscribes to Vibes List** avvia un flusso quando una persona si abbona.

![](assets/subscribes-to-vibes-list-real.jpg)

Il trigger **Click Link in SMS Message** avvia un flusso quando una persona fa clic su un collegamento nel messaggio SMS.

![](assets/clicks-link-in-sms-message.jpg)

## Filtri SMS {#sms-filters}

Puoi anche utilizzare i filtri Vibes negli elenchi avanzati. Il filtro **Abbonato all&#39;elenco Vibes** trova chiunque abbia *mai* abbonato a Vibes. Sono incluse sia le persone cancellate che quelle cancellate, anche se le persone cancellate vengono omesse dal flusso. Questo filtro è più adatto per il reporting.

![](assets/subscribed-to-vibes-list-filter-real.jpg)

Al contrario, il filtro **Membro dell&#39;elenco Vibes** trova _chiunque_ è attualmente abbonato a Vibes ed è più adatto per l&#39;utilizzo in campagne o elenchi Smart.

![](assets/image001.png)

>[!NOTE]
>
>Per impostazione predefinita, tutti i filtri SMS includono il vincolo **Data attività**.

Dopo aver impostato i trigger e i filtri Vibes nell&#39;elenco avanzato, puoi [definire il flusso](/help/marketo/product-docs/mobile-marketing/vibes-sms-messages/add-a-flow-step-for-sms.md).

>[!MORELIKETHIS]
>
>* [Definisci elenco avanzato per Smart Campaign | Trigger](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
>* [Trova e aggiungi filtri a un elenco avanzato](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)
