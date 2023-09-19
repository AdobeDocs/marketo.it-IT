---
unique-page-id: 4720433
description: Configurare i protocolli per Marketo - Documentazione Marketo - Documentazione del prodotto
title: Configurazione dei protocolli per Marketo
exl-id: cf2fd4ac-9229-4e52-bb68-5732b44920ef
feature: Getting Started
source-git-commit: 0d6507c251e2b7567483af8d75158f6bc6a1ca49
workflow-type: tm+mt
source-wordcount: '1028'
ht-degree: 3%

---

# Configurazione dei protocolli per Marketo {#configure-protocols-for-marketo}

Se l&#39;utente o l&#39;organizzazione utilizza impostazioni restrittive per il firewall o il server proxy, potrebbe essere necessario inserire nell&#39;elenco Consentiti alcuni domini e intervalli di indirizzi IP per garantire il corretto funzionamento di Adobe Marketo Engage.

## Pagine di destinazione e e-mail per campagne con marchio {#branded-campaign-landing-pages-and-emails}

Il gruppo marketing utilizza Marketo per creare pagine di destinazione e e-mail per le campagne con marchio. Per garantire il funzionamento di tali pagine di destinazione e e-mail, è necessario un piccolo aiuto da parte dell’IT. Imposta i seguenti protocolli, con le informazioni che il gruppo di marketing ti avrebbe dovuto inviare tramite e-mail.

Questo articolo deve essere condiviso con il reparto IT dell’azienda che desidera implementare questi protocolli.

