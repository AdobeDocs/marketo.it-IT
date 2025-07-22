---
unique-page-id: 14352407
description: Panoramica del canale di consegna - Documentazione di Marketo - Documentazione del prodotto
title: Panoramica del canale di consegna
exl-id: 432bad1e-4eaf-4be8-b856-be364c44816e
feature: Marketo Sales Connect
source-git-commit: 0d37fbdb7d08901458c1744dc68893e155176327
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 0%

---

# Panoramica del canale di consegna {#delivery-channel-overview}

Marketo [!DNL Sales Connect] offre più opzioni per la consegna delle e-mail. Questo articolo analizza i canali di consegna che puoi sfruttare, come selezionarli e quando sceglierne uno rispetto all’altro.

## Consigliato: Gmail o [!DNL Exchange] tramite connessione e-mail {#recommended-gmail-or-exchange-via-email-connection}

[!DNL Sales Connect] consente una configurazione semplificata e il recapito messaggi migliorato tramite il servizio Email Connection. [!UICONTROL Email Connection] consente a ogni utente di connettersi al proprio account [Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md) o [Exchange](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md) a [!DNL Sales Connect] per essere utilizzato come canale di consegna preferito per tutte le e-mail [!DNL Sales Connect].

L&#39;utilizzo di Gmail o [!DNL Exchange] offre alcuni vantaggi rispetto ad altre opzioni di canale di consegna:

* Si tratta di un canale di consegna collaudato e con una reputazione consolidata che contribuisce a mantenere elevato il tasso di consegna.
* I metodi di autenticazione come SPF e DKIM sono già configurati e gestiti dal team IT, pertanto non vi sono configurazioni aggiuntive.
* L&#39;invio di e-mail all&#39;interno di una determinata rete (ad esempio, l&#39;invio di un&#39;e-mail come utente [!DNL Exchange] a una società che riceve e-mail tramite [!DNL Exchange]) può contribuire ad aumentare ulteriormente il recapito messaggi.

È importante notare che questi canali di consegna hanno i propri limiti di invio che vengono applicati da Microsoft e Google. Per combattere questo problema, utilizziamo un meccanismo di limitazione per aiutare gli utenti a rimanere entro tali limiti. Ulteriori informazioni sulla limitazione di [posta elettronica](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md).

>[!NOTE]
>
>Per impostazione predefinita, il plug-in O365 utilizzerà sempre il tuo canale di consegna Exchange e il plug-in Gmail utilizzerà sempre il tuo canale di consegna Gmail per inviare e-mail dai plug-in.

**Tracciamento dei messaggi non recapitati**: MSC può rilevare i messaggi non recapitati per [!DNL Exchange Online] o utenti Gmail rilevando il messaggio non recapitati inviato alla casella in entrata del mittente. Queste notifiche di mancato recapito verranno aggregate in Template Analytics, Campaign Analytics e Live Feed per gli utenti. Il rilevamento delle e-mail non consegnate non è supportato per [!DNL Exchange] clienti locali.

## Canale di consegna personalizzato tramite SMTP {#custom-delivery-channel-via-smtp}

[!DNL Sales Connect] offre l&#39;opzione aggiuntiva di connettere un server SMTP di terze parti da utilizzare come canale di consegna preferito dal team di vendita.

L’utilizzo di un provider SMTP di terze parti è un’ottima opzione per i team di vendita in cui il volume delle e-mail rappresenta la priorità numero uno. I provider SMTP come [!DNL Sendgrid] e [!DNL Sparkpost] sono ottimizzati per soddisfare le esigenze di recapito in blocco di e-mail e possono essere scalati per soddisfare le esigenze di coloro che desiderano distribuire grandi volumi di e-mail.

Inoltre, i provider SMTP di terze parti offrono una serie di funzioni per supportare le esigenze di recapito del team (ad esempio i report di consegna e-mail e gli indirizzi IP dedicati), rendendola un’ottima opzione per chi cerca controlli più granulari e visibilità sul proprio canale di consegna e-mail di vendita.

## Server MSC (legacy) {#msc-servers-legacy}

I server MSC sono disponibili solo per alcuni clienti ToutApp legacy. I clienti vedranno i server MSC disponibili nelle loro impostazioni e-mail. Tutti i clienti non legacy non vedranno MSC come opzione e dovrebbero collegare il proprio account Gmail o [!DNL Outlook] a [!DNL Sales Connect] per sbloccare un canale di consegna.

I server MSC non supportano i metodi di autenticazione DKIM e SPF, che possono ridurre il tasso di recapito messaggi. Per questo motivo, consigliamo a tutti i clienti di connettersi a Gmail o [!DNL Outlook] per ottenere il recapito messaggi migliore.

## Server Marketo {#marketo-servers}

I server di posta elettronica di Marketo non si integrano con [!DNL Sales Connect]. I server Marketo sono ottimizzati per la distribuzione in blocco, in modo da adattarli alle esigenze degli esperti di marketing. Tuttavia, Gmail e [!DNL Exchange] hanno un tasso di successo più alto per le comunicazioni di vendita 1:1, motivo per cui consigliamo di utilizzare questi server per le comunicazioni di vendita.

>[!MORELIKETHIS]
>
>* [Connessione e-mail per utenti Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [Connessione e-mail per [!DNL Outlook] Utenti](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)
>* [Configurazione di un canale di consegna personalizzato](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/setting-up-a-custom-delivery-channel.md)
>* [Limitazione della connessione e-mail](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md)
