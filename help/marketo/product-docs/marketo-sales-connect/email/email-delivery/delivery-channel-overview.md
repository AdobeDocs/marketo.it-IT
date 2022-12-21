---
unique-page-id: 14352407
description: Panoramica del canale di consegna - Documenti Marketo - Documentazione del prodotto
title: Panoramica del canale di consegna
exl-id: 432bad1e-4eaf-4be8-b856-be364c44816e
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 0%

---

# Panoramica del canale di consegna {#delivery-channel-overview}

Marketo Sales Connect offre diverse opzioni per la consegna delle e-mail. Questo articolo esaminerà i canali di consegna che puoi sfruttare, come selezionarli e quando sceglierli tra loro.

## Consigliato: Gmail o Exchange tramite connessione e-mail {#recommended-gmail-or-exchange-via-email-connection}

Sales Connect consente una configurazione semplificata e un miglioramento del recapito messaggi attraverso il nostro servizio Email Connection. La connessione e-mail consente a ogni utente di connettersi ai propri [Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md) o [Exchange](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md) account a Sales Connect da utilizzare come canale di consegna scelto per tutte le e-mail di Sales Connect.

L&#39;utilizzo di Gmail o Exchange presenta alcuni vantaggi rispetto ad altre opzioni di canale di consegna:

* Si tratta di un canale di consegna collaudato con una reputazione consolidata che contribuisce a mantenere alto il recapito dei messaggi.
* I metodi di autenticazione come SPF e DKIM sono già configurati e gestiti dal team IT, quindi non è disponibile alcuna configurazione aggiuntiva.
* L’invio di e-mail all’interno di una determinata rete e-mail (ad esempio, l’invio di un’e-mail come utente di Exchange a un’azienda che riceve e-mail tramite Exchange) può contribuire ad aumentare ulteriormente il recapito messaggi.

È importante notare che questi canali di consegna hanno i propri limiti di invio che vengono applicati da Microsoft e Google. Per combatterlo, utilizziamo un meccanismo di limitazione per aiutare gli utenti a rimanere entro questi limiti. Ulteriori informazioni [limitazione e-mail](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md).

>[!NOTE]
>
>Per impostazione predefinita, il plugin O365 utilizzerà sempre il tuo canale di consegna scambio e il plugin Gmail utilizzerà sempre il tuo canale di consegna Gmail per inviare e-mail dai plugin.

**Tracciamento messaggi non recapitati**: MSC è in grado di rilevare i messaggi non recapitati per gli utenti di Exchange Online o Gmail rilevando il messaggio non recapitato inviato alla casella in entrata del mittente. Queste notifiche rimbalzate verranno raggruppate nelle notifiche di analisi dei modelli, Campaign Analytics e Live Feed per gli utenti. Il tracciamento non recapitato non è supportato per i clienti Exchange On-Prem.

## Canale di consegna personalizzato tramite SMTP {#custom-delivery-channel-via-smtp}

Sales Connect offre l&#39;opzione aggiuntiva di collegare un server SMTP di terze parti da utilizzare come canale di consegna preferito del team di vendita.

L&#39;utilizzo di un provider SMTP di terze parti è una grande opzione per i team di vendita in cui il volume di posta elettronica è la priorità numero uno. I provider SMTP come Sendgrid e Sparkpost sono ottimizzati per soddisfare le esigenze di consegna in massa di e-mail e possono essere scalati per soddisfare le esigenze di coloro che cercano di distribuire elevati volumi di e-mail.

Inoltre, i fornitori SMTP di terze parti offrono una pletora di funzionalità per aiutare a supportare le esigenze di recapito dei messaggi del tuo team (come i report di consegna delle e-mail e gli indirizzi IP dedicati), rendendo questa una grande opzione per coloro che cercano controlli più granulari e visibilità intorno al proprio canale di consegna delle e-mail di vendita.

## Server MSC (Legacy) {#msc-servers-legacy}

I server MSC sono disponibili solo per alcuni clienti ToutApp legacy. Questi clienti visualizzeranno i server MSC disponibili nelle loro impostazioni e-mail. Tutti i clienti non legacy non vedranno MSC come opzione e dovrebbero collegare il proprio account Gmail o Outlook a Vendite Connetti per sbloccare un canale di consegna.

I server MSC non supportano i metodi di autenticazione DKIM e SPF, che possono ridurre il tasso di recapito messaggi. Per questo motivo, consigliamo a tutti i clienti di connettersi a Gmail o Outlook per ottenere il miglior recapito messaggi.

## Server Marketo {#marketo-servers}

I server e-mail Marketo non si integrano con Sales Connect. I server Marketo sono ottimizzati per la distribuzione in serie e consentono di scalare le risorse in base alle esigenze degli addetti al marketing. Tuttavia, Gmail e Exchange hanno un tasso di successo più elevato per le comunicazioni di vendita 1:1, motivo per cui si consiglia di utilizzare questi server per le comunicazioni di vendita.

>[!MORELIKETHIS]
>
>* [Connessione e-mail per utenti Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [Connessione e-mail per utenti di Outlook](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)
>* [Impostazione di un canale di consegna personalizzato](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/setting-up-a-custom-delivery-channel.md)
>* [Limitazione connessione e-mail](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/email-connection-throttling.md)