Se il tuo team IT limita l’accesso web utilizzando un inserisco nell&#39;elenco Consentiti di, chiedi loro di aggiungere i seguenti domini (incluso l’asterisco) per consentire tutte le risorse e i websockets di Marketo:

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`
* `*.experience.adobe.com`
* `*.adobe.net`

## Passaggio 1: creare record DNS per le pagine di destinazione e l’e-mail {#step-create-dns-records-for-landing-pages-and-email}

**Tracciamento dei CNAME dei collegamenti**

Il team marketing avrebbe dovuto inviarti due richieste per nuovi record CNAME. Il primo è per gli URL della pagina di destinazione, in modo che le pagine di destinazione vengano visualizzate in URL che riflettono il dominio e non Marketo (l’host effettivo). La seconda è per i collegamenti di tracciamento inclusi nelle e-mail inviate da Marketo.

`1` **Aggiungi CNAME per le pagine di destinazione**

Aggiungi il CNAME della pagina di destinazione che ti hanno inviato al tuo record DNS, in modo che `[YourLandingPageCNAME]` punta alla stringa account univoca assegnata alle pagine di destinazione di Marketo. Accedi al sito del tuo registrar di dominio e immetti il CNAME della pagina di destinazione e la stringa dell’account. In genere, questo comporta tre campi:

* Alias: Invio `[YourLandingPageCNAME]` (fornito da marketing)
* Tipo: CNAME
* Puntare a: Invio `[MunchkinID].mktoweb.com` (fornito da marketing)

`2` **Aggiungi CNAME per i collegamenti di tracciamento e-mail**

Aggiungi il CNAME e-mail che ti ha inviato il marketing, in modo che `[YourEmailCNAME]` punta a [MktoTrackingLink], il collegamento di tracciamento predefinito assegnato da Marketo, nel formato:\
`[YourEmailCNAME].[YourDomain].com` IN CNAME `[MktoTrackingLink]`

Ad esempio:

`pages.abc.com IN CNAME mkto-a0244.com`

>[!NOTE]
>
>`[MktoTrackingLink]` deve essere il dominio di branding predefinito.

`3` **Notifica al team marketing**

Avvisa il team marketing quando hai completato questo processo.

`4` **Contatto [Supporto Marketo](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} per avviare il processo di provisioning di un certificato SSL.**

Il completamento di questo processo può richiedere fino a 3 giorni lavorativi.

## Passaggio 2: Inserire nell&#39;elenco Consentiti gli IP di Marketo {#step-allowlist-marketo-ips}

Quando il gruppo Marketing utilizza Marketo per inviare e-mail di test (una best practice per evitare l’invio di messaggi esplosivi), a volte le e-mail di test vengono bloccate da sistemi anti-spam che si basano sugli indirizzi IP del mittente per verificare che l’e-mail sia valida. Per assicurarti che le e-mail di test arrivino, aggiungi Marketo al tuo inserisco nell&#39;elenco Consentiti di.

Aggiungi questi indirizzi IP al tuo inserisco nell&#39;elenco Consentiti di aziendale:

94.236.119.0/26

103.237.104.0/22

130.248.172.0/24

130.248.173.0/24

130.248.244.88/29

185.28.196.0/22

192.28.144.0/20

192.28.160.0/19

199.15.212.0/22

Alcuni sistemi anti-spam utilizzano il campo Return-Path (Percorso di ritorno) dell’e-mail invece dell’indirizzo IP per l’inserimento nell’elenco Consentiti. In questi casi, l&#39;approccio migliore è quello di inserire nell&#39;elenco Consentiti il sistema di controllo dell&#39;&quot;.&#42;.mktomail.com’, in quanto Marketo utilizza diversi sottodomini delle caselle postali. Inserire nell&#39;elenco Consentiti Altri sistemi anti-spam si in base all indirizzo Da. In queste situazioni, assicurati di includere tutti i domini di invio (&quot;Da&quot;) utilizzati dal gruppo Marketing per comunicare con persone/lead.

>[!NOTE]
>
>Postini impiega una tecnologia unica e richiede la inserire nell&#39;elenco Consentiti di intervalli IP da parte di. Consulta [Inserire nell&#39;elenco Consentiti con Postini](https://nation.marketo.com/docs/DOC-1066).

## Passaggio 3: configurare SPF e DKIM {#step-set-up-spf-and-dkim}

Il team marketing avrebbe dovuto inviarti anche informazioni DKIM da aggiungere al record di risorse DNS (anch’esso elencato di seguito). Segui i passaggi per configurare correttamente DKIM e SPF, quindi avvisa il team di marketing che l’aggiornamento è stato completato.

1. Per impostare SPF, aggiungi la seguente riga alle voci DNS:

   `[CompanyDomain]` IN TXT v=spf1 mx ip4:`[CorpIP]`\
   include: mktomail.com ~tutti

   Se disponiamo già di un record SPF nella voce DNS, è sufficiente aggiungervi quanto segue:\
   include: mktomail.com

   Sostituisci il dominio dell’azienda con il dominio principale del tuo sito web (ad esempio: &quot;`(company.com/)`&quot;) e CorpIP con l&#39;indirizzo IP del server e-mail aziendale (ad es. &quot;255.255.255.255&quot;). Se intendi inviare e-mail da più domini tramite Marketo, il tuo staff IT dovrebbe aggiungere questa riga per ciascun dominio (su una riga).

1. Per DKIM, crea record di risorse DNS per ogni dominio che desideri impostare. Di seguito sono riportati i record host e i valori TXT per ogni dominio per cui firmeremo:

   `[DKIMDomain1]`: il record host è `[HostRecord1]` e il valore TXT è `[TXTValue1]`.

   `[DKIMDomain2]`: il record host è `[HostRecord2]` e il valore TXT è `[TXTValue2]`.

   Copiare HostRecord e TXTValue per ogni dominio DKIMD configurato dopo aver seguito [istruzioni](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}. Non dimenticare di verificare ogni dominio in Amministratore > E-mail > DKIM dopo che il personale IT ha completato questo passaggio.

## Passaggio 4: configurare i record MX per il dominio {#step-set-up-mx-records-for-your-domain}

Un record MX ti consente di ricevere e-mail al dominio da cui stai inviando l’e-mail per elaborare le risposte e i risponditori automatici. Se invii dal dominio aziendale, probabilmente lo hai già configurato. In caso contrario, in genere è possibile configurarlo per eseguire la mappatura sul record MX del dominio aziendale.

## Indirizzi IP in uscita {#outbound-ip-addresses}

Per connessione in uscita si intende una connessione effettuata dal Marketo Engage a un server su Internet per conto dell&#39;utente. Alcuni partner/fornitori con cui collabori o la tua organizzazione IT possono utilizzare i inserisce nell&#39;elenco Consentiti di accesso ai server di un&#39;organizzazione di produttori di cui si è proprietari, in modo da limitare l&#39;accesso ai server. In tal caso, devi fornire loro blocchi di indirizzi IP in uscita di Marketo Engage da aggiungere ai loro inserisce nell&#39;elenco Consentiti di.

**Webhook**

Marketo Engage [Webhook](/help/marketo/product-docs/administration/additional-integrations/create-a-webhook.md){target="_blank"} are an outbound integration mechanism. When a [Call Webhook](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/call-webhook.md){target="_blank"} azione di flusso eseguita come parte di una campagna intelligente, viene effettuata una richiesta HTTP a un servizio web esterno. Se l’editore del servizio web utilizza un inserisco nell&#39;elenco Consentiti di sul firewall della rete in cui si trova il servizio web esterno, deve aggiungere i blocchi di indirizzi IP elencati di seguito al proprio inserisco nell&#39;elenco Consentiti di.

**Sincronizzazione CRM**

Marketo Engage [Sincronizzazione CRM Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/add-an-existing-salesforce-field-to-the-marketo-sync.md){target="_blank"} and [Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md){target="_blank"} sono meccanismi di integrazione che effettuano richieste HTTP in uscita alle API pubblicate dal fornitore del sistema di gestione delle relazioni con i clienti. È necessario assicurarsi che l’organizzazione IT non blocchi nessuno dei blocchi di indirizzi IP riportati di seguito per l’accesso alle API del fornitore CRM.

**Blocchi di indirizzi IP in uscita del Marketo Engage**

Le tabelle seguenti descrivono tutti i server di Marketo Engage che effettuano chiamate in uscita. Utilizzare gli elenchi riportati di seguito se si sta configurando un elenco Consentiti IP, un server, un firewall, un elenco di controllo di accesso, un gruppo di sicurezza o un servizio di terze parti per ricevere connessioni in uscita dal Marketo Engage.

<table>
 <tbody>
  <tr>
   <th>Blocco IP (notazione CIDR)</th>
  </tr>
  <tr>
   <td>94.236.119.0/26</td>
  </tr>
  <tr>
   <td>103.237.104.0/22</td>
  </tr>
   <tr>
   <td>130.248.172.0/24</td>
  </tr>
   <tr>
   <td>130.248.173.0/24</td>
  </tr>
  <tr>
   <td>130.248.244.88/29</td>
  </tr>
  <tr>
   <td>185.28.196.0/22</td>
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
 </tbody>
</table>

<table>
 <tbody>
  <tr>
   <th>Indirizzo IP individuale</th>
  </tr>
  <tr>
   <td>13.237.155.207</td>
  </tr>
   <tr>
   <td>13.55.192.247</td>
  </tr>
  <tr>
   <td>18.200.201.81</td>
  </tr>
  <tr>
   <td>34.247.24.245</td>
  </tr>
  <tr>
   <td>35.165.244.220</td>
  </tr>
  <tr>
   <td>44.235.171.179</td>
  </tr>
  <tr>
   <td>52.20.211.99</td>
  </tr>
  <tr>
   <td>52.64.109.86</td>
  </tr>
  <tr>
   <td>54.160.246.246</td>
  </tr>
  <tr>
   <td>54.212.167.17</td>
  </tr>
  <tr>
   <td>54.220.138.65</td>
  </tr>
   <tr>
   <td>54.237.141.197</td>
  </tr>
  </tr>
   <tr>
   <td>130.248.168.16</td>
  </tr>
  </tr>
   <tr>
   <td>130.248.168.17</td>
  </tr>

</tbody>
</table>

