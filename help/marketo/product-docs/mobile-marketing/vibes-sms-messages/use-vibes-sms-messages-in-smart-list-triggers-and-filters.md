---
unique-page-id: 11378871
description: Usa messaggi SMS Vibs in Smart List Triggers e Filtri - Marketo Docs - Documentazione del prodotto
title: Utilizzare i messaggi SMS Vibs in attivatori e filtri di elenchi avanzati
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '287'
ht-degree: 0%

---


# Utilizzare i messaggi SMS Vibs in attivatori e filtri di elenchi avanzati {#use-vibes-sms-messages-in-smart-list-triggers-and-filters}

Dopo aver [creato un messaggio](create-a-vibes-sms-message.md)Vibes SMS, è possibile utilizzare attivatori e filtri per elenchi smart all&#39;interno di una campagna intelligente per ottenere i vantaggi. Ecco come.

1. In My Marketo fate clic su **Marketing Activities (Attività** marketing).

   ![](assets/image2016-7-28-9-3a48-3a32.png)

1. Scegliete una campagna intelligente in cui desiderate utilizzare la risorsa SMS. Trascinare su un trigger, ad esempio il popolare **Modulo** di compilazione.

   ![](assets/fills-out-form-pull-over.jpg)

## Attivatori SMS {#sms-triggers}

Sono disponibili altri attivatori SMS. Gli attivatori SMS vengono visualizzati solo se il servizio Vibes è abilitato.

![](assets/new-sms-search2.png)

Di seguito sono riportati alcuni esempi.

L&#39;attivatore Bounces messaggio SMS avvia un flusso, ad esempio l&#39;invio di un&#39;e-mail, quando un messaggio SMS viene rimbalzato.

![](assets/sms-message-bounces-real.jpg)

L’attivazione **Iscrizione a elenco** vibrazioni avvia un flusso quando una persona si iscrive.

![](assets/subscribes-to-vibes-list-real.jpg)

L&#39;attivatore** Click Link in SMS Message** avvia un flusso quando una persona fa clic su un collegamento nel messaggio SMS.

![](assets/clicks-link-in-sms-message.jpg)

## Filtri SMS {#sms-filters}

Potete anche utilizzare i filtri Vibes negli elenchi smart. Il filtro **Iscrizione a elenco** vibrazioni individua chiunque abbia *mai* effettuato l’iscrizione a Vibes. Questo include sia persone non sottoscritte che eliminate, anche se le persone eliminate vengono omesse dal flusso. Questo filtro è ideale per i report.

![](assets/subscribed-to-vibes-list-filter-real.jpg)

Per contro, il **filtro** **Member of Vibes List **trova** **chiunque** ***attualmente* iscritto a Vibes ed è più adatto per l&#39;utilizzo in campagne o elenchi intelligenti.

![](assets/image001.png)

>[!NOTE]
>
>Tutti i filtri SMS includono il vincolo **Data dell&#39;attività** per impostazione predefinita.

Dopo aver impostato attivatori e filtri Vibes nell&#39;elenco avanzato, potete [definire il flusso](add-a-flow-step-for-sms.md).

>[!MORELIKETHIS]
>
>* [Definisci elenco avanzato per Smart Campaign | Trigger](../../../product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/define-smart-list-for-smart-campaign-trigger.md)
>* [Trovare e aggiungere filtri a un elenco avanzato](../../../product-docs/core-marketo-concepts/smart-lists-and-static-lists/creating-a-smart-list/find-and-add-filters-to-a-smart-list.md)
>* [Aggiunta di un passaggio di flusso per SMS](add-a-flow-step-for-sms.md)

>



