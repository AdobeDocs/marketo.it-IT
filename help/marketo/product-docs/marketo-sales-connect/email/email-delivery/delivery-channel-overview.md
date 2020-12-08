---
unique-page-id: 14352407
description: Panoramica del canale di distribuzione - Documenti Marketo - Documentazione del prodotto
title: Panoramica del canale di distribuzione
translation-type: tm+mt
source-git-commit: 00887ea53e395bea3a11fd28e0ac98b085ef6ed8
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---


# Panoramica del canale di distribuzione {#delivery-channel-overview}

Verranno suddivisi i tre canali che puoi sfruttare, come selezionarli, quando scegliere l&#39;uno sull&#39;altro e le sfumature che li circondano.

>[!NOTE]
>
>Queste informazioni sono pertinenti solo se inviate le e-mail dall’applicazione [](http://toutapp.com/login)Web. Se utilizzate Sales Connect in Gmail o Outlook, i vostri messaggi e-mail verranno recapitati tramite tali server di posta elettronica.

## Server e-mail MSC (predefinito) {#msc-email-servers-default}

Per impostazione predefinita, questo metodo viene selezionato per la distribuzione dei messaggi e-mail. I server e-mail MSC sono una grande opzione per gli utenti che non utilizzano Gmail o Outlook. Inoltre, poiché sono i nostri server, abbiamo la possibilità di ricevere qualsiasi messaggio di errore relativo ai rimbalzi o alle consegne non riuscite e di presentarveli nella sezione &quot;Conversazioni non riuscite&quot; della scheda Conversazioni.

Un altro vantaggio dell&#39;utilizzo dei server MSC è che, quando si utilizza un&#39;identità [](https://help.toutapp.com/hc/en-us/articles/215371427)e-mail, il destinatario visualizzerà l&#39;indirizzo e-mail dell&#39;identità creata.

Quando utilizzate i server MSC, i destinatari potrebbero vedere un tag &quot;via toutapp.com&quot;. Questo è il client di posta elettronica che informa l&#39;utente che l&#39;e-mail è stata inviata utilizzando Sales Connect.

Per ulteriori dettagli, consultate questo articolo [della guida](https://support.google.com/mail/answer/1311182?hl=en)Gmail.

>[!NOTE]
>
>I nostri server MSC non dispongono di un record [](https://dmarc.org/) DMARC disponibile. Non possono essere inseriti nella white list dei server.

## Gmail Server {#gmail-server}

Se il provider e-mail della società è Gmail, potete utilizzare l&#39;account esistente per inviare i messaggi e-mail a Sales Connect. Questa è una grande opzione se si desidera evitare le informazioni &quot;via toutapp.com&quot;, e se si preferisce affidarsi alla reputazione del dominio della società e alla sua recapito. Un ulteriore vantaggio dell&#39;utilizzo di un server Gmail è che tutto ciò che si invia dall&#39;applicazione Web verrà automaticamente aggiunto alla cartella di invio Gmail.

Possiamo collegarci correttamente con un solo account Gmail (un indirizzo e-mail) che invierà i messaggi e-mail di vendita Connect. Questo significa che se utilizzate più identità e-mail, verrà visualizzato solo l&#39;indirizzo dell&#39;account a cui siamo connessi quando guardiamo i dettagli.

Nell’applicazione Web, l’identità dell’utente verrà visualizzata come l’avete creata (sopra). Tuttavia, l&#39;invio tramite i server Gmail mostrerà l&#39;indirizzo dell&#39;account connesso.

>[!NOTE]
>
>Poiché Sales Connect non gestisce direttamente i server Gmail, nell’applicazione Web non vengono registrati eventi di e-mail rimbalzate.

## Server SMTP personalizzato  {#custom-smtp-server}

Pagare per il proprio server? Utilizzare un ambiente Microsoft Exchange? Questa è un&#39;opzione per voi. Consulta [queste istruzioni](http://docs.marketo.com/x/zYTS) per la configurazione. Come i server di posta elettronica, dal momento che Sales Connect non gestisce direttamente il server, nell’applicazione Web non vengono registrati eventi e-mail rimbalzati.

