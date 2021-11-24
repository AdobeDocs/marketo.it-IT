---
description: Panoramica del canale di consegna - Documenti Marketo - Documentazione del prodotto
title: Panoramica del canale di consegna
hide: true
hidefromtoc: true
source-git-commit: 3b7cc0c855221f6fd0fba6dca08ccbe361ca9758
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 0%

---

# Panoramica del canale di consegna {#delivery-channel-overview}

Marketo Sales offre diverse opzioni per inviare e-mail. Questo articolo esaminerà i canali di consegna che puoi sfruttare, come selezionarli e quando sceglierli tra loro.

## Consigliato: Gmail o Exchange tramite connessione e-mail {#recommended-gmail-or-exchange-via-email-connection}

Le vendite di Marketo consentono una configurazione semplificata e una migliore consegna tramite il nostro servizio Email Connection. La connessione e-mail consente a ogni utente di connettersi ai propri [Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md) o [Exchange](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md) account per Marketo Sales da utilizzare come canale di consegna preferito per tutte le e-mail di vendita Marketo.

L&#39;utilizzo di Gmail o Exchange presenta alcuni vantaggi rispetto ad altre opzioni di canale di consegna:

* Si tratta di un canale di consegna collaudato con una reputazione consolidata che contribuisce a mantenere alto il recapito dei messaggi.
* I metodi di autenticazione come SPF e DKIM sono già configurati e gestiti dal team IT, quindi non è disponibile alcuna configurazione aggiuntiva.
* L’invio di e-mail all’interno di una determinata rete e-mail (ad esempio, l’invio di un’e-mail come utente di Exchange a un’azienda che riceve e-mail tramite Exchange) può contribuire ad aumentare ulteriormente il recapito messaggi.

È importante notare che questi canali di consegna hanno i propri limiti di invio che vengono applicati da Microsoft e Google. Per combatterlo, utilizziamo un meccanismo di limitazione per aiutare gli utenti a rimanere entro questi limiti. Ulteriori informazioni [limitazione e-mail](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md).

>[!NOTE]
>
>Per impostazione predefinita, il plugin O365 utilizzerà sempre il tuo canale di consegna scambio e il plugin Gmail utilizzerà sempre il tuo canale di consegna Gmail per inviare e-mail dai plugin.

**Tracciamento messaggi non recapitati**: Marketo Sales è in grado di rilevare i messaggi non recapitati per gli utenti di Exchange Online o Gmail rilevando il messaggio non recapitato inviato alla casella in entrata del mittente. Queste notifiche rimbalzate verranno raggruppate nelle notifiche di analisi dei modelli, Campaign Analytics e Live Feed per gli utenti. Il tracciamento non recapitato non è supportato per i clienti Exchange On-Prem.

## Canale di consegna personalizzato tramite SMTP {#custom-delivery-channel-via-smtp}

Marketo Sales offre l&#39;opzione aggiuntiva di collegare un server SMTP di terze parti da utilizzare come canale di consegna preferito del team di vendita.

L&#39;utilizzo di un provider SMTP di terze parti è una grande opzione per i team di vendita in cui il volume di posta elettronica è la priorità numero uno. I provider SMTP come Sendgrid e Sparkpost sono ottimizzati per soddisfare le esigenze di consegna in massa di e-mail e possono essere scalati per soddisfare le esigenze di coloro che cercano di distribuire elevati volumi di e-mail.

Inoltre, i fornitori SMTP di terze parti offrono una pletora di funzionalità per aiutare a supportare le esigenze di recapito dei messaggi del tuo team (come i report di consegna delle e-mail e gli indirizzi IP dedicati), rendendo questa una grande opzione per coloro che cercano controlli più granulari e visibilità intorno al proprio canale di consegna delle e-mail di vendita.

## Server di vendita Marketo (legacy) {#marketo-sales-servers-legacy}

I server di vendita Marketo sono disponibili solo per alcuni clienti ToutApp legacy. Questi clienti visualizzeranno i server di vendita Marketo disponibili nelle loro impostazioni e-mail. Tutti i clienti non legacy non vedranno Marketo Sales come opzione e dovrebbero collegare il loro account Gmail o Outlook alle vendite Marketo per sbloccare un canale di consegna.

I server di vendita Marketo non supportano i metodi di autenticazione DKIM e SPF, che possono ridurre il tasso di recapito messaggi. Per questo motivo, consigliamo a tutti i clienti di connettersi a Gmail o Outlook per ottenere il miglior recapito messaggi.

## Server Marketo {#marketo-servers}

I server e-mail Marketo non si integrano con le vendite Marketo. I server Marketo sono ottimizzati per la distribuzione in serie e consentono di scalare le risorse in base alle esigenze degli addetti al marketing. Tuttavia, Gmail e Exchange hanno un tasso di successo più elevato per le comunicazioni di vendita 1:1, motivo per cui si consiglia di utilizzare questi server per le comunicazioni di vendita.

>[!MORELIKETHIS]
>
>* [Connessione e-mail per utenti Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [Connessione e-mail per utenti di Outlook](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)
>* [Impostazione di un canale di consegna personalizzato](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/setting-up-a-custom-delivery-channel.md)
>* [Limitazione connessione e-mail](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md)

