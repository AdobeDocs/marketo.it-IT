---
unique-page-id: 4720433
description: Configurare i protocolli per Marketo - Documentazione Marketo - Documentazione del prodotto
title: Configurare i protocolli per Marketo
exl-id: cf2fd4ac-9229-4e52-bb68-5732b44920ef
source-git-commit: 3d29cb4cf4af7d83a82d47cfd6b0c44d659ee82b
workflow-type: tm+mt
source-wordcount: '1046'
ht-degree: 2%

---

# Configurare i protocolli per Marketo {#configure-protocols-for-marketo}

Se l’utente o l’organizzazione utilizza impostazioni del firewall o del server proxy restrittive, o l’amministratore di rete può dover inserire nell&#39;elenco Consentiti alcuni domini e intervalli di indirizzi IP per garantire che Adobe Marketo Engage funzioni come previsto.

## Pagine di destinazione ed e-mail con brand Campaign {#branded-campaign-landing-pages-and-emails}

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

Aggiungi il CNAME della pagina di destinazione che ti hanno inviato al tuo record DNS in modo che `[YourLandingPageCNAME]` punta alla stringa account univoca assegnata alle pagine di destinazione di Marketo. Accedi al sito del registrar del tuo dominio e immetti la pagina di destinazione CNAME e Account String. In genere, si tratta di tre campi:

* Alias: Invio `[YourLandingPageCNAME]` (fornito dalla commercializzazione)
* Tipo: CNAME
* Punta a: Invio `[MarketoAccountString].mktoweb.com` (fornito dalla commercializzazione)

`2` **Aggiungi CNAME per i collegamenti di tracciamento e-mail**

Aggiungi l’e-mail marketing CNAME inviata, in modo che `[YourEmailCNAME]` punti [MktoTrackingLink], il collegamento di tracciamento predefinito assegnato da Marketo, nel formato:\
`[YourEmailCNAME].[YourDomain].com` IN CNAME `[MktoTrackingLink]`

Ad esempio:

`pages.abc.com IN CNAME mkto-a0244.com`

>[!NOTE]
>
>`[MktoTrackingLink]` deve essere il dominio di branding predefinito.

`3` **Notifica al team di marketing**

Invia una notifica al team di marketing al completamento di questo processo.

`4` **Contatto [Supporto Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target=&quot;_blank&quot;} per avviare il processo di provisioning di un certificato SSL.**

Il completamento di questo processo può richiedere fino a 3 giorni lavorativi.

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

Alcuni sistemi anti-spam utilizzano il campo Email Return-Path invece dell&#39;indirizzo IP per l&#39;autorizzazione. In questi casi, l&#39;approccio migliore è quello di inserire nell&#39;elenco Consentiti &quot;&#42;.mktomail.com&#39;, in quanto Marketo utilizza diversi sottodomini di cassette postali. Altri sistemi anti-spam inserire nell&#39;elenco Consentiti in base all&#39;indirizzo Da. In queste situazioni, accertati di includere tutti i domini di invio (&quot;Da&quot;) utilizzati dal gruppo di marketing per comunicare con persone/lead.

>[!NOTE]
>
>Postini utilizza una tecnologia unica e richiede inserire nell&#39;elenco Consentiti intervalli IP. Vedi [Inserire nell&#39;elenco Consentiti con Postini](https://nation.marketo.com/docs/DOC-1066).

## Passaggio 3: Configurare SPF e DKIM {#step-set-up-spf-and-dkim}

Il team marketing deve aver inviato anche le informazioni DKIM da aggiungere al record di risorse DNS (anch’esso elencato di seguito). Segui i passaggi per configurare correttamente DKIM e SPF, quindi notifica al team di marketing che questo è stato aggiornato.

1. Per impostare SPF, aggiungi la seguente riga alle voci DNS:

   `[CompanyDomain]` IN TXT v=spf1 mx ip4:`[CorpIP]`\
   include: mktomail.com ~all

   Se nella voce DNS è già presente un record SPF, è sufficiente aggiungere quanto segue:\
   include: mktomail.com

   Sostituisci CompanyDomain con il dominio principale del tuo sito web (ad esempio: &quot;`(company.com/)`&quot;) e CorpIP con l&#39;indirizzo IP del server e-mail aziendale (ad es. &quot;255.255.255.255&quot;). Se desideri inviare e-mail da più domini tramite Marketo, devi far aggiungere questa riga al tuo personale IT per ogni dominio (su una riga).

