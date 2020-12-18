---
unique-page-id: 14352600
description: Come configurare il server SMTP di Outlook365 con il servizio di vendita Connect - Documenti Marketo - Documentazione del prodotto
title: Come configurare il server SMTP di Outlook365 con Connect di vendita
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---


# Come impostare il server SMTP di Outlook365 con il servizio di vendita {#how-to-set-up-your-outlook-smtp-server-with-sales-connect}

>[!NOTE]
>
>Se l&#39;azienda utilizza Outlook e si sta tentando di configurare un canale di consegna e-mail con Marketo Sales Connect, si consiglia di connettersi al server Exchange [utilizzando la funzionalità di connessione e-mail](http://docs.marketo.com/x/Z4AOAQ).

Per impostare un server [SMTP](http://docs.marketo.com/x/zYTS) personalizzato come canale di consegna alternativo, ToutApp richiede l&#39;utilizzo di una qualche forma di autenticazione a scopo di sicurezza. È possibile configurare qualsiasi server SMTP nella [pagina di configurazione SMTP](http://toutapp.com/next#settings/email-servers/smtp/configure). Per configurare un server SMTP di Office365, Microsoft consiglia la configurazione seguente:\
**Server** SMTP: smtp.office365.com\
**Porta** server: Porta 587 - Protetto\
**Metodo** di autenticazione: Login (SSL/TLS)\
**Nome utente o login**: l&#39;indirizzo e-mail di Office365\
**Password**: password e-mail di Office365\
**Il tuo dominio**: dominio della tua società

Se riscontri ancora problemi durante la configurazione del server SMTP, collabora con l&#39;amministratore di Exchange per assicurarsi che vengano utilizzate le credenziali corrette.

>[!NOTE]
>
>Durante l&#39;invio tramite Office365 SMTP, Microsoft impone un `limit of 30 messages sent per minute` e un limite di 10.000 destinatari al giorno. Inoltre, `each member` del team che desidera inviare le e-mail tramite il server SMTP di Office365 dovrà impostare questa impostazione con il proprio indirizzo e-mail e la propria password nelle impostazioni di Sales Connect. Selezionando la casella per l&#39;impostazione &quot; `Make this deliverability channel to all my team members` `" will not work` per questa configurazione, in conformità ai criteri dell&#39;account Microsoft Office365.

