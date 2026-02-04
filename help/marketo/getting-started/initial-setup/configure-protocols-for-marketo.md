---
unique-page-id: 4720433
description: Configurare i protocolli per Marketo Engage - Documentazione di Marketo Engage - Documentazione del prodotto
title: Configurare i protocolli per Marketo Engage
exl-id: cf2fd4ac-9229-4e52-bb68-5732b44920ef
feature: Getting Started
source-git-commit: ee8b46179d9fe85c4d5f2ebd7c2d31b7fbf516c3
workflow-type: tm+mt
source-wordcount: '2129'
ht-degree: 100%

---

# Configurare i protocolli per Marketo Engage{#configure-protocols-for-marketo-engage}

Se tu o la tua organizzazione utilizzate impostazioni restrittive per il firewall o il server proxy, tu o l’amministratore della rete potreste dover inserire nell’elenco Consentiti alcuni domini e intervalli di indirizzi IP per garantire il corretto funzionamento di Adobe Marketo Engage.

Per assistenza nell’implementazione dei protocolli riportati di seguito, condividi questo articolo con il tuo reparto IT. Se quest’ultimo limita l’accesso web mediante un elenco di domini consentiti, assicurati che vengano aggiunti i seguenti domini (incluso l’asterisco) affinché le risorse e i websocket di Marketo non vengano bloccati:

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`
* `*.experience.adobe.com`
* `*.adobe.net`

## Passaggio 1: creare record DNS per pagine di destinazione e e-mail {#step-create-dns-records-for-landing-pages-and-email}

**CNAME per i collegamenti di tracciamento**

Dovresti aver ricevuto due richieste dal team marketing per nuovi record CNAME. La prima è per gli URL delle pagine di destinazione, in modo che queste vengano visualizzate in URL che riflettono il tuo dominio e non Marketo Engage (l’host effettivo). La seconda è per i collegamenti di tracciamento inclusi nelle e-mail inviate da Marketo Engage.

`1` **Aggiungere CNAME per le pagine di destinazione**

Aggiungi al record DNS il CNAME delle pagine di destinazione che ti è stato inviato, in modo che `[YourLandingPageCNAME]` punti alla stringa account univoca assegnata alle pagine di destinazione Marketo Engage. Accedi al sito del fornitore di servizi di registrazione del tuo dominio e inserisci il CNAME delle pagine di destinazione e la stringa account. In genere, questo comporta tre campi:

* Alias: inserisci `[YourLandingPageCNAME]` (che ti è stato fornito dal marketing)
* Tipo: CNAME
* Punta a: inserisci `[MunchkinID].mktoweb.com` (che ti è stato fornito dal marketing)

`2` **Aggiungere CNAME per i collegamenti di tracciamento delle e-mail**

Aggiungi il CNAME per le e-mail che ti è stato inviato dal marketing, in modo che `[YourEmailCNAME]` punti a [MktoTrackingLink], il collegamento di tracciamento predefinito assegnato da Marketo Engage, nel formato:
`[YourEmailCNAME].[YourDomain].com` IN CNAME `[MktoTrackingLink]`

Ad esempio:

`pages.abc.com IN CNAME mkto-a0244.com`

>[!NOTE]
>
>`[MktoTrackingLink]` deve essere il dominio di branding predefinito.

`3` **Avvisare il team marketing**

Una volta completato questo processo, avvisa il team marketing.

`4` **Contatta l’[assistenza Adobe](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} per avviare il processo di provisioning di un certificato SSL.**

Questo processo può richiedere fino a tre giorni lavorativi.

## Passaggio 2: inserire gli IP di Marketo Engage nell’elenco Consentiti {#step-allowlist-marketo-ips}

Quando il gruppo Marketing utilizza Marketo Engage per inviare e-mail di test (best practice consigliata prima di inviare e-mail di massa), a volte le e-mail di test vengono bloccate da sistemi anti-spam che si basano sugli indirizzi IP del mittente per verificare che l’e-mail sia valida. Per assicurarti che queste e-mail di test vengano recapitate, aggiungi Marketo Engage al tuo elenco di indirizzi IP consentiti.

Aggiungi questi indirizzi IP al tuo elenco Consentiti aziendale:

130.248.172.0/24

130.248.173.0/24

130.248.244.88/29

185.28.196.0/22

192.28.144.0/20

192.28.160.0/19

199.15.212.0/22

Per alcuni sistemi anti-spam, nell’elenco Consentiti viene utilizzato il campo Return-Path dell’e-mail invece dell’indirizzo IP. In questi casi, l’approccio migliore consiste nell’inserire nell’elenco Consentiti “&#42;.mktomail.com”, poiché Marketo Engage utilizza diversi sottodomini per le caselle di posta elettronica. Altri sistemi anti-spam utilizzano nell’elenco Consentiti l’indirizzo del mittente. In queste situazioni, assicurati di includere tutti i domini di invio (“Da”) utilizzati dal gruppo marketing nelle loro comunicazioni con persone e lead.

>[!NOTE]
>
>Il sistema Postini impiega una tecnologia unica e richiede di inserire nell’elenco Consentiti intervalli di indirizzi IP. Vedi [Aggiungere voci all’elenco Consentiti con Postini](https://nation.marketo.com/docs/DOC-1066).

## Passaggio 3: configurare SPF e DKIM {#step-set-up-spf-and-dkim}

Il team di marketing deve averti inviato anche i dati relativi a DKIM (Domain Keys Identified Mail) da aggiungere al record di risorse DNS (elencate di seguito). Segui questi passaggi per configurare DKIM e SPF (Sender Policy Framework), quindi avvisa il team di marketing una volta completato l’aggiornamento.

1. Per configurare SPF, aggiungi la riga seguente alle nostre voci DNS:

   `[CompanyDomain]` IN TXT v=spf1 mx ip4:`[CorpIP]`
include: mktomail.com ~all

   Se è già presente un record SPF nella voce DNS, aggiungi semplicemente quanto segue: 
include: mktomail.com

   Sostituisci CompanyDomain con il dominio principale del tuo sito web (ad esempio “`(company.com/)`”) e CorpIP con l’indirizzo IP del server di posta elettronica aziendale (ad es. “255.255.255.255”). Se intendi inviare e-mail da più domini tramite Marketo Engage, chiedi al personale IT di aggiungere questa riga per ciascun dominio (su una riga).

1. Per DKIM, crea record di risorse DNS per ogni dominio da impostare. Di seguito sono riportati i record host e i valori TXT per ogni dominio per il quale firmeremo:

   `[DKIMDomain1]`: il record host è `[HostRecord1]` e il valore TXT è `[TXTValue1]`.

   `[DKIMDomain2]`: il record host è `[HostRecord2]` e il valore TXT è `[TXTValue2]`.

   Copia HostRecord e TXTValue per ogni DKIMDomain configurato dopo aver seguito le [istruzioni qui](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}. Non dimenticare di verificare ogni dominio in Amministrazione > E-mail > DKIM dopo che il personale IT avrà completato questo passaggio.

## Passaggio 4: configurare DMARC {#set-up-dmarc}

DMARC (Domain-based Message Authentication, Reporting, and Conformance) è un protocollo di autenticazione utilizzato per aiutare le organizzazioni a proteggere il proprio dominio da utilizzi non autorizzati. DMARC estende i protocolli di autenticazione esistenti, come SPF e DKIM, per informare i server destinatari sulle azioni da intraprendere in caso di errore di autenticazione nel dominio. Anche se DMARC è attualmente facoltativo, è altamente consigliato in quanto proteggerà meglio il brand e la reputazione della tua organizzazione. I principali fornitori, come Google e Yahoo, richiederanno l’utilizzo di DMARC per i mittenti in blocco a partire da febbraio 2024.

Affinché il protocollo DMARC funzioni, devi disporre di almeno uno dei seguenti record TXT DNS:

* Un SPF valido
* Un record DKIM valido per il dominio FROM: (consigliato per Marketo Engage)

Inoltre, devi disporre di un record TXT DNS specifico per DMARC per il tuo dominio FROM. Facoltativamente, puoi definire un indirizzo e-mail a tua scelta per indicare dove posizionare i rapporti di DMARC all’interno della tua organizzazione, in modo da poterli monitorare.

Come best practice, si consiglia di implementare DMARC gradualmente, passando il criterio di DMARC da p=none a p=quarantine e infine a p=reject man mano che acquisisci familiarità con il potenziale impatto di DMARC, impostando inoltre i criteri di DMARC in modo da ottenere un allineamento semplificato su SPF e DKIM.

### Esempio di flusso di lavoro di DMARC {#dmarc-example-workflow}

1. Se hai configurato la ricezione dei rapporti DMARC, devi effettuare le seguenti operazioni:

   I. Analizza il feedback e i rapporti ricevuti e utilizza il criterio (p=none), che indica al destinatario di non intraprendere alcuna azione nei confronti dei messaggi che non superano l’autenticazione, ma di inviare comunque i rapporti e-mail al mittente.

   II. Se l’autenticazione dei messaggi legittimi non riesce, esamina e risolvi i problemi relativi a SPF/DKIM.

   III. Determina se SPF o DKIM sono allineati e consentono l’autenticazione di tutte le e-mail legittime.

   IV. Esamina i rapporti per assicurarti che i risultati corrispondano a quelli previsti in base ai criteri SPF/DKIM.

1. Regola il criterio in (p=quarantine), che indica al server di posta elettronica ricevente di mettere in quarantena i messaggi che non riescono ad autenticarsi (in genere tali messaggi vengono spostati nella cartella spam).

   I. Esamina i rapporti per assicurarti che i risultati siano quelli previsti.

1. Se il comportamento dei messaggi al livello p=quarantine ti soddisfa, puoi modificare il criterio in (p=reject). Il criterio p=reject indica al destinatario di rifiutare completamente (mancato recapito) qualsiasi e-mail per il dominio che non supera l’autenticazione. Con questo criterio abilitato, solo i messaggi e-mail verificati come autenticati al 100% dal tuo dominio potranno anche essere recapitati nella casella in entrata.

>[!CAUTION]
>
>Utilizza questa regola con cautela e determina se è appropriata per la tua organizzazione.

### Reporting di DMARC {#dmarc-reporting}

DMARC offre la possibilità di ricevere rapporti relativi alle e-mail che non superano SPF/DKIM. Esistono due diverse tipologie di rapporti generati dai provider ISP che i mittenti possono ricevere tramite i tag RUA/RUF nel proprio criterio DMARC. nell’ambito del processo di autenticazione.

* Rapporti aggregati (RUA): non contengono PII (informazioni personali identificabili) che potrebbero essere sensibili secondo il GDPR (Regolamento generale sulla protezione dei dati).

* Rapporti forensi (RUF): contengono indirizzi e-mail con dati sensibili secondo il GDPR. Prima dell’utilizzo, è consigliabile verificare internamente come gestire le informazioni in conformità al GDPR.

L’utilizzo principale di questi rapporti è quello di ricevere una panoramica delle e-mail che rappresentano un tentativo di spoofing. Si tratta di rapporti estremamente tecnici, che è consigliabile elaborare tramite un strumento di terze parti.

### Esempio di record DMARC {#example-dmarc-records}

* Record minimo necessario: `v=DMARC1; p=none`

* Record che punta a un indirizzo e-mail per ricevere i rapporti: `v=DMARC1; p=none;  rua=mailto:emaill@domain.com;     ruf=mailto:email@domain.com`

### Tag DMARC e funzionamento {#dmarc-tags-and-what-they-do}

I record DMARC dispongono di più componenti denominati tag DMARC. Ogni tag ha un valore che specifica un determinato aspetto di DMARC.

<table>
<thead>
  <tr>
    <th>Nome tag </th>
    <th>Obbligatorio/facoltativo </th>
    <th>Funzione </th>
    <th>Esempio </th>
    <th>Valore predefinito </th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>v</td>
    <td>Obbligatorio</td>
    <td>Questo tag DMARC specifica la versione. Al momento è disponibile una sola versione, quindi il valore fisso sarà v=DMARC1</td>
    <td>V=DMARC1 DMARC1</td>
    <td>DMARC1</td>
  </tr>
  <tr>
    <td>p</td>
    <td>Obbligatorio</td>
    <td>Mostra il criterio DMARC selezionato e indica al sistema ricevente di segnalare, mettere in quarantena o rifiutare un messaggio e-mail che non supera i controlli di autenticazione.</td>
    <td>p=none, quarantine o reject</td>
    <td>-</td>
  </tr>
  <tr>
    <td>fo</td>
    <td>Facoltativo</td>
    <td>Consente al proprietario del dominio di specificare le opzioni di reporting.</td>
    <td>0: genera rapporto se tutto non riesce
    <br>1: genera rapporto se qualsiasi cosa non riesce
    <br>d: genera rapporto se DKIM non riesce
    <br>s: genera rapporto se SPF non riesce</td>
    <td>1 (consigliato per i rapporti DMARC)</td>
  </tr>
  <tr>
    <td>pct</td>
    <td>Facoltativo</td>
    <td>Indica la percentuale di messaggi sottoposti a filtro.</td>
    <td>pct=20</td>
    <td>100</td>
  </tr>
  <tr>
    <td>rua</td>
    <td>Facoltativo (consigliato)</td>
    <td>Identifica dove verranno consegnati i rapporti aggregati.</td>
    <td>rua=mailto:aggrep@esempio.com</td>
    <td>-</td>
  </tr>
  <tr>
    <td>ruf</td>
    <td>Facoltativo (consigliato)</td>
    <td>Identifica dove verranno consegnati i rapporti forensi.</td>
    <td>ruf=mailto:authfail@esempio.com</td>
    <td>-</td>
  </tr>
  <tr>
    <td>sp</td>
    <td>Facoltativo</td>
    <td>Specifica il criterio DMARC per i sottodomini del dominio principale.</td>
    <td>sp=reject</td>
    <td>-</td>
  </tr>
  <tr>
    <td>adkim</td>
    <td>Facoltativo</td>
    <td>Può essere rigoroso (s, per Strict) o flessibile (r, per Relaxed). L’allineamento flessibile indica che il dominio utilizzato nella firma DKIM può essere un sottodominio dell’indirizzo “Da”. L’allineamento rigoroso indica che il dominio utilizzato nella firma DKIM deve corrispondere esattamente a quello nell’indirizzo Da.</td>
    <td>adkim=r </td>
    <td>r</td>
  </tr>
  <tr>
    <td>aspf</td>
    <td>Facoltativo</td>
    <td>Può essere rigoroso (s, per Strict) o flessibile (r, per Relaxed). L’allineamento flessibile indica che il dominio ReturnPath può essere un sottodominio dell’indirizzo Da. L’allineamento rigoroso indica che il dominio Return-Path deve corrispondere esattamente all’indirizzo Da.</td>
    <td>aspf=r</td>
    <td>r</td>
  </tr>
</tbody>
</table>

Per tutti i dettagli su DMARC e le relative opzioni, visita [https://dmarc.org/](https://dmarc.org/){target="_blank"}.

### DMARC e Marketo Engage {#dmarc-and-marketo-engage}

Esistono due tipi di allineamento per DMARC: allineamento DKIM ed SPF.

>[!NOTE]
>
>Si consiglia di impostare l’allineamento DMARC su DKIM rispetto a SPF per Marketo Engage.

* DMARC allineato a DKIM - Per configurare DMARC allineato a DKIM:

   * Imposta DKIM per il dominio DA: del tuo messaggio. Segui le istruzioni riportate in [questo articolo](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}.
   * Configura DMARC per il dominio FROM:/DKIM configurato in precedenza

* SPF allineato a DMARC - Per impostare SPF allineato a DMARC tramite il Return-Path con brand:

   * Imposta il dominio Return-Path con brand
      * Configura il record SPF appropriato
      * Modifica il record MX in modo che punti a quello predefinito per il datacenter da cui viene inviata l’e-mail

   * Configura DMARC per il dominio Return-Path con brand

* Se invii messaggi tramite Marketo Engage con un IP dedicato e non hai già implementato (o non hai la certezza di aver implementato) un Return-Path con brand, apri un ticket presso l’[assistenza Adobe](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

* Se invii messaggi da Marketo Engage tramite un pool condiviso di IP, puoi verificare se sei idoneo per gli IP attendibili [facendone richiesta qui](https://na-sjg.marketo.com/lp/marketoprivacydemo/Trusted-IP-Sending-Range-Program.html){target="_blank"}. Il Return-Path con brand è offerto gratuitamente a chi invia da IP attendibili di Marketo Engage. Se ricevi l’approvazione per questo programma, contatta l’assistenza Adobe per impostare il Return-Path con brand.

   * IP attendibili: un pool condiviso di IP riservati agli utenti con bassi volumi, che inviano meno di 75.000 messaggi al mese e non sono idonei per un IP dedicato. Questi utenti devono inoltre soddisfare i requisiti delle best practice.

* Se invii messaggi da Marketo Engage tramite IP condivisi e non sei idoneo per gli IP attendibili e invii più di 100.000 messaggi al mese, devi contattare il team Adobe Account (il tuo account manager) per acquistare un IP dedicato.

* L’allineamento SPF rigoroso non è supportato né consigliato in Marketo Engage.

## Passaggio 5: configurare i record MX per il dominio {#step-set-up-mx-records-for-your-domain}

Un record MX ti consente di ricevere e-mail al dominio da cui le stai inviando, per elaborare le risposte e i risponditori automatici. Se invii dal dominio aziendale, probabilmente lo hai già configurato. In caso contrario, in genere puoi configurarlo con la mappatura sul record MX del dominio aziendale.

## Indirizzi IP in uscita {#outbound-ip-addresses}

Una connessione in uscita è una connessione effettuata da Marketo Engage per tuo conto verso un server su Internet. Alcuni partner/fornitori con cui collabori o la tua organizzazione IT possono utilizzare l’elenco Consentiti per limitare l’accesso ai server. In tal caso, devi fornire loro i blocchi di indirizzi IP in uscita di Marketo Engage da aggiungere ai loro elenchi Consentiti.

**Webhook**

I [webhook](/help/marketo/product-docs/administration/additional-integrations/create-a-webhook.md){target="_blank"} di Marketo Engage sono un meccanismo di integrazione in uscita. Quando viene eseguita un’azione di flusso [Chiamata webhook](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/call-webhook.md){target="_blank"} come parte di una campagna avanzata, viene effettuata una richiesta HTTP a un servizio web esterno. Se l’editore del servizio web utilizza un elenco Consentiti sul firewall della rete in cui si trova il servizio web esterno, deve aggiungere al proprio elenco Consentiti i blocchi di indirizzi IP elencati di seguito.

**Sincronizzazione CRM**

Le funzionioni di [sincronizzazione con CRM Salesforce](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/add-an-existing-salesforce-field-to-the-marketo-sync.md){target="_blank"} e [sincronizzazione con Microsoft Dynamics](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md){target="_blank"} di Marketo Engage sono meccanismi di integrazione che eseguono richieste HTTP in uscita alle API pubblicate dal fornitore del sistema CRM. Assicurati che la tua organizzazione IT non impedisca a nessuno dei blocchi di indirizzi IP riportati di seguito di accedere alle API del tuo fornitore CRM.

**Blocchi di indirizzi IP in uscita di Marketo Engage**

Le seguenti tabelle coprono tutti i server Marketo Engage che effettuano chiamate in uscita. Utilizza gli elenchi qui sotto per la configurazione dell’elenco Consentiti di indirizzi IP, server, firewall, elenco di controllo degli accessi, gruppo di sicurezza o servizio di terze parti per la ricezione di connessioni in uscita da Marketo Engage.

<table>
 <tbody>
  <tr>
   <th>Blocco IP (notazione CIDR)</th>
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
  <tr>
   <td>124.47.174.193</td>
  </tr>
  <tr>
   <td>130.248.168.16</td>
  </tr>
   <tr>
   <td>130.248.168.17</td>
  </tr>
  <tr>
   <td>199.15.213.245</td>
  </tr>
  <tr>
   <td>199.15.215.245</td>
  </tr>
 </tbody>
</table>
