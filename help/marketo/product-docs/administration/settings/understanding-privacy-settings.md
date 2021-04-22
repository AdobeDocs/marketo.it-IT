---
unique-page-id: 10617187
description: Informazioni sulle impostazioni della privacy - Documenti Marketo - Documentazione del prodotto
title: Informazioni sulle impostazioni di privacy
exl-id: 1fde9011-02a9-4ec9-bfa4-c56a52ce1eed
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '521'
ht-degree: 0%

---

# Informazioni sulle impostazioni della privacy {#understanding-privacy-settings}

## Panoramica {#overview}

Marketo offre agli esperti di marketing un modo per ottenere il consenso dei visitatori web per seguirli. Esistono due modi per rinunciare o puoi scegliere di essere monitorato da IP anonimi.

* I visitatori web selezionano la funzione Do Not Track (DNT) nel proprio browser (e l’addetto al marketing rispetta la richiesta del visitatore web Do Not Track)
* I visitatori web utilizzano un cookie di rinuncia fornito da un esperto di marketing su un sito web

Oppure, l’addetto al marketing può tenere traccia degli utenti, ma utilizzare un IP anonimo.

Questi metodi possono influenzare il valore e la funzionalità di Marketo in aree specifiche. Tuttavia, se l’addetto al marketing *non apporta modifiche alla configurazione di Marketo, la funzionalità Marketo rimane la stessa.*

## Impostazioni browser per Do Not Track {#browser-settings-for-do-not-track}

I visitatori web possono impostare il proprio browser per impedire il tracciamento da parte di qualsiasi sito web scegliendo &quot;Do Not Track&quot; (Non tenere traccia). Questo impedisce il tracciamento di questo particolare browser e dispositivo. Per informazioni complete, consulta le impostazioni della privacy del browser.

In Munchkin, un addetto al marketing può [decidere se supportare o ignorare l&#39;impostazione DNT del browser](/help/marketo/product-docs/administration/settings/edit-do-not-track-browser-support-settings.md).

In Personalizzazione web, un addetto al marketing può decidere se [supportare o ignorare l&#39;impostazione DNT del browser](/help/marketo/product-docs/web-personalization/getting-started/setting-web-personalization-to-do-not-track.md).

## Rinuncia da un sito Web specifico {#opt-out-from-a-specific-website}

Puoi anche consentire ai visitatori del sito di rinunciare al tracciamento dei siti web dal tuo sito web, indipendentemente dal fatto che le impostazioni **Browser Do Not Track** siano configurate o meno. Questo consente al visitatore del sito di specificare le proprie preferenze di tracciamento direttamente dal sito web.

Per fare questo, devi aggiungere un parametro a un collegamento di rinuncia su una pagina web che ha abilitato il monitoraggio dei Munchkin. Può trattarsi di qualsiasi pagina web, ma il collegamento della pagina web deve contenere il seguente parametro:

?marketo_opt_out=true

Di seguito sono riportati alcuni esempi di una pagina web con un collegamento di rinuncia e una pagina di destinazione per dopo aver fatto clic sul collegamento. Il tuo varierà.

Ecco una pagina web con un pulsante con il parametro &quot;?marketo_opt_out=true&quot; nel collegamento di rinuncia.

![](assets/opt-out-1.png)

Puoi creare e pubblicare una pagina di destinazione come pagina di follow-up per quando fai clic sul collegamento con il parametro &quot;?marketo_opt_out=true&quot;.

![](assets/opt-out-2.png)

Quando fai clic sul collegamento, Marketo aggiunge un cookie chiamato **mkto_opt_out** al browser del visitatore che disabilita il tracciamento Munchkin per il visitatore del sito che fa clic sul collegamento con il parametro precedente.

Per verificare che il cookie possa essere impiantato, accertati di essere un lead cookie e fai clic sul collegamento . Quindi controlla i cookie del browser per verificare che il cookie **mkto_opt_out** sia stato aggiunto.

![](assets/opt-out-3.png)

>[!NOTE]
>
>Attualmente funziona solo con Munchkin versioni 152 e successive.

## Consenso {#opt-in}

Gli addetti al marketing possono consentire agli utenti di effettuare il consenso utilizzando le funzionalità di Marketo nelle e-mail, nei moduli, nelle pagine di destinazione e in altri metodi.

## Tracciamento tramite un IP anonimo {#tracking-using-an-anonymized-ip}

Gli addetti al marketing possono preservare la privacy tenendo traccia degli utenti con un indirizzo IP anonimo. A tal fine, aggiungi questo codice al codice Javascript RTP o Munchkin incorporato nel sito web.

* Per Munchkin, aggiungi semplicemente {&quot;anonymizeIP&quot;,true} alla funzione init.

   >[!NOTE]
   >
   >L&#39;utilizzo di questo parametro richiede che Munchkin V2 sia abilitato. Per attivarla per l&#39;abbonamento, contatta il [Supporto Marketo](https://nation.marketo.com/community/support_solutions).

* Per la personalizzazione web (RTP, Web Personalization), aggiungi questo al codice javascript:

`anonymize IP : before calling rtp('send','view'); add rtp('set', 'settings', {'anonymizeIP' : true});`
