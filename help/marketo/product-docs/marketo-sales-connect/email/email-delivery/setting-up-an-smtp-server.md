---
unique-page-id: 14746594
description: Configurazione di un server SMTP - Documenti Marketo - Documentazione del prodotto
title: Configurazione di un server SMTP
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '596'
ht-degree: 0%

---


# Configurazione di un server SMTP {#setting-up-an-smtp-server}

## Panoramica {#overview}

**Che cos&#39;è un server SMTP?**

**** Simple  **** Mail  **** Transfer  **** Protocol, questo è il server responsabile per l&#39;invio della posta in uscita. Quando si invia un&#39;e-mail dal client di posta elettronica, si utilizza lo stesso servizio per inviare l&#39;e-mail.

**Perché è necessario configurare il server SMTP con Sales Connect?**

Consente di utilizzare la reputazione del dominio e della recapito della tua azienda e di non dover fare affidamento su altri. I nostri server MSC predefiniti fanno parte di un pool IP condiviso, il che significa inviare da una reputazione condivisa. È consigliabile che il team configuri il proprio canale di distribuzione con Sales Connect.

**Come vengono inviati i servizi di vendita con il server SMTP?**

Seguendo [questi passaggi](http://docs.marketo.com/x/ZgPh).

![](assets/1.png)

`<pre><em>SMTP Server Setup Page in Sales Connect</em><br> </pre>` **Devo configurare qualcosa nel mio client e-mail?**

Per quanto riguarda il canale di consegna, no. Una volta installato il componente aggiuntivo, Sales Connect utilizzerà lo stesso canale di distribuzione configurato per l&#39;invio di e-mail.

## Ottenimento delle credenziali SMTP {#getting-the-smtp-credentials}

**Come posso ottenere le mie credenziali SMTP?**

Contattate il team IT per scoprire il canale di distribuzione utilizzato dalla società per inviare e-mail e come accedere alle credenziali SMTP. A seconda della configurazione del server, potrebbero essere disponibili alcuni valori personalizzati per il nome del server SMTP o la porta del server. Se non disponete di un team IT dedicato, rivolgetevi al vostro provider di posta elettronica.

**Quali sono le mie opzioni se la mia azienda utilizza Office365?**

Pros

* Configurazione semplice
* Qualsiasi utente con un account Office365 avrà accesso a questo server SMTP

Cons

* Può verificarsi la limitazione
* Ogni utente deve impostarlo autonomamente
* La modifica della password O365 dell&#39;utente comporterà l&#39;interruzione della connessione

Se si utilizza Office365 o Exchange Online, è possibile connettersi al server SMTP utilizzando un set standard di credenziali. Tenete presente che Office365 non è un servizio di consegna di posta elettronica di massa, anche se questo funzionerà bene per l&#39;invio di e-mail una tantum. Quando si inviano e-mail in massa, Office365 potrebbe limitare le e-mail, il che potrebbe causare errori di consegna. Per ulteriori informazioni su questo articolo di Microsoft su [come impostare l&#39;invio del client SMTP](http://support.office.com/en-us/article/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-office-365-69f58e99-c550-4274-ad18-c805d654b4c4).
`<blockquote>  <p>“You can only send from one email address unless your device can store login credentials for multiple Office 365 mailboxes. Office 365 imposes a limit of 30 messages sent per minute, and a limit of 10,000 recipients per day.”</p> </blockquote>`\
Se decidi di utilizzare Office365 come canale di consegna, dovrai immettere queste credenziali. Impossibile utilizzare le stesse credenziali in tutto il team perché Office 365 utilizza l&#39;e-mail e la password dell&#39;utente per connettersi.

Microsoft e invio in blocco

[Fare clic ](http://technet.microsoft.com/en-us/library/exchange-online-limits.aspx#RecipientLimits) qui per informazioni sull&#39;invio in massa in Office365. 
`<blockquote>  <p>“Exchange Online customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.”</p> </blockquote>`\
**E se la mia azienda utilizzasse Gmail?**

Non sarà necessario ottenere credenziali SMTP se il team desidera utilizzare Gmail come canale di consegna con Sales Connect. Sales Connect consente agli utenti di accedere al proprio canale di distribuzione Gmail tramite la nostra integrazione OAuth. Gli utenti possono attivarlo integrando il proprio account di vendita Connect con Gmail.

![](assets/2.png)

**Posso condividere le stesse credenziali SMTP con l&#39;intero team?**

Questo dipende dal canale di consegna che utilizzate. Ad esempio, servizi come Sparkpost consentono che le credenziali siano basate su dominio, in modo che chiunque invii con un dominio specifico venga autenticato per inviarle tramite tale server. In tal caso, potete condividere le credenziali con il team.

Se vi state connettendo a Office365, le credenziali sono basate sull&#39;indirizzo e-mail. Ciò significa che solo l&#39;indirizzo e-mail che ha stabilito la connessione sarà autenticato per inviare e-mail attraverso quel canale di consegna, pertanto le credenziali devono **non** essere condivise.

![](assets/3.png)

