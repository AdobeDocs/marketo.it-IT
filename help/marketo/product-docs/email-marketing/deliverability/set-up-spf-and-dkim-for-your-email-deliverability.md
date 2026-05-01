---
unique-page-id: 4720710
description: Scopri come configurare SPF e DKIM nel DNS per migliorare il recapito messaggi e-mail. Autorizza Marketo a inviare per tuo conto e a ridurre i flag di posta indesiderata.
title: Configurare SPF e DKIM per la recapitabilità e-mail
exl-id: a0f88e94-3348-4f48-bbd2-963e2af93dc0
feature: Deliverability
source-git-commit: 240b78561db11e169188698880d4707a5c1f64de
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 89%

---

# Configurare SPF e DKIM per la recapitabilità e-mail {#set-up-spf-and-dkim-for-your-email-deliverability}

Un metodo rapido per migliorare il tasso di consegna delle e-mail consiste nell’incorporare **SPF** (Sender Policy Framework) e **DKIM** (Domain Keys Identified Mail) nelle impostazioni DNS. Con questa aggiunta alle voci DNS, stai dicendo ai destinatari che hai autorizzato Marketo a inviare e-mail per tuo conto. Senza questa modifica, l’e-mail ha una maggiore probabilità di essere considerata spam poiché è stata indirizzata dal tuo dominio, ma tramite un indirizzo IP con dominio Marketo.

>[!CAUTION]
>
>Per apportare questa modifica al record DNS è necessario rivolgersi all’amministratore della rete.

## Configurare SPF {#set-up-spf}

**Se NON disponi di un record SPF nel tuo dominio**

Chiedi all’amministratore della tua rete di aggiungere la riga seguente alle voci DNS. Sostituisci [domain] con il dominio principale del tuo sito web (ad es. “azienda.com”) e [corpIP] con l’indirizzo IP del server di posta elettronica aziendale (ad es. &quot;255.255.255.255&quot;). Se invii e-mail da più domini tramite Marketo, devi aggiungere questa voce a ciascun dominio (su una riga).

`[domain] IN TXT v=spf1 mx ip4:[corpIP] include:mktomail.com ~all`

**Se DISPONI di un record SPF nel tuo dominio**

Se disponi già di un record SPF nella voce DNS, aggiungi quanto segue:

include:mktomail.com

## Configurare DKIM {#set-up-dkim}

**Cos’è DKIM? Perché configurare DKIM?**

DKIM è un protocollo di autenticazione utilizzato dai server che ricevono le e-mail per determinare se un messaggio e-mail è stato effettivamente inviato dal mittente indicato. DKIM spesso migliora la recapitabilità delle e-mail nella casella in entrata, in quanto consente di verificare che il messaggio non sia un falso.

**Come funziona DKIM?**

Una volta configurata la chiave pubblica nel record DNS e attivato il dominio di invio nella sezione di amministrazione (A), verrà attivata la firma personalizzata DKIM per i messaggi in uscita, che includerà una firma digitale crittografata con ogni e-mail inviata per tuo conto (B). I server riceventi saranno quindi in grado di decrittografare la firma digitale facendo riferimento alla “chiave pubblica” nel DNS del dominio di invio (C). Se la chiave nell’e-mail corrisponde a quella nel record DNS, è più probabile che il server e-mail ricevente accetti l’e-mail inviata da Marketo per tuo conto.

![](assets/image2015-1-12-13-3a56-3a55.png)

**Come configurare DKIM?**

Consulta [Configurare una firma DKIM personalizzata](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}.

>[!MORELIKETHIS]
>
>* Scopri di più su SPF e sul suo funzionamento`: http://www.open-spf.org/Introduction/`
>* Il mio SPF è configurato correttamente?: `https://www.kitterman.com/spf/validate.html`
>* Ho usato la sintassi corretta?: `http://www.open-spf.org/SPF_Record_Syntax/`
