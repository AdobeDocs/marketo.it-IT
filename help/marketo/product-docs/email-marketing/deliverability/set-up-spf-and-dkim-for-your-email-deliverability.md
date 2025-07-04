---
unique-page-id: 4720710
description: Configurare SPF e DKIM per il recapito messaggi e-mail - Documentazione Marketo - Documentazione del prodotto
title: Configurare SPF e DKIM per il recapito messaggi e-mail
exl-id: a0f88e94-3348-4f48-bbd2-963e2af93dc0
feature: Deliverability
source-git-commit: b95458ffab422901ef5e674756ae5e413ec542fd
workflow-type: tm+mt
source-wordcount: '421'
ht-degree: 0%

---

# Configurare SPF e DKIM per il recapito messaggi e-mail {#set-up-spf-and-dkim-for-your-email-deliverability}

Un metodo rapido per migliorare le percentuali di consegna delle e-mail consiste nell&#39;incorporare **SPF** (Sender Policy Framework) e **DKIM** (Domain Keys Identified Mail) nelle impostazioni DNS. Con questa aggiunta alle voci DNS, stai dicendo ai destinatari che hai autorizzato Marketo a inviare e-mail per tuo conto. Senza questa modifica, l’e-mail ha una maggiore probabilità di essere contrassegnata come spam poiché è stata indirizzata dal dominio, ma inviata da un indirizzo IP con un dominio Marketo.

>[!CAUTION]
>
>Per apportare questa modifica nel record DNS è necessario rivolgersi all&#39;amministratore di rete.

## Configurare SPF {#set-up-spf}

**Se non hai un record SPF nel tuo dominio**

Chiedere all&#39;amministratore di rete di aggiungere la riga seguente alle voci DNS. Sostituisci [dominio] con il dominio principale del tuo sito Web (ad es. &quot;company.com&quot;) e [corpIP] con l&#39;indirizzo IP del server di posta elettronica aziendale (ad esempio &quot;255.255.255.255&quot;) Se invii e-mail da più domini tramite Marketo, devi aggiungerle a ciascun dominio (su una riga).

`[domain] IN TXT v=spf1 mx ip4:[corpIP] include:mktomail.com ~all`

**Se il tuo dominio contiene un record SPF**

Se nella voce DNS è già presente un record SPF, aggiungervi quanto segue:

include:mktomail.com

## Configurare DKIM {#set-up-dkim}

**Cos&#39;è DKIM? Perché configurare DKIM?**

DKIM è un protocollo di autenticazione utilizzato dai destinatari e-mail per determinare se un messaggio e-mail è stato inviato da chi lo afferma. DKIM spesso migliora il recapito delle e-mail alla casella in entrata, in quanto il destinatario può essere certo che il messaggio non sia un falso.

**Come funziona DKIM?**

Dopo aver configurato la chiave pubblica nel record DNS e aver attivato il dominio di invio nella sezione Amministratore (A), verrà attivata la firma personalizzata di DKIM per i messaggi in uscita, che includerà una firma digitale crittografata con ogni e-mail inviata per te (B). I riceventi saranno in grado di decrittografare la firma digitale cercando la &quot;chiave pubblica&quot; nel DNS (C) del dominio di invio. Se la chiave nell’e-mail corrisponde a quella nel record DNS, è più probabile che il server di posta ricevente accetti l’e-mail Marketo inviata per tuo conto.

![](assets/image2015-1-12-13-3a56-3a55.png)

**Configurazione di DKIM**

Consulta [Configurare una firma DKIM personalizzata](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md){target="_blank"}.

>[!MORELIKETHIS]
>
>* Ulteriori informazioni su SPF e sul suo funzionamento`: http://www.open-spf.org/Introduction/`
>* Il mio SPF è configurato correttamente?: `https://www.kitterman.com/spf/validate.html`
>* Ho usato la sintassi corretta?: `http://www.open-spf.org/SPF_Record_Syntax/`
