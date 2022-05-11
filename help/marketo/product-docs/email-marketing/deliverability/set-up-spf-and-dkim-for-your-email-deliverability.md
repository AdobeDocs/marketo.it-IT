---
unique-page-id: 4720710
description: Configurare SPF e DKIM per la consegna delle e-mail - Documenti Marketo - Documentazione del prodotto
title: Impostare SPF e DKIM per il recapito messaggi e-mail
exl-id: a0f88e94-3348-4f48-bbd2-963e2af93dc0
source-git-commit: de32becbfe74c2a88c53de8af8be4ee022782114
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 0%

---

# Impostare SPF e DKIM per il recapito messaggi e-mail {#set-up-spf-and-dkim-for-your-email-deliverability}

Un metodo rapido per migliorare le percentuali di consegna delle e-mail è quello di incorporare **SPF** (Framework dei criteri per il mittente) e **DKIM** (Domain Keys Identified Mail) nelle impostazioni DNS. Oltre alle voci DNS, stai comunicando ai destinatari che hai autorizzato Marketo a inviare e-mail per tuo conto. Senza questa modifica, l’e-mail ha maggiori possibilità di essere contrassegnata come spam da quando l’e-mail è stata indirizzata dal tuo dominio, ma inviata da un indirizzo IP con un dominio Marketo.

>[!CAUTION]
>
>Per apportare questa modifica al record DNS, è necessario che l’amministratore di rete apporti questa modifica.

## Imposta SPF {#set-up-spf}

**Se NON hai un record SPF sul tuo dominio**

Chiedi all&#39;amministratore di rete di aggiungere la seguente riga alle voci DNS. Sostituisci [dominio] con il dominio principale del tuo sito web (es. &quot;company.com&quot;) e [corpIP] con l&#39;indirizzo IP del server e-mail aziendale (ad es. &quot;255.255.255.255&quot;). Se invii e-mail da più domini tramite Marketo, devi aggiungerle a ciascun dominio (su una riga).

`[domain] IN TXT v=spf1 mx ip4:[corpIP] include:mktomail.com ~all`

**Se disponi di un record SPF sul dominio**

Se nella voce DNS è già presente un record SPF, aggiungilo come segue:

include:mktomail.com

## Configurare DKIM {#set-up-dkim}

**Cos&#39;è DKIM? Perché voglio configurare DKIM?**

DKIM è un protocollo di autenticazione utilizzato dai ricevitori di e-mail per determinare se un messaggio e-mail è stato inviato da chi afferma che è stato inviato da. DKIM migliora spesso la consegna delle e-mail alla casella in entrata, poiché un destinatario può essere sicuro che il messaggio non è un falso.

**Come funziona DKIM?**

Dopo aver impostato la chiave pubblica nel record DNS e aver attivato il dominio di invio nella sezione Amministratore (A), attiveremo la firma DKIM personalizzata per i messaggi in uscita, che includerà una firma digitale crittografata con ogni e-mail inviata per te (B). I ricevitori potranno decrittografare la firma digitale ricercando la &quot;chiave pubblica&quot; nel DNS (C) del dominio di invio. Se la chiave nell’e-mail corrisponde alla chiave nel record DNS, il server di posta ricevente accetterà più facilmente l’e-mail Marketo inviata per tuo conto.

![](assets/image2015-1-12-13-3a56-3a55.png)

**Come si configura DKIM?**

Fai riferimento a [Imposta una firma DKIM personalizzata](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md).

>[!MORELIKETHIS]
>
>* [Ulteriori informazioni su SPF e come funziona](http://www.open-spf.org/Introduction/)
>* [Strumenti di consegna e-mail Marketo](https://www.marketo.com/software/email-marketing/email-deliverability/)
>* [Il Mio SPF È Impostato Correttamente?](https://www.kitterman.com/spf/validate.html)
>* [Ho usato la sintassi giusta?](http://www.open-spf.org/SPF_Record_Syntax/)

