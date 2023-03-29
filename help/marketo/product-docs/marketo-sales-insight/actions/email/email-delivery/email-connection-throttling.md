---
description: Limitazione della connessione e-mail - Documenti Marketo - Documentazione del prodotto
title: Limitazione connessione e-mail
exl-id: 02450a1e-5b30-4057-b204-19fab1a7d6c9
source-git-commit: 88c4e844f7ce26b12bae8177dd5311813fb4adcb
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 0%

---

# Limitazione connessione e-mail {#email-connection-throttling}

L&#39;integrazione dell&#39;account Sales Connect per l&#39;invio tramite i provider di posta elettronica Exchange o Gmail offre una configurazione semplificata e ottimizza il recapito dei messaggi e-mail per le comunicazioni di vendita 1:1. Tuttavia, per mantenere i sistemi sani e gli account sicuri, Gmail e Exchange impongono limiti di invio delle e-mail. Tali limiti possono essere aumentati o diminuiti a discrezione dei fornitori.

## Limitazione connessione e-mail (Beta) {#email-connection-throttling-beta}

>[!AVAILABILITY]
>
>Questa funzione è attualmente in versione beta. Per partecipare, contatta il team dell&#39;account Adobe (il tuo Account Manager).

La limitazione della connessione e-mail consente agli amministratori di Sales Connect di configurare il tasso di invio delle e-mail quando si utilizza Gmail o Exchange come canale di consegna, in modo che il tasso di consegna delle e-mail al provider del canale di consegna non superi i limiti imposti.

Quando i limiti vengono costantemente superati, questo può talvolta essere visto come comportamento sospetto dal provider del canale di consegna, causando errori nelle e-mail e talvolta persino un account da disattivare.

**Note/Elementi di rilievo**

* Abilitato automaticamente una volta che un utente si connette a Gmail o Exchange
* Può essere personalizzato se desideri aumentare o diminuire le impostazioni dalla raccomandazione per soddisfare le tue esigenze
* Solo limita le e-mail inviate tramite Gmail o Exchange, non limita per il canale di consegna personalizzato
* La limitazione della connessione e-mail mette in coda ogni singolo utente e-mail separatamente in quanto ogni utente ha la propria connessione con il proprio provider di posta elettronica

**Configurazione delle impostazioni di limitazione della connessione e-mail**

1. Fai clic sull’icona a forma di ingranaggio e seleziona **Impostazioni**.

   ![](assets/email-connection-throttling-1.png)

1. In Impostazioni amministratore, fai clic su **Generale**.

   ![](assets/email-connection-throttling-2.png)

1. Nella scheda Limitazione connessione e-mail a destra, fai clic sul pulsante **Abilita limitazione e-mail** cursore.

   ![](assets/email-connection-throttling-3.png)

1. Nella scheda Limitazione connessione e-mail a destra, immetti la dimensione batch desiderata di e-mail che verranno inviate al provider del canale e-mail.

   ![](assets/email-connection-throttling-4.png)

1. Impostare il tempo di attesa prima dell&#39;invio di ogni batch. In questo esempio scegliamo 25 e-mail ogni 45 secondi.

   ![](assets/email-connection-throttling-5.png)

1. Fai clic su **Salva**.

   ![](assets/email-connection-throttling-6.png)

Con le modifiche salvate, tutti gli utenti riceveranno le e-mail inviate in batch al proprio account Gmail o Exchange connesso per la consegna.

## Limiti per i provider di posta elettronica {#email-provider-limits}

**Outlook 365**

Aziende/aziende

* 10.000 al giorno
* 30 al minuto
* 500 destinatari per e-mail

Ulteriori informazioni [si trova qui](https://docs.microsoft.com/en-us/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#RecipientLimits).

**Gmail**

* 2000 al giorno (500 per conti di prova e con contrassegno)
* 2 e-mail al secondo (limite API)
* 2.000 destinatari per messaggio (massimo 500 destinatari per destinatari esterni)

Ulteriori informazioni [si trova qui](https://support.google.com/a/answer/166852?hl=en).

**Microsoft Exchange Server (2010, 2013)**

I limiti sono impostati dal reparto IT dell&#39;organizzazione in quanto il server è ospitato dall&#39;organizzazione. Per ulteriori informazioni, contattare l&#39;amministratore di rete o di sistema.

>[!MORELIKETHIS]
>
>* [Panoramica del canale di consegna](/help/marketo/product-docs/marketo-sales-connect/email/email-delivery/delivery-channel-overview.md)
>* [Connessione e-mail per utenti Gmail](/help/marketo/product-docs/marketo-sales-connect/email-plugins/gmail/email-connection-for-gmail-users.md)
>* [Connessione e-mail per utenti di Outlook](/help/marketo/product-docs/marketo-sales-connect/email-plugins/msc-for-outlook/email-connection-for-outlook-users.md)

