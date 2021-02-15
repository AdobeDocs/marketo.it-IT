---
unique-page-id: 10617187
description: Informazioni sulle impostazioni sulla privacy - Documenti Marketo - Documentazione del prodotto
title: Informazioni sulle impostazioni di privacy
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 0%

---


# Informazioni sulle impostazioni di privacy {#understanding-privacy-settings}

## Panoramica {#overview}

Marketo offre agli esperti di marketing un modo per ottenere il consenso dei visitatori del Web per seguirli. Esistono due modi per rifiutare o potete scegliere di essere tracciati tramite IP anonimi.

* I visitatori Web selezionano la funzione Non tenere traccia (DNT) nel browser (e l&#39;esperto di marketing rispetta la richiesta del visitatore Web di Non tenere traccia)
* I visitatori Web utilizzano un cookie di rinuncia fornito da un esperto di marketing su un sito Web

Oppure, l&#39;esperto di marketing può monitorare gli utenti, ma utilizzare un IP anonimo.

Questi metodi possono influenzare il valore e la funzionalità di Marketo in aree specifiche. Tuttavia, se l&#39;esperto di marketing *non modifica nulla nella configurazione di Marketo, la funzionalità di Marketo rimane la stessa.*

## Impostazioni browser per non tenere traccia {#browser-settings-for-do-not-track}

I visitatori Web possono impostare il proprio browser per impedire il tracciamento da parte di qualsiasi sito Web scegliendo &quot;Non tenere traccia&quot; (DNT). Questo impedisce il monitoraggio di questo particolare browser e dispositivo. Per informazioni dettagliate, consultate le impostazioni di privacy del browser.

A Monaco, un esperto di marketing può [decidere se supportare o ignorare l&#39;impostazione DNT del browser](/help/marketo/product-docs/administration/settings/edit-do-not-track-browser-support-settings.md).

In Web Personalization (Personalizzazione Web), un esperto di marketing può decidere se [supportare o ignorare l&#39;impostazione DNT del browser](/help/marketo/product-docs/web-personalization/getting-started/setting-web-personalization-to-do-not-track.md).

## Rifiuto da un sito Web specifico {#opt-out-from-a-specific-website}

Potete inoltre consentire ai visitatori del sito di rifiutare il tracciamento del sito Web, indipendentemente dalla configurazione delle impostazioni **Browser Do Not Track**. Questo consente al visitatore del sito di specificare le proprie preferenze di tracciamento direttamente dal sito Web.

A tal fine, dovete aggiungere un parametro a un collegamento di rifiuto in una pagina Web in cui sia attivato il tracciamento dei mecchi. Può trattarsi di una qualsiasi pagina Web, ma il collegamento della pagina Web deve contenere il seguente parametro:

?marketo_opt_out=true

Di seguito sono riportati alcuni esempi di una pagina Web con un collegamento di rinuncia e una pagina di destinazione dopo aver fatto clic sul collegamento. La tua varierà.

Di seguito è riportata una pagina Web con un pulsante con il parametro &quot;?marketo_opt_out=true&quot; nel collegamento di rinuncia.

![](assets/opt-out-1.png)

Potete creare e pubblicare una pagina di destinazione come pagina di follow-up quando viene fatto clic sul collegamento con il parametro &quot;?marketo_opt_out=true&quot;.

![](assets/opt-out-2.png)

Quando si fa clic sul collegamento, Marketo aggiunge un cookie denominato **mkto_opt_out** al browser del visitatore che disabilita il tracciamento di Munchkin per il visitatore del sito che fa clic sul collegamento con il parametro precedente.

Per verificare che il cookie possa essere impiantato, verifica di essere un lead cucinato e fai clic sul collegamento. Quindi controllate i cookie del browser per verificare che sia stato aggiunto il cookie **mkto_opt_out**.

![](assets/opt-out-3.png)

>[!NOTE]
>
>Attualmente funziona solo con Munchkin versioni 152 e successive.

## Opt In {#opt-in}

Gli addetti al marketing possono consentire agli utenti di scegliere se utilizzare le funzionalità di Marketo nelle e-mail, nei moduli, nelle pagine di destinazione e in altri metodi.

## Tracciamento tramite un IP anonimo {#tracking-using-an-anonymized-ip}

Gli addetti al marketing possono preservare la privacy monitorando gli utenti con un indirizzo IP anonimo. A tal fine, aggiungete questo codice al codice RTP o Munchkin Javascript incorporato nel sito Web.

* Per Munchkin, aggiungi semplicemente {&quot;anonymizeIP&quot;,true} alla funzione init.

   >[!NOTE]
   >
   >L&#39;utilizzo di questo parametro richiede che Munchkin V2 sia abilitato. Per attivarla per l&#39;iscrizione, contattate il [Supporto marketing](https://nation.marketo.com/community/support_solutions).

* Per la personalizzazione Web (RTP), aggiungete questo al javascript:

`anonymize IP : before calling rtp('send','view'); add rtp('set', 'settings', {'anonymizeIP' : true});`
