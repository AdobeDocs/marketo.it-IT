---
description: Limitazione della connessione e-mail - Documentazione di Marketo - Documentazione del prodotto
title: Limitazione della connessione e-mail
exl-id: 093f5459-1bbb-45dd-8590-71ea4e1168d4
feature: Marketo Sales Connect
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---

# Limitazione della connessione e-mail {#email-connection-throttling}

L&#39;integrazione dell&#39;account Sales Connect da inviare tramite i provider di posta elettronica Exchange o Gmail offre una configurazione semplificata e ottimizza la consegna delle e-mail per comunicazioni di vendita 1:1. Tuttavia, per mantenere i sistemi sani e gli account sicuri, Gmail ed Exchange impongono limiti di invio delle e-mail. Tali limiti possono essere aumentati o diminuiti a discrezione dei fornitori.

## Panoramica {#overview}

La limitazione della connessione e-mail consente agli amministratori di Sales Connect di configurare la frequenza di invio delle e-mail quando si utilizza Gmail o Exchange come canale di consegna, in modo che la frequenza con cui le e-mail vengono consegnate al provider del canale di consegna non superi i limiti imposti.

Quando i limiti vengono costantemente superati, a volte questo può essere visto come un comportamento sospetto da parte del provider del canale di consegna, che causa il mancato funzionamento delle e-mail e a volte anche la disabilitazione di un account.

**Note/Elementi di rilievo**

* Attivazione automatica dopo la connessione di un utente a Gmail o Exchange
* Può essere personalizzato se desideri aumentare o diminuire le impostazioni da consigli per soddisfare le tue esigenze
* Limita le e-mail inviate tramite Gmail o Exchange, non limita il canale di consegna personalizzato
* La limitazione della connessione e-mail mette in coda ogni singolo utente e-mail separatamente, in quanto ogni utente dispone di una propria connessione con il proprio provider e-mail

**Configurazione delle impostazioni di limitazione della connessione e-mail**

1. Fai clic sull’icona a forma di ingranaggio e seleziona **Impostazioni**.

   ![](assets/email-connection-throttling-1.png)

1. Clic **Generale**.

   ![](assets/email-connection-throttling-2.png)

1. Nella scheda Limitazione connessione e-mail, inserisci la dimensione batch desiderata delle e-mail che verranno inviate al provider del canale e-mail.

   ![](assets/email-connection-throttling-3.png)

1. Imposta il tempo di attesa prima dell’invio di ciascun batch. In questo esempio scegliamo 25 e-mail ogni 45 secondi.

   ![](assets/email-connection-throttling-4.png)

1. Clic **Salva**.

   ![](assets/email-connection-throttling-5.png)

Con le modifiche salvate, tutti gli utenti riceveranno le e-mail inviate in batch al proprio account Gmail o Exchange connesso per la consegna.

## Limiti provider e-mail {#email-provider-limits}

**Outlook 365**

Aziende/Aziende

* 10.000 al giorno
* 30 al minuto
* 500 destinatari per e-mail

Ulteriori informazioni [si trova qui](https://docs.microsoft.com/en-us/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#RecipientLimits).

**Gmail**

* 2000 al giorno (500 per gli account di prova e contrassegnati)
* 2 e-mail al secondo (limite API)
* 2.000 destinatari per messaggio (massimo 500 per i destinatari esterni)

Ulteriori informazioni [si trova qui](https://support.google.com/a/answer/166852?hl=en).

**Microsoft Exchange Server (2010, 2013)**

I limiti sono impostati dal reparto IT dell’organizzazione in quanto il server è ospitato dall’organizzazione. Per ulteriori informazioni, contattare l&#39;amministratore di rete o di sistema.

>[!MORELIKETHIS]
>
>* [Panoramica del canale di consegna](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/delivery-channel-overview.md)
>* [Connessione e-mail per utenti Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [Connessione e-mail per gli utenti di Outlook](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)
