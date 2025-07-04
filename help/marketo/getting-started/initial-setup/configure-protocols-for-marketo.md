---
unique-page-id: 4720433
description: Configurare i protocolli per Marketo Engage - Documentazione Marketo Engage - Documentazione del prodotto
title: Configurazione dei protocolli per Marketo Engage
exl-id: cf2fd4ac-9229-4e52-bb68-5732b44920ef
feature: Getting Started
source-git-commit: 8ff62b372b4d0f98ab88c569bdc3608eb63b70c7
workflow-type: tm+mt
source-wordcount: '2131'
ht-degree: 8%

---

# Configurazione dei protocolli per Marketo Engage{#configure-protocols-for-marketo-engage}

Se l&#39;utente o l&#39;organizzazione utilizza impostazioni restrittive del firewall o del server proxy, potrebbe essere necessario inserire nell&#39;elenco Consentiti alcuni domini e intervalli di indirizzi IP per garantire il corretto funzionamento di Adobe Marketo Engage.

Per assistenza nell’implementazione dei protocolli riportati di seguito, condividi questo articolo con il tuo reparto IT. Se limitano l’accesso web utilizzando un inserisco nell&#39;elenco Consentiti di, accertati di aggiungere i seguenti domini (incluso l’asterisco) per consentire tutte le risorse e i websockets di Marketo Engage:

* `*.marketo.com`
* `*.marketodesigner.com`
* `*.mktoweb.com`
* `*.experience.adobe.com`
* `*.adobe.net`

## Passaggio 1: creare record DNS per le pagine di destinazione e l’e-mail {#step-create-dns-records-for-landing-pages-and-email}

**CNAME collegamento di tracciamento**

Il team marketing avrebbe dovuto inviarti due richieste per nuovi record CNAME. Il primo è per gli URL della pagina di destinazione, in modo che le pagine di destinazione vengano visualizzate in URL che riflettono il dominio e non Marketo Engage (l’host effettivo). La seconda è per i collegamenti di tracciamento inclusi nelle e-mail inviate da Marketo Engage.

`1` **Aggiungi CNAME per le pagine di destinazione**

Aggiungi il CNAME della pagina di destinazione che ti hanno inviato al tuo record DNS, in modo che `[YourLandingPageCNAME]` punti alla stringa account univoca assegnata alle tue pagine di destinazione Marketo Engage. Accedi al sito del tuo registrar di dominio e immetti il CNAME della pagina di destinazione e la stringa dell’account. In genere, questo comporta tre campi:

* Alias: immetti `[YourLandingPageCNAME]` (fornito dal marketing)
* Tipo: CNAME
* Puntare a: immettere `[MunchkinID].mktoweb.com` (fornito dal marketing)

`2` **Aggiungi CNAME per i collegamenti di tracciamento e-mail**

Aggiungi l&#39;e-mail inviata dal marketing CNAME, in modo che `[YourEmailCNAME]` punti a [MktoTrackingLink], il collegamento di tracciamento predefinito assegnato da Marketo Engage, nel formato:\
`[YourEmailCNAME].[YourDomain].com` IN CNAME `[MktoTrackingLink]`

Ad esempio:

`pages.abc.com IN CNAME mkto-a0244.com`

>[!NOTE]
>
>`[MktoTrackingLink]` deve essere il dominio di branding predefinito.

`3` **Notifica al team marketing**

Avvisa il team marketing quando hai completato questo processo.

