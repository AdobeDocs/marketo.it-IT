---
description: Passaggi della configurazione - Documenti Marketo - Documentazione del prodotto
short-description: Hai appena iniziato a usare Adobe Marketo Engage? Scopri quali passaggi devi completare prima di iniziare a utilizzarlo.
title: Passaggi di configurazione
feature: Getting Started
exl-id: 5f37da48-b2ed-4e48-a5a2-429149745085
source-git-commit: 21bcdc10fe1f3517612efe0f8e2adaf2f4411a70
workflow-type: tm+mt
source-wordcount: '1663'
ht-degree: 2%

---

# Passaggi di configurazione {#setup-steps}

**Benvenuto in Adobe Marketo Engage!**

Prima di immergerti, devi completare alcuni passaggi.

Questi passaggi includono:

* Personalizzare gli URL della pagina di destinazione e i collegamenti e-mail per migliorare l’affidabilità e il recapito messaggi
* Configurazione dei protocolli per Marketo Engage
* Sincronizzazione del CRM in corso
* Aggiunta di codice di tracciamento al sito Web aziendale

>[!NOTE]
>
>Devi eseguire questi passaggi solo se la tua azienda è **nuova in Marketo**. In caso contrario, la configurazione potrebbe essere già stata eseguita.

Alcuni passaggi richiedono l’aiuto del team IT.

## Garantire il recapito dei messaggi e-mail {#ensure-email-deliverability}

>[!NOTE]
>
>Sei cliente di Launch Pack? Puoi saltare questo passaggio. Il tuo consulente ti fornirà un documento con le istruzioni per la configurazione IT durante la tua chiamata di avvio.

Puoi adottare diverse misure per garantire che le e-mail raggiungano il maggior numero possibile di persone.

* **Personalizza i collegamenti di tracciamento**. Puoi scegliere un CNAME per utilizzare il tuo dominio (anziché quello di Marketo) nei collegamenti che includi nelle e-mail da Marketo. Questo rafforza il branding del dominio e aumenta la fiducia e il recapito messaggi con i destinatari.
* **Aggiungi Marketo al tuo inserisco nell&#39;elenco Consentiti di gestione delle e-mail aziendali per il tuo indirizzo di posta elettronica**. È buona prassi comune inviare e-mail di test agli account di test prima di inviare e-mail alle persone effettive. di inserire nell&#39;elenco Consentiti Marketo, puoi evitare che le e-mail di test vengano bloccate o contrassegnate come spam.
* **Configura SPF e DKIM**. Queste tecnologie garantiscono ai destinatari che le e-mail Marketo non siano spam. Per evitare che i filtri anti-spam dei destinatari rifiutino le e-mail di Marketo, segui la procedura riportata di seguito per [Configurare un SPF e un DKIM per il recapito e-mail](/help/marketo/product-docs/email-marketing/deliverability/set-up-spf-and-dkim-for-your-email-deliverability.md).
* **Imposta un record MX per il dominio.** Un record MX ti consente di ricevere e-mail al dominio da cui stai inviando l&#39;e-mail per elaborare le risposte e i risponditori automatici. Se invii dal dominio aziendale, probabilmente lo hai già configurato. In caso contrario, puoi in genere impostare la mappatura sul record MX del dominio aziendale.
* **Impostazioni consigliate per l&#39;indirizzo Da.** In tutte le campagne e-mail devi utilizzare un dominio e-mail valido, esistente e funzionante nell&#39;Indirizzo mittente. Può essere utile configurare un sottodominio del dominio aziendale piuttosto che inviare dati dal dominio aziendale. In questo modo i problemi del flusso di posta aziendale non influiranno sul flusso di posta Marketo e viceversa. Inoltre, l&#39;invio di posta da `something@nonexistentdomain.com` causerà il filtraggio o il blocco delle e-mail. Qualsiasi dominio utilizzato nell&#39;indirizzo mittente deve avere un account postmaster@ valido e funzionante e un account abusivo@.

