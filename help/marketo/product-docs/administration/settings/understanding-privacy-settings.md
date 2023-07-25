---
unique-page-id: 10617187
description: Informazioni sulle impostazioni della privacy - Documentazione di Marketo - Documentazione del prodotto
title: Informazioni sulle impostazioni della privacy
exl-id: 1fde9011-02a9-4ec9-bfa4-c56a52ce1eed
feature: Administration
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '514'
ht-degree: 0%

---

# Informazioni sulle impostazioni della privacy {#understanding-privacy-settings}

## Panoramica {#overview}

Marketo offre agli esperti di marketing un modo per ottenere il consenso dei visitatori web per monitorarli. Esistono due modi per rinunciare o puoi scegliere di essere tracciato da un IP anonimo.

* I visitatori Web selezionano la funzione Do Not Track (DNT) nel browser (e l’addetto al marketing rispetta la richiesta del visitatore Web di Do Not Track)
* I visitatori web utilizzano un cookie di rinuncia fornito da un addetto marketing su un sito web

In alternativa, l’addetto al marketing può tenere traccia degli utenti, ma utilizzando un IP anonimo.

Questi metodi possono influire sul valore e sulle funzionalità di Marketo in aree specifiche. Tuttavia, se l’addetto marketing _non_ cambiando qualunque cosa nella configurazione di Marketo, la funzionalità Marketo rimane la stessa.

## Impostazioni browser per Do Not Track {#browser-settings-for-do-not-track}

I visitatori possono impostare il proprio browser per impedire il tracciamento da parte di qualsiasi sito web scegliendo &quot;Do Not Track&quot; (DNT). Questo impedisce il tracciamento per questo particolare browser e dispositivo. Per informazioni dettagliate, consulta le impostazioni di privacy del browser.

In entrata [!DNL Munchkin], un addetto marketing può [decidere se supportare o ignorare l&#39;impostazione DNT del browser](/help/marketo/product-docs/administration/settings/edit-do-not-track-browser-support-settings.md).

Nella personalizzazione web, un addetto al marketing può decidere se [supporta o ignora l&#39;impostazione DNT del browser](/help/marketo/product-docs/web-personalization/getting-started/setting-web-personalization-to-do-not-track.md).

## Rinuncia a un sito Web specifico {#opt-out-from-a-specific-website}

Puoi anche consentire ai visitatori del sito di rinunciare al tracciamento del sito web dal sito, indipendentemente dal fatto che lo facciano o meno **Browser Do Not Track** impostazioni configurate. Questo consente al visitatore del sito di specificare le preferenze di tracciamento direttamente dal sito web.

A questo scopo, devi aggiungere un parametro a un collegamento di rinuncia in una pagina web con [!DNL Munchkin] tracciamento abilitato. Può essere una qualsiasi pagina Web, ma il collegamento della pagina Web deve contenere il seguente parametro:

?marketo_opt_out=true

Di seguito sono riportati alcuni esempi di pagine web con un collegamento di rinuncia e una pagina di destinazione per dopo aver fatto clic sul collegamento. Il vostro sarà diverso.

Ecco una pagina web con un pulsante con il parametro &quot;?marketo_opt_out=true&quot; nel collegamento di rinuncia.

![](assets/understanding-privacy-settings-1.png)

Puoi creare e pubblicare una pagina di destinazione come pagina di follow-up per quando fai clic sul collegamento con il parametro &quot;?marketo_opt_out=true&quot;.

![](assets/understanding-privacy-settings-2.png)

Quando fai clic sul collegamento, Marketo aggiunge un cookie denominato **mkto_opt_out** al browser del visitatore che disabilita [!DNL Munchkin] tracciamento per il visitatore del sito che fa clic sul collegamento con il parametro precedente.

Per verificare che il cookie possa essere piantato, verifica di essere un lead cookie e fai clic sul collegamento. Quindi controlla i cookie del browser per verificare che **mkto_opt_out** cookie aggiunto.

![](assets/understanding-privacy-settings-3.png)

>[!NOTE]
>
>Attualmente funziona solo con [!DNL Munchkin] versioni 152 e successive.

## Consenso {#opt-in}

Gli addetti al marketing possono consentire agli utenti di dare il consenso utilizzando le funzionalità di Marketo in e-mail, moduli, pagine di destinazione e altri metodi.

## Tracciamento tramite IP anonimo {#tracking-using-an-anonymized-ip}

Gli addetti al marketing possono preservare la privacy monitorando gli utenti con un indirizzo IP anonimo. Per farlo, aggiungi questo codice all’RTP o [!DNL Munchkin] JavaScript incorporato nel sito Web.

* Per [!DNL Munchkin], aggiungi semplicemente {&quot;anonymizeIP&quot;,true} alla funzione init.

  >[!NOTE]
  >
  >L&#39;utilizzo di questo parametro richiede che [!DNL Munchkin] V2. Per abilitarlo per l’abbonamento, contatta [Supporto Marketo](https://nation.marketo.com/community/support_solutions).

* Per la personalizzazione web (RTP), aggiungi questo al codice JavaScript:

`anonymize IP : before calling rtp('send','view'); add rtp('set', 'settings', {'anonymizeIP' : true});`
