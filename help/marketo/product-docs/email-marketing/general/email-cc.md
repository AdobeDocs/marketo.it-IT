---
unique-page-id: 17727995
description: E-mail CC - Documentazione di Marketo - Documentazione del prodotto
title: E-mail CC
exl-id: 00550e98-916d-4e66-91f8-7394c242a29b
feature: Email Editor
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '547'
ht-degree: 0%

---

# E-mail CC {#email-cc}

E-mail CC consente l’invio di e-mail specifiche tramite Marketo per includere i destinatari CC.

Questa funzione è disponibile su tutte le risorse e-mail di Marketo, indipendentemente da come viene inviata l’e-mail (batch o attiva campagna). Il destinatario CC riceverà una copia esatta dell’e-mail inviata alla persona Marketo scelta. Di conseguenza, qualsiasi attività di coinvolgimento (aperture, clic, ecc.) verrà registrato nel registro attività della persona Marketo nella riga &quot;A&quot; dell’e-mail. Tuttavia, l’attività di consegna (inviata, consegnata, mancato recapito permanente, ecc.) _diverso da &quot;mancato recapito non permanente&quot;_ will **non** registrarsi, in quanto Marketo non è in grado di distinguere gli eventi di consegna per la persona Marketo dai destinatari CC. Marketo creerà fino a 100.000 CC alla volta. Se la tua lista intelligente supera i 100.000 e ogni persona che la contiene deve assolutamente ottenere un certificato CC, ti consigliamo di spezzarla.

>[!NOTE]
>
>E-mail CC non è stato progettato per essere utilizzato con test A/B. Puoi utilizzarlo comunque, ma poiché tecnicamente non è supportato, il Supporto Marketo non sarà in grado di fornire assistenza per la risoluzione dei problemi.

## Configurare E-mail CC {#set-up-email-cc}

1. In Il mio Marketo, fai clic su **Amministratore**.

   ![](assets/one.png)

1. Nella struttura, seleziona **E-mail**.

   ![](assets/two.png)

1. Clic **Modifica impostazioni CC e-mail**.

   ![](assets/three.png)

1. Seleziona fino a 25 campi per lead Marketo o società (di tipo &quot;E-mail&quot;) da rendere disponibili come indirizzi CC nelle e-mail. Clic **Salva** al termine.

   ![](assets/four.png)

## Utilizzo di E-mail CC {#using-email-cc}

1. Seleziona l’e-mail e fai clic su **Modifica bozza**.

   ![](assets/five.png)

1. Clic **Impostazioni e-mail**.

   ![](assets/six.png)

1. Selezionare fino a cinque campi che si desidera utilizzare per le persone CC. In questo esempio, vogliamo solo il CC del proprietario del lead. Clic **Salva** al termine.

   ![](assets/seven.png)

   È semplice come quello! Nell’esempio precedente, quando invii l’e-mail, il Proprietario lead dei destinatari scelti sarà CC’d.

   >[!NOTE]
   >
   >Se un indirizzo e-mail non valido si trova in un campo CC, verrà ignorato.

   Per una rapida identificazione, la visualizzazione Riepilogo e-mail mostra se/quali campi E-mail CC sono stati selezionati.

   ![](assets/eight.png)

   Se l’e-mail è approvata, ma l’amministratore di Marketo disabilita uno o più campi CC prima dell’invio dell’e-mail, **queste persone non riceveranno un’e-mail**. In questo caso, la visualizzazione Riepilogo e-mail disabiliterà tutti i campi disabilitati dopo l’approvazione ma prima dell’invio:

   ![](assets/removal.png)

   >[!NOTE]
   >
   >L’errore riportato sopra viene visualizzato anche nella sezione Email Settings (Impostazioni e-mail) della bozza dell’e-mail.

## Dopo l’invio {#after-the-send}

* Se un destinatario CC fa clic su un collegamento tracciato nell’e-mail, l’attività di clic (come tutte le altre attività di coinvolgimento) verrà associata al destinatario principale dell’e-mail. Inoltre, possono fare clic su una pagina con il codice di tracciamento web di Marketo (munchkin.js), facendoli diventare il destinatario principale.

>[!TIP]
>
>Hai la possibilità di: [disabilitazione di alcuni o di tutti i collegamenti di tracciamento](/help/marketo/product-docs/email-marketing/general/functions-in-the-editor/disable-tracking-for-an-email-link.md) in un messaggio e-mail.

* Dopo l’esecuzione di una campagna e-mail, l’attività Invia e-mail includerà un elenco di tutti gli indirizzi CC inclusi per ciascun destinatario dell’e-mail. Se alcuni indirizzi CC sono stati saltati a causa dell’annullamento dell’abbonamento, questo verrà rilevato anche nell’attività.
* I collegamenti e le pagine per annullare l’abbonamento funzionano normalmente nelle e-mail in CC. Questo consente ai destinatari CC di annullare l’abbonamento se lo desiderano (in conformità con le normative anti-spam) e un record di questa azione verrà memorizzato nel database di Marketo.
* Le persone elencate come non sottoscritte nel tuo database Marketo **non** ricevere e-mail tramite CC.