`4` **Contatta il [Supporto Adobe](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"} per avviare il processo di provisioning di un certificato SSL.**

Il completamento di questo processo può richiedere fino a 3 giorni lavorativi.

## Passaggio 2: Inserire nell&#39;elenco Consentiti IP Marketo Engage {#step-allowlist-marketo-ips}

Quando il gruppo Marketing utilizza Marketo Engage per inviare e-mail di test (una best practice per evitare l’invio di messaggi esplosivi), a volte le e-mail di test vengono bloccate da sistemi anti-spam che si basano sugli indirizzi IP del mittente per verificare che l’e-mail sia valida. Per assicurarti che arrivino queste e-mail di test, aggiungi Marketo Engage al tuo inserisco nell&#39;elenco Consentiti di.

Aggiungi questi indirizzi IP al tuo elenco Consentiti di aziendale:

103.237.104.0/22

130.248.172.0/24

130.248.173.0/24

130.248.244.88/29

185.28.196.0/22

192.28.144.0/20

192.28.160.0/19

199.15.212.0/22

Alcuni sistemi anti-spam utilizzano il campo Return-Path (Percorso di ritorno) dell’e-mail invece dell’indirizzo IP per l’inserimento nell’elenco Consentiti. In questi casi, l&#39;approccio migliore consiste nel inserire nell&#39;elenco Consentiti &#39;&#42;.mktomail.com&#39;, poiché Marketo Engage utilizza diversi sottodomini delle cassette postali. Inserire nell&#39;elenco Consentiti Altri sistemi anti-spam si in base all&#39;indirizzo del mittente. In queste situazioni, assicurati di includere tutti i domini di invio (&quot;Da&quot;) utilizzati dal gruppo Marketing per comunicare con persone/lead.

>[!NOTE]
>
>Postini impiega una tecnologia unica e richiede la inserire nell&#39;elenco Consentiti di intervalli IP da parte di. Vedi [Inserisce nell&#39;elenco Consentiti con Postini](https://nation.marketo.com/docs/DOC-1066).

## Passaggio 3: configurare SPF e DKIM {#step-set-up-spf-and-dkim}

Il team marketing avrebbe dovuto inviarti anche informazioni su DKIM (Domain Keys Identified Mail) da aggiungere al record di risorse DNS (anch’esso elencato di seguito). Segui i passaggi per configurare correttamente DKIM e SPF (Sender Policy Framework), quindi avvisa il team di marketing che l’aggiornamento è stato completato.

1. Per impostare SPF, aggiungi la seguente riga alle voci DNS:

   `[CompanyDomain]` IN TXT v=spf1 mx ip4:`[CorpIP]`\
   include: mktomail.com ~tutti

   Se disponiamo già di un record SPF nella voce DNS, è sufficiente aggiungervi quanto segue:\
   include: mktomail.com

   Sostituire CompanyDomain con il dominio principale del sito Web (ad esempio: &quot;`(company.com/)`&quot;) e CorpIP con l&#39;indirizzo IP del server di posta elettronica aziendale (ad esempio &quot;255.255.255.255&quot;) Se intendi inviare e-mail da più domini tramite Marketo Engage, il tuo staff IT dovrebbe aggiungere questa riga per ciascun dominio (su una riga).

1. Per DKIM, crea record di risorse DNS per ogni dominio che desideri impostare. Di seguito sono riportati i record host e i valori TXT per ogni dominio per cui firmeremo:

   `[DKIMDomain1]`: il record host è `[HostRecord1]` e il valore TXT è `[TXTValue1]`.

   `[DKIMDomain2]`: il record host è `[HostRecord2]` e il valore TXT è `[TXTValue2]`.

   Copiare HostRecord e TXTValue per ogni dominio DKIMD configurato dopo aver seguito le [istruzioni qui](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}. Non dimenticare di verificare ogni dominio in Amministratore > E-mail > DKIM dopo che il personale IT ha completato questo passaggio.

## Passaggio 4: configurare DMARC {#set-up-dmarc}

DMARC (Domain-based Message Authentication, Reporting &amp; Conformance) è un protocollo di autenticazione utilizzato per aiutare le organizzazioni a proteggere il proprio dominio da utilizzi non autorizzati. DMARC estende i protocolli di autenticazione esistenti, come SPF e DKIM, per informare i server destinatari sulle azioni da intraprendere in caso di errore di autenticazione nel dominio. Anche se DMARC è attualmente opzionale, è vivamente consigliato in quanto proteggerà meglio il marchio e la reputazione della tua organizzazione. I principali provider come Google e Yahoo richiederanno l’utilizzo di DMARC per i mittenti in blocco a partire da febbraio 2024.

Affinché il protocollo DMARC funzioni, devi disporre di almeno uno dei seguenti record TXT DNS:

* Un SPF valido
* Un record DKIM valido per il dominio FROM: (consigliato per Marketo Engage)

Inoltre, è necessario disporre di un record TXT DNS specifico per DMARC per il dominio FROM:. Facoltativamente, puoi definire un indirizzo e-mail a tua scelta per indicare dove collocare i rapporti di DMARC all’interno della tua organizzazione, in modo da poter monitorare i rapporti.

Come best practice, si consiglia di implementare lentamente l’implementazione di DMARC aumentando il livello dei criteri di DMARC da p=none a p=quarantena, a p=rifiuta man mano che acquisisci comprensione del potenziale impatto di DMARC, e di impostare i criteri di DMARC in modo da ottenere un allineamento meno rigoroso su SPF e DKIM.

### Esempio di flusso di lavoro di DMARC {#dmarc-example-workflow}

1. Se sei configurato per ricevere i rapporti di DMARC, devi effettuare le seguenti operazioni...

   I. Analizza il feedback e i rapporti ricevuti e utilizzati (p=none), che indica al destinatario di non eseguire azioni contro i messaggi che non superano l’autenticazione, ma che inviano comunque i rapporti e-mail al mittente.

   II. Rivedi e risolvi i problemi relativi a SPF/DKIM se l’autenticazione dei messaggi legittimi non riesce.

   III. Determina se SPF o DKIM sono allineati e consentono l’autenticazione di tutte le e-mail legittime.

   IV. Esamina i rapporti per assicurarti che i risultati siano quelli previsti in base ai criteri SPF/DKIM.

1. Procedi con l’impostazione del criterio (p=quarantena), che indica al server e-mail ricevente di mettere in quarantena le e-mail che non superano l’autenticazione (in genere significa inserire tali messaggi nella cartella di posta indesiderata).

   I. Rivedi i rapporti per assicurarti che i risultati siano quelli previsti.

1. Se si è soddisfatti del comportamento dei messaggi a livello di p=quarantena, è possibile modificare i criteri in (p=rifiuta). Il criterio p=rifiuta indica al destinatario di rifiutare completamente (non recapitare) qualsiasi e-mail per il dominio che non supera l’autenticazione. Con questo criterio abilitato, solo i messaggi e-mail verificati come autenticati al 100% dal dominio avranno anche la possibilità di inserire messaggi nella casella in entrata.

>[!CAUTION]
>
>Utilizza questa regola con cautela e determina se è appropriata per la tua organizzazione.

### Generazione rapporti DMARC {#dmarc-reporting}

DMARC offre la possibilità di ricevere rapporti relativi alle e-mail che non superano SPF/DKIM. Esistono due diversi rapporti generati dai server ISP come parte del processo di autenticazione che i mittenti possono ricevere tramite i tag RUA/RUF nei propri criteri DMARC.

* Aggregate Reports (RUA): non contiene dati PII (personalmente identificabili) sensibili ai requisiti del GDPR (General Data Protection Regulation, Regolamento generale sulla protezione dei dati).

* Rapporti forensi (RUF): contiene indirizzi e-mail sensibili al RGPD. Prima di utilizzare, è consigliabile verificare internamente come gestire le informazioni che devono essere conformi ai requisiti RGPD.

L’utilizzo principale di questi rapporti è quello di ricevere una panoramica delle e-mail che sono un tentativo di spoofing. Si tratta di rapporti altamente tecnici che è meglio digerire tramite uno strumento di terze parti.

### Esempio di record DMARC {#example-dmarc-records}

* Record minimo nudo: `v=DMARC1; p=none`

* Registra indirizzamento a un indirizzo e-mail per ricevere i report: `v=DMARC1; p=none;  rua=mailto:emaill@domain.com;     ruf=mailto:email@domain.com`

### Tag DMARC e operazioni {#dmarc-tags-and-what-they-do}

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
    <td>Mostra il criterio di DMARC selezionato e indirizza il destinatario a segnalare, mettere in quarantena o rifiutare i messaggi che non superano i controlli di autenticazione.</td>
    <td>p=none, quarantena o rifiuto</td>
    <td>-</td>
  </tr>
  <tr>
    <td>fo</td>
    <td>Facoltativo</td>
    <td>Consente al proprietario del dominio di specificare le opzioni di reporting.</td>
    <td>0: genera il rapporto se tutto non riesce 
    <br>1: genera report in caso di errori 
    <br>d: genera report in caso di errore di DKIM 
    <br>s: genera report se SPF non riesce</td>
    <td>1 (consigliato per i rapporti di DMARC)</td>
  </tr>
  <tr>
    <td>pct</td>
    <td>Facoltativo</td>
    <td>Indica la percentuale di messaggi soggetti a filtro.</td>
    <td>pct=20</td>
    <td>100</td>
  </tr>
  <tr>
    <td>rua</td>
    <td>Facoltativo (consigliato)</td>
    <td>Identifica dove verranno consegnati i rapporti aggregati.</td>
    <td>rua=mailto:aggrep@example.com</td>
    <td>-</td>
  </tr>
  <tr>
    <td>ruf</td>
    <td>Facoltativo (consigliato)</td>
    <td>Identifica dove verranno consegnati i rapporti forensi.</td>
    <td>ruf=mailto:authfail@example.com</td>
    <td>-</td>
  </tr>
  <tr>
    <td>sp</td>
    <td>Facoltativo</td>
    <td>Specifica i criteri di DMARC per i sottodomini del dominio padre.</td>
    <td>sp=rifiuta</td>
    <td>-</td>
  </tr>
  <tr>
    <td>adkim</td>
    <td>Facoltativo</td>
    <td>Può essere Strict (s) o Relaxed ®. L’allineamento rilassato indica che il dominio utilizzato nella firma DKIM può essere un sottodominio dell’indirizzo "Da". L'allineamento rigido indica che il dominio utilizzato nella firma DKIM deve corrispondere esattamente al dominio utilizzato nell'indirizzo Da.</td>
    <td>adkim=r </td>
    <td>r</td>
  </tr>
  <tr>
    <td>aspf</td>
    <td>Facoltativo</td>
    <td>Può essere Strict (s) o Relaxed ®. L'allineamento semplificato indica che il dominio ReturnPath può essere un sottodominio dell'indirizzo From. L'allineamento rigido indica che il dominio del percorso di ritorno deve corrispondere esattamente all'indirizzo Da.</td>
    <td>aspf=r</td>
    <td>r</td>
  </tr>
</tbody>
</table>

Per informazioni complete su DMARC e sulle opzioni disponibili, visitare il sito Web all&#39;indirizzo [https://dmarc.org/](https://dmarc.org/){target="_blank"}.

### DMARC e MARKETO ENGAGE {#dmarc-and-marketo-engage}

Esistono due tipi di allineamento per DMARC: allineamento DKIM e allineamento SPF.

>[!NOTE]
>
>Si consiglia di eseguire l&#39;allineamento DMARC su DKIM rispetto a SPF per Marketo Engage.

* DMARC allineato a DKIM: per configurare DMARC allineato a DKIM è necessario:

   * Configura DKIM per il dominio FROM: del messaggio. Utilizza le istruzioni [in questo articolo](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}.
   * Configura DMARC per il dominio FROM:/DKIM configurato in precedenza

* SPF allineato a DMARC: per impostare SPF allineato a DMARC tramite il percorso di ritorno del marchio, è necessario:

   * Imposta il dominio del percorso di ritorno con marchio
      * Configurare il record SPF appropriato
      * Modifica il record MX in modo che punti al record MX predefinito per il datacenter in cui verrà inviata la posta

   * Configurare DMARC per il dominio del percorso di ritorno del marchio

* Se invii messaggi da Marketo Engage tramite un IP dedicato e non hai già implementato il percorso di ritorno del marchio, oppure non sei sicuro di averlo fatto, apri un ticket con [Supporto Adobe](https://nation.marketo.com/t5/support/ct-p/Support){target="_blank"}.

* Se invii messaggi da Marketo Engage tramite un pool condiviso di IP, puoi verificare se sei idoneo per gli IP attendibili [applicando qui](https://na-sjg.marketo.com/lp/marketoprivacydemo/Trusted-IP-Sending-Range-Program.html?lang=it){target="_blank"}. Il percorso di ritorno con marchio è offerto gratuitamente a chi invia da IP attendibili di Marketo Engage. Se approvato per questo programma, contatta il supporto Adobe per impostare il percorso di ritorno a marchio.

   * IP attendibili: un pool condiviso di IP riservati agli utenti con volumi inferiori che inviano &lt;75.000/mese che non sono idonei per un IP dedicato. Anche questi utenti devono soddisfare i requisiti delle best practice.

* Se invii messaggi da Marketo Engage tramite IP condivisi e non sei idoneo per gli IP attendibili e invii più di 100.000 messaggi al mese, devi contattare il Team account di Adobe (il tuo account manager) per acquistare un IP dedicato.

* L&#39;allineamento rigoroso dell&#39;SPF non è supportato né consigliato in Marketo Engage.

## Passaggio 5: configurare i record MX per il dominio {#step-set-up-mx-records-for-your-domain}

Un record MX ti consente di ricevere e-mail al dominio da cui stai inviando l’e-mail per elaborare le risposte e gli auto-responder. Se invii dal dominio aziendale, probabilmente lo hai già configurato. In caso contrario, in genere è possibile configurarlo per eseguire la mappatura sul record MX del dominio aziendale.

## Indirizzi IP in uscita {#outbound-ip-addresses}

Per connessione in uscita si intende una connessione effettuata da Marketo Engage a un server su Internet per conto dell&#39;utente. Alcuni partner/fornitori con cui collabori o la tua organizzazione IT possono utilizzare i inserisce nell&#39;elenco Consentiti di accesso ai server di un&#39;organizzazione di IT di cui si è proprietari, in modo da limitare l&#39;accesso ai server. In tal caso, devi fornire loro i blocchi di indirizzi IP in uscita di Marketo Engage da aggiungere ai loro elenchi Consentiti.

**Webhook**

I [webhook](/help/marketo/product-docs/administration/additional-integrations/create-a-webhook.md){target="_blank"} di Marketo Engage sono un meccanismo di integrazione in uscita. Quando viene eseguita un&#39;azione di flusso [Chiama webhook](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/flow-actions/call-webhook.md){target="_blank"} come parte di una campagna intelligente, viene effettuata una richiesta HTTP a un servizio Web esterno. Se l’editore del servizio web utilizza un inserisco nell&#39;elenco Consentiti di sul firewall della rete in cui si trova il servizio web esterno, deve aggiungere i blocchi di indirizzi IP elencati di seguito al proprio inserisco nell&#39;elenco Consentiti di.

**Sincronizzazione CRM**

Marketo Engage [Salesforce CRM Sync](/help/marketo/product-docs/crm-sync/salesforce-sync/sfdc-sync-details/add-an-existing-salesforce-field-to-the-marketo-sync.md){target="_blank"} e [Microsoft Dynamics Sync](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md){target="_blank"} sono meccanismi di integrazione che eseguono richieste HTTP in uscita alle API pubblicate dal fornitore del sistema CRM. È necessario assicurarsi che l’organizzazione IT non blocchi nessuno dei blocchi di indirizzi IP riportati di seguito per l’accesso alle API del fornitore CRM.

**Blocchi di indirizzi IP in uscita Marketo Engage**

Le tabelle seguenti descrivono tutti i server Marketo Engage che effettuano chiamate in uscita. Inserire nell&#39;elenco Consentiti Utilizzare gli elenchi riportati di seguito se si sta configurando un gruppo IP, un server, un firewall, un elenco di controllo di accesso, un gruppo di sicurezza o un servizio di terze parti per ricevere connessioni in uscita da Marketo Engage.

<table>
 <tbody>
  <tr>
   <th>Blocco IP (notazione CIDR)</th>
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
   <td>13 237 155 207</td>
  </tr>
   <tr>
   <td>13 55 192 247</td>
  </tr>
  <tr>
   <td>18 200 201 81</td>
  </tr>
  <tr>
   <td>34 247 24 245</td>
  </tr>
  <tr>
   <td>35 165 244 220</td>
  </tr>
  <tr>
   <td>44 235 171 179</td>
  </tr>
  <tr>
   <td>52 20 211 99</td>
  </tr>
  <tr>
   <td>52 64 109 86</td>
  </tr>
  <tr>
   <td>54 160 246 246</td>
  </tr>
  <tr>
   <td>54 212 167 17</td>
  </tr>
  <tr>
   <td>54 220 138 65</td>
  </tr>
   <tr>
   <td>54 237 141 197</td>
  </tr>
  <tr>
   <td>124 47 174 193</td>
  </tr>
  <tr>
   <td>130 248 168 166</td>
  </tr>
   <tr>
   <td>130 248 168 17</td>
  </tr>
  <tr>
   <td>199.15.213.245</td>
  </tr>
  <tr>
   <td>199.15.215.245</td>
  </tr>
 </tbody>
</table>