1. Per DKIM, crea record di risorse DNS per ogni dominio che desideri impostare. Di seguito sono riportati i record host e i valori TXT per ogni dominio per cui firmeremo:

   `[DKIMDomain1]`: Record host `[HostRecord1]` e il valore TXT è `[TXTValue1]`.

   `[DKIMDomain2]`: Record host `[HostRecord2]` e il valore TXT è `[TXTValue2]`.

   Copia HostRecord e TXTVvalue per ogni dominio DKIMD configurato dopo aver seguito il [istruzioni qui](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target=&quot;_blank&quot;}. Non dimenticare di verificare ogni dominio in Amministratore > E-mail > DKIM dopo che il tuo personale IT ha completato questo passaggio.

## Passaggio 4: Configurare i record MX per il dominio {#step-set-up-mx-records-for-your-domain}

Un record MX ti consente di ricevere la posta al dominio da cui invii l’e-mail per elaborare le risposte e rispondere automaticamente. Se invii dal dominio aziendale, probabilmente questo è già configurato. In caso contrario, in genere puoi configurarlo per eseguire il mapping al record MX del dominio aziendale.

## Indirizzi IP in uscita {#outbound-ip-addresses}

Una connessione in uscita è una effettuata dal Marketo Engage a un server su Internet per tuo conto. Alcuni partner/fornitori con cui si lavora o una propria organizzazione IT possono utilizzare inseriti nell&#39;elenco Consentiti per limitare l’accesso ai server. In tal caso, devi fornire loro blocchi di indirizzi IP in uscita Marketi Engage da aggiungere ai loro inserire nell&#39;elenco Consentiti.

**Webhook**

Marketo Engage [Webhook](/help/marketo/product-docs/administration/additional-integrations/create-a-webhook.md){target=&quot;_blank&quot;} è un meccanismo di integrazione in uscita. Quando un [Chiama Webhook](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/call-webhook.md)L&#39;azione di flusso {target=&quot;_blank&quot;} viene eseguita come parte di una campagna avanzata. Viene effettuata una richiesta HTTP a un servizio Web esterno. Se l’autore del servizio Web utilizza un inserì nell&#39;elenco Consentiti sul firewall della rete in cui si trova il servizio Web esterno, l’editore deve aggiungere al proprio inserire nell&#39;elenco Consentiti i blocchi di indirizzi IP elencati di seguito.

**Sincronizzazione CRM**

Marketo Engage [Sincronizzazione CRM Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/add-an-existing-salesforce-field-to-the-marketo-sync.md){target=&quot;_blank&quot;} e [Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md){target=&quot;_blank&quot;} sono meccanismi di integrazione che eseguono richieste HTTP in uscita alle API pubblicate dal fornitore di gestione delle relazioni con i clienti. Devi assicurarti che la tua organizzazione IT non blocchi nessuno dei blocchi di indirizzi IP qui sotto dall’accesso alle API del tuo fornitore di gestione delle relazioni con i clienti.

**Marketo Engage blocchi di indirizzi IP in uscita**

Le tabelle seguenti coprono tutti i server di Marketo Engage che eseguono chiamate in uscita. Utilizzare gli elenchi riportati di seguito se si configura un inserire nell&#39;elenco Consentiti IP, un server, un firewall, un elenco di controllo degli accessi, un gruppo di sicurezza o un servizio di terze parti per la ricezione di connessioni in uscita dal Marketo Engage.

<table>
 <tbody>
  <tr>
   <th>Blocco IP (notazione CIDR)</th>
  </tr>
  <tr>
   <td>192.28.144.0/20</td>
  </tr>
   <tr>
   <td>192.28.160.0/19</td>
  </tr>
   <tr>
   <td>199.15.212.0/22</td>
  </tr>
   <tr>
   <td>185.28.196.0/22</td>
  </tr>
   <tr>
   <td>130.248.172.0/24</td>
  </tr>
   <tr>
   <td>130.248.173.0/24</td>
  </tr>
  <tr>
   <td>103.237.104.0/22</td>
  </tr>
  <tr>
   <td>94.236.119.0/26</td>
  </tr>
 </tbody>
</table>

<table>
 <tbody>
  <tr>
   <th>Indirizzo IP individuale</th>
  </tr>
  <tr>
   <td>54.212.167.17</td>
  </tr>
   <tr>
   <td>44.235.171.179</td>
  </tr>
   <tr>
   <td>35.165.244.220</td>
  </tr>
   <tr>
   <td>52.20.211.99</td>
  </tr>
   <tr>
   <td>54.237.141.197</td>
  </tr>
  <tr>
   <td>54.160.246.246</td>
  </tr>
   <tr>
   <td>18.200.201.81</td>
  </tr>
  <tr>
   <td>34.247.24.245</td>
  </tr>
   <tr>
   <td>54.220.138.65</td>
  </tr>
  <tr>
   <td>13.237.155.207</td>
  </tr>
   <tr>
   <td>13.55.192.247</td>
  </tr>
  <tr>
   <td>52.64.109.86</td>
  </tr>
 </tbody>
</table>

