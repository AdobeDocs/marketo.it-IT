---
unique-page-id: 4720433
description: Configurare i protocolli per Marketo - Marketo Docs - Documentazione prodotto
title: Configurare i protocolli per Marketo
translation-type: tm+mt
source-git-commit: 0ec525defbefe610f0bd1227b1c8f8e125d8e362
workflow-type: tm+mt
source-wordcount: '712'
ht-degree: 1%

---


# Configurare i protocolli per Marketo {#configure-protocols-for-marketo}

Il gruppo di marketing utilizza Marketo per creare pagine di destinazione e e-mail con il logo aziendale. Per garantire il funzionamento di queste pagine di destinazione e delle e-mail, è necessario un piccolo aiuto da parte dell&#39;IT. Configurate i seguenti protocolli, con le informazioni che il vostro gruppo di marketing avrebbe dovuto inviarvi tramite e-mail.

Questo articolo deve essere condiviso con il reparto IT della società che desidera implementare questi protocolli.

>[!NOTE]
>
>Se il team IT limita l&#39;accesso Web utilizzando un inserire nell&#39;elenco Consentiti di , chiedi loro di aggiungere i seguenti domini (incluso l&#39;asterisco) per consentire a tutte le risorse e i socket Web di Marketo:

* `*.marketo.com`

* `*.marketodesigner.com`

* `*.mktoweb.com`

## Passaggio 1: Creare record DNS per le pagine di destinazione e le e-mail {#step-create-dns-records-for-landing-pages-and-email}

**Tracciamento dei CNAME di collegamento**

Il team marketing deve averti inviato due richieste per nuovi record CNAME. Il primo riguarda gli URL delle pagine di destinazione, in modo che le pagine di destinazione siano visualizzate negli URL che riflettono il dominio e non in Marketo (l’host effettivo). Il secondo riguarda i collegamenti di tracciamento inclusi nelle e-mail che inviano da Marketo.

`1` **Aggiungi CNAME per pagine di destinazione**

Aggiungete il CNAME della pagina di destinazione che vi hanno inviato al record DNS, in modo che punti `[YourLandingPageCNAME]` alla stringa account univoca assegnata alle pagine di destinazione Marketo. Accedete al sito del registrar del vostro dominio e immettete la pagina di destinazione CNAME e Stringa account. In genere si tratta di tre campi:

* Alias: Invio `[YourLandingPageCNAME]` (fornito da marketing)
* Tipo: CNAME
* Punto a: Invio `[MarketoAccountString].mktoweb.com` (fornito da marketing)

`2` **Aggiungi CNAME per i collegamenti di tracciamento e-mail**

Aggiungi l’e-mail di marketing CNAME inviata, in modo che `[YourEmailCNAME]` punti a [MktoTrackingLink], il collegamento di tracciamento predefinito assegnato da Marketo, nel formato:\
`[YourEmailCNAME].[YourDomain].com` IN CNAME `[MktoTrackingLink]`

Ad esempio:

`pages.abc.com IN CNAME mkto-a0244.com`

`3` **Notifica al team di marketing**

Notifica al team di marketing una volta completata la procedura.

## Passaggio 2:  Inserire nell&#39;elenco Consentiti gli IP Marketo {#step-allowlist-marketo-ips}

Quando il gruppo Marketing utilizza Marketo per inviare e-mail di prova (una procedura consigliata prima dell&#39;invio delle esplosioni), le e-mail di prova talvolta vengono bloccate dai sistemi anti-spam che si affidano agli indirizzi IP del mittente per verificare la validità dell&#39;e-mail. Per garantire l&#39;arrivo di tali e-mail di test, aggiungi Marketo al tuo inserire nell&#39;elenco Consentiti di .

Aggiungi questi indirizzi IP al tuo inserire nell&#39;elenco Consentiti  aziendale:

199.15.212.0/22\
192.28.144.0/20
192.28.160.0/19\
185.28.196.0/22\
130.248.172.0/24\
130.248.173.0/24\
103.237.104.0/22\
94.236.119.0/26

Alcuni sistemi anti-spam utilizzano il campo email Return-Path invece dell&#39;indirizzo IP per l&#39;assegnazione. In questi casi, l&#39;approccio migliore è   &quot;*.mktomail.com&quot;, in quanto Marketo utilizza diversi sottodomini di cassette postali. Altri sistemi anti-spam  inserì nell&#39;elenco Consentiti in base all&#39;indirizzo Da. In queste situazioni, accertatevi di includere tutti i domini di invio (&quot;Da&quot;) usati dal gruppo Marketing per comunicare con persone/lead.

>[!NOTE]
>
>Postini utilizza una tecnologia unica e richiede  intervalli IP inserì nell&#39;elenco Consentiti. Consulta [Inserire nell&#39;elenco Consentiti con Postini](https://nation.marketo.com/docs/DOC-1066).

## Passaggio 3: Configurare SPF e DKIM {#step-set-up-spf-and-dkim}

Il team di marketing deve inoltre aver inviato informazioni DKIM da aggiungere al record di risorse DNS (elencato di seguito). Segui i passaggi per configurare correttamente DKIM e SPF, quindi informa il team di marketing che questo è stato aggiornato.

1. Per configurare SPF, aggiungi la seguente riga alle voci DNS:

   `[CompanyDomain]` IN TXT v=spf1 mx ip4:`[CorpIP]`\
   include: mktomail.com ~all

   Se disponiamo già di un record SPF esistente nella nostra voce DNS, aggiungeteci semplicemente quanto segue:\
   include: mktomail.com

   Sostituisci CompanyDomain con il dominio principale del tuo sito Web (ad esempio: &quot;`(company.com/)`&quot;) e CorpIP con l&#39;indirizzo IP del server e-mail aziendale (ad esempio &quot;255.255.255.255&quot;). Se invierete e-mail da più domini tramite Marketo, è necessario che il personale IT aggiunga questa riga per ciascun dominio (su una sola riga).

1. Per DKIM, crea record di risorse DNS per ogni dominio che desideri impostare. Di seguito sono riportati i record host e i valori TXT per ciascun dominio per il quale verranno firmati:

   `[DKIMDomain1]`: Record host è `[HostRecord1]` e il valore TXT è `[TXTValue1]`.

   `[DKIMDomain2]`: Record host è `[HostRecord2]` e il valore TXT è `[TXTValue2]`.

   Copiate HostRecord e TXTVvalue per ogni DKIMDomain configurato dopo aver seguito le [istruzioni riportate qui](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md). Non dimenticare di verificare ogni dominio in Admin (Amministratore) > Email (E-mail) > DKIM dopo che il personale IT ha completato questo passaggio.

## Passaggio 4: Configurare i record MX per il dominio {#step-set-up-mx-records-for-your-domain}

Un record MX consente di ricevere la posta al dominio da cui si invia l&#39;e-mail per elaborare le risposte e rispondere automaticamente. Se invii dal dominio aziendale, probabilmente hai già configurato questo. In caso contrario, potete in genere configurarlo per la mappatura al record MX del vostro dominio aziendale.
