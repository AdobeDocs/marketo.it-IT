---
unique-page-id: 17727995
description: Email CC - Marketo Docs - Documentazione prodotto
title: CC e-mail
translation-type: tm+mt
source-git-commit: 0f0217a88929661798015b51a26259a973f9f6ea
workflow-type: tm+mt
source-wordcount: '547'
ht-degree: 0%

---


# Email CC {#email-cc}

Email CC consente l&#39;invio tramite Marketo di e-mail specifiche per includere i destinatari CC.

Questa funzione è disponibile su tutte le risorse e-mail di Marketo, a prescindere da come l’e-mail viene inviata (in batch o viene attivata la campagna). Il destinatario CC riceverà una copia esatta dell&#39;e-mail inviata alla persona selezionata. Come tale, qualsiasi attività di coinvolgimento (aperture, clic ecc.) verranno registrati nel registro delle attività della Persona di marketing nella riga &quot;A&quot; dell&#39;e-mail. Tuttavia, attività di consegna (inviata, consegnata, rimbalzo duro, ecc.) _diverso da &quot;rimbalzo morbido&quot;_ non si  **** registrerà, in quanto Marketo non è in grado di distinguere gli eventi di consegna per Marketo Person dai destinatari CC&quot;. Marketo può CC fino a 100.000 persone alla volta. Se la tua smart list supera i 100 k ed è imperativo che ogni persona su di esso ottiene CC&#39;d, ti consigliamo di interrompere la tua lista.

>[!NOTE]
>
>Email CC non è stato progettato per essere utilizzato con test A/B. Potete comunque utilizzarlo se desiderate, ma poiché tecnicamente non è supportato, il supporto di Marketo non sarebbe in grado di fornire assistenza per la risoluzione di problemi.

## Impostazione di Email CC {#set-up-email-cc}

1. In My Marketo, fare clic su **Admin**.

   ![](assets/one.png)

1. Nella struttura ad albero, selezionare **E-mail**.

   ![](assets/two.png)

1. Fare clic su **Edit Email CC Settings**.

   ![](assets/three.png)

1. Seleziona fino a 25 campi Marketo Lead o Company (di tipo &quot;E-mail&quot;) per rendere disponibile l&#39;uso come indirizzi CC nelle e-mail. Fare clic su **Salva** al termine.

   ![](assets/four.png)

## Utilizzo di Email CC {#using-email-cc}

1. Selezionate il messaggio e-mail e fate clic su **Modifica bozza**.

   ![](assets/five.png)

1. Fare clic su **Impostazioni e-mail**.

   ![](assets/six.png)

1. Seleziona fino a cinque campi da utilizzare per CC People. In questo esempio, vogliamo solo che il proprietario principale sia CC. Fare clic su **Salva** al termine.

   ![](assets/seven.png)

   È semplice come quella! Nell’esempio precedente, quando invii l’e-mail, il proprietario principale dei destinatari scelti sarà CCd.

   >[!NOTE]
   >
   >Se un indirizzo e-mail non valido si trova in un campo CC, verrà ignorato.

   Per una rapida identificazione, la visualizzazione Riepilogo e-mail mostra se sono stati selezionati i campi per e-mail con CC.

   ![](assets/eight.png)

   Se l&#39;e-mail è approvata, ma l&#39;amministratore di marketing disabilita uno o più campi CC prima dell&#39;invio dell&#39;e-mail, **gli utenti non riceveranno un&#39;e-mail**. In questo scenario, la visualizzazione Riepilogo e-mail visualizzerà in grigio tutti i campi che sono stati disattivati dopo l’approvazione ma che sono stati pre-inviati:

   ![](assets/removal.png)

   >[!NOTE]
   >
   >Questo errore viene visualizzato anche nella sezione Impostazioni e-mail della bozza dell&#39;e-mail.

## Dopo la {#after-the-send}

* Se un destinatario CC fa clic su un collegamento tracciato nell’e-mail, l’attività di clic (come tutte le altre attività di coinvolgimento) verrà associata al destinatario principale dell’e-mail. Inoltre, possono passare a una pagina con il codice di monitoraggio Web di Marketo (munchkin.js), causando il cookie come destinatario principale.

>[!TIP]
>
>È possibile disattivare alcuni o tutti i collegamenti di tracciamento](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/disable-tracking-for-an-email-link.md) in un messaggio e-mail.[

* Dopo l&#39;esecuzione di una campagna e-mail, l&#39;attività Invia e-mail includerà un elenco di tutti gli indirizzi CC inclusi per ciascun destinatario della mailing. Se eventuali indirizzi CC sono stati ignorati a causa dell’annullamento della sottoscrizione, questa verrà rilevata anche nell’attività.
* I collegamenti e le pagine di annullamento della sottoscrizione funzionano normalmente nelle e-mail CCd. Questo consente ai destinatari CC di annullare l’iscrizione se lo desiderano (nel rispetto delle normative anti-spam) e un record di questa azione verrà memorizzato nel database Marketo.
* Le persone elencate come non sottoscritte nel database Marketo **non** riceveranno e-mail tramite CC.
