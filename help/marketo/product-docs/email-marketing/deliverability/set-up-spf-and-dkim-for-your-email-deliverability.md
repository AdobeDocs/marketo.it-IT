---
unique-page-id: 4720710
description: Impostazione di SPF e DKIM per la distribuzione delle e-mail - Marketo Docs - Documentazione del prodotto
title: Impostazione di SPF e DKIM per la distribuzione tramite e-mail
translation-type: tm+mt
source-git-commit: 074701d1a5f75fe592ac7f44cce6fb3571e94710
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 0%

---


# Impostare SPF e DKIM per la distribuzione delle e-mail {#set-up-spf-and-dkim-for-your-email-deliverability}

Un metodo rapido per migliorare le percentuali di consegna delle e-mail consiste nell&#39;incorporare **SPF** (Sender Policy Framework) e **DKIM** (Domain Keys Identified Mail) nelle impostazioni DNS. Con questa aggiunta alle voci DNS, stai dicendo ai destinatari che hai autorizzato Marketo a inviare e-mail per conto tuo. Senza questa modifica, l&#39;e-mail ha maggiori possibilità di essere contrassegnata come spam da quando l&#39;e-mail è stata indirizzata dal dominio, ma inviata da un indirizzo IP con un dominio Marketo.

>[!CAUTION]
>
>L&#39;amministratore di rete dovrà apportare questa modifica al record DNS.

## Configurare SPF {#set-up-spf}

**Se NON si dispone di un record SPF sul dominio**

Chiedete all&#39;amministratore di rete di aggiungere la seguente riga alle voci DNS. Sostituire [dominio] con il dominio principale del sito Web (ad esempio &quot;company.com&quot;) e [corpIP] con l&#39;indirizzo IP del server di posta elettronica aziendale (ad esempio &quot;255.255.255.255&quot;). Se invii e-mail da più domini tramite Marketo, devi aggiungerlo a ciascun dominio (su una sola riga).

`[domain] IN TXT v=spf1 mx ip4:[corpIP] include:mktomail.com ~all`

**Se si dispone di un record SPF nel dominio**

Se nella voce DNS è già presente un record SPF, aggiungervi quanto segue:

include:mktomail.com

## Configurare DKIM {#set-up-dkim}

**Cos&#39;è DKIM? Perché si desidera impostare DKIM?**

DKIM è un protocollo di autenticazione che viene utilizzato dai ricevitori e-mail per determinare se un messaggio e-mail è stato inviato da chi afferma che è stato inviato da. DKIM migliora spesso la possibilità di inviare e-mail alla inbox, dal momento che il destinatario può essere certo che il messaggio non è un falso.

**Come funziona DKIM?**

Dopo aver configurato la chiave pubblica nel record DNS e attivato il dominio di invio nella sezione Amministratore (A), attiveremo la firma DKIM personalizzata per i messaggi in uscita, che includerà una firma digitale crittografata con ogni e-mail inviata per voi (B). I ricevitori potranno decifrare la firma digitale cercando la &quot;chiave pubblica&quot; nel DNS (C) del dominio di invio. Se la chiave nell&#39;e-mail corrisponde alla chiave nel record DNS, è più probabile che il server di posta ricevente accetti l&#39;e-mail inviata da Marketo per conto dell&#39;utente.

![](assets/image2015-1-12-13-3a56-3a55.png)

**Come si configura DKIM?**

Fare riferimento a [Configurare una firma DKIM personalizzata](/help/marketo/product-docs/email-marketing/deliverability/set-up-a-custom-dkim-signature.md).

>[!MORELIKETHIS]
>
>* [Scopri di più su SPF e come funziona](https://www.open-spf.org/Introduction/)
>* [Strumenti di distribuzione delle e-mail di Marketo](https://www.marketo.com/software/email-marketing/email-deliverability/)
>* [Il mio SPF è impostato correttamente?](https://www.kitterman.com/spf/validate.html)
>* [Ho usato la sintassi giusta?](https://www.open-spf.org/SPF_Record_Syntax/)