Se utilizzi le app Google per l’hosting dell’e-mail aziendale, non potrai creare e-mail di abuso@ o postmaster@ nel tuo dominio. Per ovviare a questo problema, è necessario creare gruppi denominati &quot;abuso&quot; e &quot;postmaster&quot;. Gli utenti membri di questi gruppi riceveranno le e-mail inviate a tali indirizzi (ad esempio, <postmaster@domain.com>). Le istruzioni dettagliate per la creazione dei gruppi sono disponibili [qui](https://support.google.com/a/answer/33343#adminconsole){target="_blank"}.

Scegli un CNAME per i collegamenti di tracciamento e-mail (scegli un CNAME _diverso_ dalla pagina di destinazione selezionata al passaggio 3). Alcuni esempi:

* vai2.[DominioSocietà].com
* em.[DominioSocietà].com
* wow![DominioSocietà].com

La prima parte è il CNAME di tracciamento e-mail, `[EmailTrackingCNAME]`. Sarà necessario assegnarlo al reparto IT.

>[!CAUTION]
>
>I CNAME per e-mail e pagina di destinazione devono essere diversi. Inoltre, evita CNAME come &quot;track&quot; o &quot;link&quot;. Viene spesso segnalato come spam

Per trovare il collegamento di tracciamento di Marketo, vai all&#39;area **[!UICONTROL Admin]**.

![](assets/setup-steps-1.png)

Fai clic su **[!UICONTROL Email]**.

![](assets/setup-steps-2.png)

Copia [!UICONTROL Tracking Link] dalle impostazioni e-mail.

[!UICONTROL Tracking Link] è nel formato: `mkto-[a-z][4 digits].com`.

![](assets/setup-steps-3.png)

`[MktoTrackingLink]`. Salvatela. Sarà necessario consegnarlo al reparto IT nel passaggio 5.

Raccogli i domini &quot;Da&quot;. Creare un elenco di tutti i domini &quot;Da&quot; (come in `[Sender]@[FromDomain].com`) che si intende utilizzare per l&#39;invio di e-mail da Marketo. Per la maggior parte, ce n&#39;è solo uno.

Ad esempio, &#39;marketo.com&#39; &#39;info.marketo.com&#39;. Si tratta di `[FromDomain1]`,`[FromDomain2]`, ecc. Salvateli. Dovrai assegnarli al reparto IT nel passaggio 5.

Ora disponi di tutte le informazioni necessarie per inviare la richiesta al reparto IT.

## Personalizzare gli URL della pagina di destinazione con un CNAME {#customize-your-landing-page-urls-with-a-cname}

>[!NOTE]
>
>Sei cliente di Launch Pack? Puoi saltare questo passaggio. Il tuo consulente ti fornirà un documento con le istruzioni per la configurazione IT durante la tua chiamata di avvio.

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

Scegli un CNAME per le pagine di destinazione. Alcuni esempi:

    * **vai**.[DominioSocietà].com
    * **www2**.[DominioSocietà].com
    * **lp**.[DominioSocietà].com

>[!TIP]
>
>Sii breve! Gli URL più brevi sono più facili da ricordare. Consigliamo di usare &quot;go&quot; come dominio.

La prima parte in grassetto è `[LandingPageCNAME]`. Ne avrai bisogno al punto 5.

Per recuperare l&#39;ID Munchkin che sostituirai con il CNAME della pagina di destinazione, passa all&#39;area **Amministratore**.

![](assets/setup-steps-4.png)

Fai clic su **Il mio account**.

![](assets/setup-steps-5.png)

Copia [!UICONTROL Account String] dalle impostazioni della pagina di destinazione.

![](assets/setup-steps-6.png)

Questo è `[Munchkin ID]`. Salvatela. Sarà necessario consegnarlo al reparto IT nel passaggio 5.

Configura le impostazioni del dominio in modo che le pagine di destinazione utilizzino il dominio della tua azienda invece di quello di Marketo (dove sono ospitate).

## Chiedi all&#39;IT di configurare i protocolli {#ask-it-to-configure-protocols}

>[!NOTE]
>
>Sei cliente di Launch Pack? Puoi saltare questo passaggio. Il tuo consulente ti fornirà un documento con le istruzioni per la configurazione IT durante la tua chiamata di avvio.

Una volta raccolte tutte le informazioni necessarie, puoi inviare una richiesta al reparto IT. È possibile utilizzare il testo seguente come modello, sostituendo il testo in grassetto con le proprie informazioni.

[Includi un collegamento a questo articolo](/help/marketo/getting-started/initial-setup/configure-protocols-for-marketo.md).

Incolla questo testo nell’e-mail e sostituisci i segnaposto in grassetto:

>[!NOTE]
>
>Vedere i passaggi 3 e 4 per determinare il testo da sostituire ai segnaposto. Ricorda che `[LandingPageCNAME]` e `[EmailTrackingCNAME]` devono essere diversi.

`----------------------------------------------`

Gentile amministratore IT,

Il team Marketing utilizza la piattaforma Marketo per comunicare con il personale. Per garantire un recapito messaggi e-mail ottimale, è necessario apportare le seguenti modifiche:

`1)` Per le nostre pagine di destinazione, aggiungi una voce DNS (CNAME) per **[LandingPageCNAME]**.**[DominioSocietà]**.com, che punta a **[ID Munchkin]**.mktoweb.com.

`2)` Per i collegamenti di tracciamento nelle e-mail, aggiungi una voce DNS (CNAME) per **[EmailTrackingCNAME]**.**[DominioSocietà]**.com, che punta a **[MktoTrackingLink]**.

`3)` Inserire nell&#39;elenco Consentiti Marketo.

    * Se si utilizzano gli indirizzi IP nel Inserisco nell&#39;elenco Consentiti di delle e-mail, aggiungere gli IP elencati di seguito:
    199.15.212.0/22
    
    192.28.144.0/20
    
    192.28.160.0/19
    
    185.28.196.0/22
    
    130.248.172.0/24
    
    130.248.173.0/24
    
    103.237.104.0/22
    
    94.236.119.0/26

>[!NOTE]
>
>Contatta il Supporto Marketo se desideri un elenco abbreviato di IP da al inserisco nell&#39;elenco Consentiti specifico per il tuo ambiente.

    * Se il sistema antispam utilizza i domini From, aggiungi questi:

**`[FromDomain1]`**
**`[FromDomain2]`**

`4)` È necessario configurare SPF e DKIM in modo che Marketo sia autorizzato a inviare e-mail firmate per nostro conto.

`a.` Per configurare SPF, aggiungere la seguente riga alle voci DNS:

IN TXT **[Da dominio]**: v=spf1 mx ip4:**[IP aziendali]**
<br/>include: mktomail.com ~tutti

Se disponiamo già di un record SPF nella voce DNS, è sufficiente aggiungervi quanto segue:

include:mktomail.com

`[`Sostituisci **Dal dominio** con il tuo indirizzo e-mail Dal dominio (es: company.com) e **CorpIP** con l&#39;indirizzo IP del tuo server e-mail aziendale (es: 255.255.255.255).  Se intendi inviare e-mail da più domini tramite Marketo, il tuo staff IT dovrebbe aggiungere questa riga per ciascun dominio (su una riga).`]`

`b.` Per DKIM, creare record di risorse DNS per ogni dominio che si desidera impostare. Di seguito sono riportati i record host e i valori TXT per ogni dominio per cui firmeremo:

**`[DKIMDomain1]`**: il record host è **`[HostRecord1]`** e il valore TXT è **`[TXTValue1]`**.

**`[DKIMDomain2]`**: il record host è **`[HostRecord2]`** e il valore TXT è **`[TXTValue2]`**.

`[`Copiare **HostRecord** e **TXTValue** per ogni **DKIMDomain** configurato dopo aver seguito le [istruzioni](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md). Non dimenticare di verificare ogni dominio in **Amministratore > E-mail > DKIM** dopo che il personale IT ha completato questo passaggio.`]`

`5)` È necessario assicurarsi che sia presente un record MX valido per i domini FROM **`[FromDomain1]`**, **`[FromDomain2]`**, ecc. Può confermare? In caso contrario, configuralo per eseguire il mapping al record MX del dominio aziendale. In questo modo sarà possibile elaborare le risposte e i risponditori automatici alle nostre comunicazioni Marketo.

Fatemi sapere quando avete completato questi passaggi, in modo che io possa completare il processo di configurazione con Marketo.

Grazie. Sei il migliore!

Cordiali saluti

**`[Your Name]`**

`----------------------------------------------`

Invia l&#39;e-mail al reparto IT. Sappiamo che il completamento di queste attività può richiedere del tempo all&#39;IT. Puoi continuare con il passaggio successivo, ma ricorda che devi tornare a questo passaggio per completare la configurazione di Marketo Engage.

## Completare l&#39;installazione di Marketo al termine dell&#39;IT {#complete-your-marketo-setup-after-it-finishes}

Una volta completate le attività, segui questi passaggi per aggiungere la pagina di destinazione e i CNAME e-mail e per attivare la firma DKIM.

Vai all&#39;area **[!UICONTROL Admin]** per aggiungere il tuo CNAME pagina di destinazione

![](assets/setup-steps-7.png)

Selezionare le pagine di destinazione e fare clic su **[!UICONTROL Edit]** nell&#39;area [!UICONTROL Settings].

![](assets/setup-steps-8.png)

Immettere il nuovo nome di dominio nel campo **[!UICONTROL Domain Name for Landing Pages]**. Il modulo dovrebbe essere:

`[LandingPageCNAME].[CompanyDomain].com`

![](assets/setup-steps-9.png)

Nel campo pagina **[!UICONTROL Fallback]**, immettere l&#39;URL a cui si desidera che le persone accedano se una pagina di destinazione non è disponibile. Se non disponi di una pagina di fallback, puoi utilizzare la home page dell’azienda. Nel campo **[!UICONTROL Homepage]**, immetti il sito Web della tua azienda.

![](assets/setup-steps-10.png)

Nell&#39;area [!UICONTROL Admin], seleziona **[!UICONTROL Email]** per aggiungere il tuo CNAME e-mail

![](assets/setup-steps-11.png)

Scorri verso il basso fino a [!UICONTROL Branding Domains]. Selezionare il dominio e fare clic su **[!UICONTROL Edit]**.

![](assets/setup-steps-12.png)

Nel campo Dominio, immetti il dominio di tracciamento e-mail. Il modulo dovrebbe essere:

`[EmailTrackingCNAME].[CompanyDomain].com`. Fai clic su **[!UICONTROL Save]**.

![](assets/setup-steps-13.png)

## Integrare il CRM {#integrate-your-crm}

Questa è probabilmente la parte più emozionante della configurazione. È ora di riempire Marketo con tutti quei lead e contatti che hai memorizzato nel tuo CRM!

Scegli una delle seguenti opzioni, a seconda del sistema di gestione delle relazioni con i clienti utilizzato dalla tua azienda.

* [Integra Marketo Engage con  [!DNL Salesforce.com]](/help/marketo/product-docs/crm-sync/salesforce-sync/understanding-the-salesforce-sync.md)
* [Integra Marketo Engage con  [!DNL Microsoft Dynamics]](/help/marketo/product-docs/crm-sync/microsoft-dynamics-sync/understanding-the-microsoft-dynamics-sync.md)

  >[!NOTE]
  >
  >Per completare questi passaggi, è necessario l’assistenza dell’amministratore del sistema di gestione delle relazioni con i clienti della tua azienda.

## Aggiungi codice di tracciamento al tuo sito web {#add-tracking-code-to-your-website}

>[!NOTE]
>
>Sei un cliente di [!DNL Launch Pack]? Puoi saltare questo passaggio. Il tuo consulente ti fornirà le istruzioni del codice [!DNL Munchkin] nel documento di istruzioni per la configurazione IT.

Marketo Engage dispone di un JavaScript di tracciamento personalizzato (denominato [!DNL Munchkin]) che è possibile utilizzare per tenere traccia delle attività personali su qualsiasi pagina Web. [!DNL Munchkin] è richiesto per integrare il sito Web in Marketo. Segui questi passaggi per [Aggiungere [!DNL Munchkin] codice di tracciamento al tuo sito Web](/help/marketo/product-docs/administration/additional-integrations/add-munchkin-tracking-code-to-your-website.md){target="_blank"}.

>[!NOTE]
>
>Per aggiungere il codice di tracciamento è necessaria l’esperienza con HTML.

## Aspettative di prestazioni {#performance-expectations}

Quali sono le aspettative in termini di prestazioni di Marketo? Può variare a seconda delle dimensioni e della complessità delle campagne di marketing. Tuttavia, è possibile aspettarsi livelli di prestazioni equivalenti a quelli descritti nella colonna &quot;Standard&quot; in diverse tabelle presenti nella [descrizione del prodotto Marketo Engage](https://helpx.adobe.com/legal/product-descriptions/adobe-marketo-engage---product-description.html){target="_blank"}. Le colonne &quot;Prestazioni&quot; e &quot;Performance Plus&quot; fanno riferimento a pacchetti del livello prestazioni che forniscono [livelli di prestazioni superiori](https://nation.marketo.com/t5/product-documents/marketo-engage-performance-tiers/ta-p/328835){target="_blank"}.

>[!MORELIKETHIS]
>
>* [Configura protocolli per Marketo Engage](/help/marketo/getting-started/initial-setup/configure-protocols-for-marketo.md)
>
>* [Configurazione utente](/help/marketo/getting-started/initial-setup/user-setup.md)
