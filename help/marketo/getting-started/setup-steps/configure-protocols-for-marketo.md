---
unique-page-id: 4720433
description: Configurare i protocolli per Marketo - Documentazione Marketo - Documentazione del prodotto
title: Configurare i protocolli per Marketo
exl-id: cf2fd4ac-9229-4e52-bb68-5732b44920ef
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '712'
ht-degree: 1%

---

# Configurare i protocolli per Marketo {#configure-protocols-for-marketo}

Il gruppo di marketing utilizza Marketo per creare pagine di destinazione ed e-mail con brand per campagne. Per garantire il funzionamento di queste pagine di destinazione ed e-mail, è necessario un piccolo aiuto da parte dell’IT. Configura i seguenti protocolli, con le informazioni che il tuo gruppo di marketing ti avrebbe dovuto inviare tramite e-mail.

Questo articolo deve essere condiviso con il reparto IT dell&#39;azienda che desidera implementare questi protocolli.

>[!NOTE]
>
>Se il tuo team IT limita l&#39;accesso web utilizzando un inserire nell&#39;elenco Consentiti, chiedi loro di aggiungere i seguenti domini (incluso l&#39;asterisco) per consentire tutte le risorse Marketo e i websoket:

* `*.marketo.com`

* `*.marketodesigner.com`

* `*.mktoweb.com`

## Passaggio 1: Creare record DNS per pagine di destinazione e posta elettronica {#step-create-dns-records-for-landing-pages-and-email}

**Tracciamento dei CNAME dei collegamenti**

Il team di marketing dovrebbe averti inviato due richieste per nuovi record CNAME. La prima riguarda gli URL delle pagine di destinazione, in modo che le pagine di destinazione vengano visualizzate negli URL che riflettono il dominio e non in Marketo (l’host effettivo). Il secondo riguarda i collegamenti di tracciamento inclusi nelle e-mail inviate da Marketo.

`1` **Aggiungi CNAME per pagine di destinazione**

Aggiungi il CNAME della pagina di destinazione che ti ha inviato al record DNS, in modo che `[YourLandingPageCNAME]` punti alla stringa account univoca assegnata alle pagine di destinazione di Marketo. Accedi al sito del registrar del tuo dominio e immetti la pagina di destinazione CNAME e Account String. In genere, si tratta di tre campi:

* Alias: Inserisci `[YourLandingPageCNAME]` (fornito dal marketing)
* Tipo: CNAME
* Punta a: Inserisci `[MarketoAccountString].mktoweb.com` (fornito dal marketing)

`2` **Aggiungi CNAME per i collegamenti di tracciamento e-mail**

Aggiungi il marketing CNAME dell&#39;e-mail che ti ha inviato, in modo che `[YourEmailCNAME]` punti a [MktoTrackingLink], il collegamento di tracciamento predefinito assegnato da Marketo, nel formato:\
`[YourEmailCNAME].[YourDomain].com` IN CNAME  `[MktoTrackingLink]`

Ad esempio:

`pages.abc.com IN CNAME mkto-a0244.com`

`3` **Notifica al team di marketing**

Notifica al team di marketing al completamento di questo processo.

## Passaggio 2: Inserire nell&#39;elenco Consentiti IP Marketo {#step-allowlist-marketo-ips}

Quando il gruppo di marketing utilizza Marketo per inviare e-mail di test (una best practice prima di inviare esplosioni e-mail), le e-mail di test vengono talvolta bloccate dai sistemi anti-spam che si basano sugli indirizzi IP del mittente per verificare che l’e-mail sia valida. Per assicurare che tali e-mail di test arrivino, aggiungi Marketo al tuo inserire nell&#39;elenco Consentiti.

Aggiungi questi indirizzi IP al tuo inserire nell&#39;elenco Consentiti aziendale:

199.15.212.0/22\
192.28.144.0/20
192.28.160.0/19\
185.28.196.0/22\
130.248.172.0/24\
130.248.173.0/24\
103.237.104.0/22\
94.236.119.0/26

Alcuni sistemi anti-spam utilizzano il campo Email Return-Path invece dell&#39;indirizzo IP per l&#39;autorizzazione. In questi casi, l’approccio migliore è quello di inserire nell&#39;elenco Consentiti ‘*.mktomail.com’, in quanto Marketo utilizza diversi sottodomini di cassette postali. Altri sistemi anti-spam inserire nell&#39;elenco Consentiti in base all&#39;indirizzo Da. In queste situazioni, assicurati di includere tutti i domini di invio (&quot;Da&quot;) utilizzati dal tuo gruppo di marketing per comunicare con persone/lead.

>[!NOTE]
>
>Postini utilizza una tecnologia unica e richiede inserire nell&#39;elenco Consentiti intervalli IP. Vedi [Inserire nell&#39;elenco Consentiti con Postini](https://nation.marketo.com/docs/DOC-1066).

## Passaggio 3: Impostare SPF e DKIM {#step-set-up-spf-and-dkim}

Il team di marketing deve aver inviato anche le informazioni DKIM da aggiungere al record di risorse DNS (anch’esso elencato di seguito). Segui i passaggi per configurare correttamente DKIM e SPF, quindi notifica al team di marketing che questo è stato aggiornato.

1. Per impostare SPF, aggiungi la seguente riga alle voci DNS:

   `[CompanyDomain]` IN TXT v=spf1 mx ip4:`[CorpIP]`\
   include: mktomail.com ~all

   Se nella voce DNS è già presente un record SPF, è sufficiente aggiungere quanto segue:\
   include: mktomail.com

   Sostituisci CompanyDomain con il dominio principale del tuo sito web (ad esempio: &quot;`(company.com/)`&quot;) e CorpIP con l&#39;indirizzo IP del server e-mail aziendale (ad esempio. &quot;255.255.255.255&quot;). Se desideri inviare e-mail da più domini tramite Marketo, devi far aggiungere questa riga al tuo personale IT per ogni dominio (su una riga).

1. Per DKIM, crea record di risorse DNS per ogni dominio che desideri impostare. Di seguito sono riportati i record host e i valori TXT per ogni dominio per cui firmeremo:

   `[DKIMDomain1]`: Il record host è  `[HostRecord1]` e il valore TXT è  `[TXTValue1]`.

   `[DKIMDomain2]`: Il record host è  `[HostRecord2]` e il valore TXT è  `[TXTValue2]`.

   Copia HostRecord e TXTVvalue per ogni DKIMDomain configurato dopo aver seguito le [istruzioni qui](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md). Non dimenticare di verificare ogni dominio in Amministratore > E-mail > DKIM dopo che il tuo personale IT ha completato questo passaggio.

## Passaggio 4: Configurare i record MX per il dominio {#step-set-up-mx-records-for-your-domain}

Un record MX ti consente di ricevere la posta al dominio da cui invii l’e-mail per elaborare le risposte e rispondere automaticamente. Se invii dal dominio aziendale, probabilmente questo è già configurato. In caso contrario, in genere puoi configurarlo per eseguire il mapping al record MX del dominio aziendale.
