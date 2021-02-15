---
unique-page-id: 14352407
description: Panoramica del canale di distribuzione - Documenti Marketo - Documentazione del prodotto
title: Panoramica del canale di distribuzione
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '456'
ht-degree: 0%

---


# Panoramica del canale di consegna {#delivery-channel-overview}

Verranno suddivisi i tre canali che puoi sfruttare, come selezionarli, quando scegliere l&#39;uno sull&#39;altro e le sfumature che li circondano.

>[!NOTE]
>
>Queste informazioni sono pertinenti solo se si inviano e-mail dall&#39; [applicazione Web](https://toutapp.com/login). Se utilizzate Sales Connect in Gmail o Outlook, i vostri messaggi e-mail verranno recapitati tramite tali server di posta elettronica.

## Server e-mail MSC (predefinito) {#msc-email-servers-default}

Per impostazione predefinita, questo metodo viene selezionato per la distribuzione dei messaggi e-mail. I server e-mail MSC sono una grande opzione per gli utenti che non utilizzano Gmail o Outlook. Inoltre, poiché sono i nostri server, abbiamo la possibilità di ricevere qualsiasi messaggio di errore relativo ai rimbalzi o alle consegne non riuscite e di presentarveli nella sezione &quot;Conversazioni non riuscite&quot; della scheda Conversazioni.

Un altro vantaggio dell&#39;utilizzo dei server MSC è che, quando si utilizza un [ID e-mail](/help/marketo/product-docs/marketo-sales-connect/getting-started/email-settings/add-identity.md), il destinatario visualizzerà l&#39;indirizzo e-mail dell&#39;identità creata.

Quando utilizzate i server MSC, i destinatari potrebbero vedere un tag &quot;via toutapp.com&quot;. Questo è il client di posta elettronica che informa l&#39;utente che l&#39;e-mail è stata inviata utilizzando Sales Connect.

Per ulteriori dettagli, consultare questo [articolo della Guida di Gmail](https://support.google.com/mail/answer/1311182?hl=en).

>[!NOTE]
>
>I nostri server MSC non dispongono di un [record DMARC](https://dmarc.org/) che è disponibile. Non possono essere inseriti nella white list dei server.

## Server di posta elettronica {#gmail-server}

Se il provider e-mail della società è Gmail, potete utilizzare l&#39;account esistente per inviare i messaggi e-mail a Sales Connect. Questa è una grande opzione se si desidera evitare le informazioni &quot;via toutapp.com&quot;, e se si preferisce affidarsi alla reputazione del dominio della società e alla sua recapito. Un ulteriore vantaggio dell&#39;utilizzo di un server Gmail è che tutto ciò che si invia dall&#39;applicazione Web verrà automaticamente aggiunto alla cartella di invio Gmail.

Possiamo collegarci correttamente con un solo account Gmail (un indirizzo e-mail) che invierà i messaggi e-mail di vendita Connect. Questo significa che se utilizzate più identità e-mail, verrà visualizzato solo l&#39;indirizzo dell&#39;account a cui siamo connessi quando guardiamo i dettagli.

Nell’applicazione Web, l’identità dell’utente verrà visualizzata come l’avete creata (sopra). Tuttavia, l&#39;invio tramite i server Gmail mostrerà l&#39;indirizzo dell&#39;account connesso.

>[!NOTE]
>
>Poiché Sales Connect non gestisce direttamente i server Gmail, nell’applicazione Web non vengono registrati eventi di e-mail rimbalzate.

## Server SMTP personalizzato {#custom-smtp-server}

Pagare per il proprio server? Utilizzare un ambiente Microsoft Exchange? Questa è un&#39;opzione per voi. Verificare [queste istruzioni](https://docs.marketo.com/x/zYTS) al momento della configurazione. Come i server di posta elettronica, dal momento che Sales Connect non gestisce direttamente il server, nell’applicazione Web non vengono registrati eventi e-mail rimbalzati.
