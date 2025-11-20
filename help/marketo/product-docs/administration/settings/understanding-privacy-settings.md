---
unique-page-id: 10617187
description: Informazioni sulle impostazioni della privacy - Documentazione di Marketo - Documentazione del prodotto
title: Informazioni sulle impostazioni della privacy
exl-id: 1fde9011-02a9-4ec9-bfa4-c56a52ce1eed
feature: Administration
source-git-commit: eccf4a66f5d3c581a82a363918b40ae37aa73576
workflow-type: tm+mt
source-wordcount: '479'
ht-degree: 1%

---

# Informazioni sulle impostazioni della privacy {#understanding-privacy-settings}

## Panoramica {#overview}

Marketo offre agli esperti di marketing un modo per ottenere il consenso dei visitatori web per monitorarli. Esistono due modi per rinunciare o puoi scegliere di essere tracciato da un IP anonimo.

* I visitatori Web selezionano la funzione Do Not Track (DNT) nel browser (e l’addetto al marketing rispetta la richiesta del visitatore Web di Do Not Track)
* I visitatori web utilizzano un cookie di rinuncia fornito da un addetto marketing su un sito web

In alternativa, l’addetto al marketing può tenere traccia degli utenti, ma utilizzando un IP anonimo.

Questi metodi possono influire sul valore e sulle funzionalità di Marketo in aree specifiche. Tuttavia, se l&#39;addetto marketing _non modifica_ nulla nella configurazione di Marketo, la funzionalità di Marketo rimane invariata.

## Impostazioni browser per Do Not Track {#browser-settings-for-do-not-track}

I visitatori possono impostare il proprio browser per impedire il tracciamento da parte di qualsiasi sito web scegliendo &quot;Do Not Track&quot; (DNT). Questo impedisce il tracciamento per questo particolare browser e dispositivo. Per informazioni dettagliate, consulta le impostazioni di privacy del browser.

In [!DNL Munchkin] un addetto marketing può [decidere se supportare o ignorare l&#39;impostazione DNT del browser](/help/marketo/product-docs/administration/settings/edit-do-not-track-browser-support-settings.md).

In Web Personalization, un addetto al marketing può decidere se [supportare o ignorare l&#39;impostazione DNT del browser](/help/marketo/product-docs/web-personalization/getting-started/setting-web-personalization-to-do-not-track.md).

## Rinuncia a un sito Web specifico {#opt-out-from-a-specific-website}

Puoi anche consentire ai visitatori del sito di rinunciare al monitoraggio del sito Web dal sito Web, indipendentemente dal fatto che le impostazioni **Browser Do Not Track** siano configurate o meno. Questo consente al visitatore del sito di specificare le preferenze di tracciamento direttamente dal sito web.

Per eseguire questa operazione, è necessario aggiungere un parametro a un collegamento di rinuncia in una pagina Web in cui è abilitato il monitoraggio di [!DNL Munchkin]. Può essere una qualsiasi pagina Web, ma il collegamento della pagina Web deve contenere il seguente parametro:

?marketo_opt_out=true

Di seguito sono riportati alcuni esempi di pagine web con un collegamento di rinuncia e una pagina di destinazione per dopo aver fatto clic sul collegamento. Il vostro sarà diverso.

Ecco una pagina web con un pulsante con il parametro &quot;?marketo_opt_out=true&quot; nel collegamento di rinuncia.

![](assets/understanding-privacy-settings-1.png)

Puoi creare e pubblicare una pagina di destinazione come pagina di follow-up per quando fai clic sul collegamento con il parametro &quot;?marketo_opt_out=true&quot;.

![](assets/understanding-privacy-settings-2.png)

Quando si fa clic sul collegamento, Marketo aggiunge un cookie denominato **mkto_opt_out** al browser del visitatore che disabilita il monitoraggio di [!DNL Munchkin] per il visitatore del sito che fa clic sul collegamento con il parametro precedente.

Per verificare che il cookie possa essere piantato, verifica di essere un lead cookie e fai clic sul collegamento. Controlla quindi i cookie del browser per verificare che sia stato aggiunto il cookie **mkto_opt_out**.

![](assets/understanding-privacy-settings-3.png)

>[!NOTE]
>
>Attualmente funziona solo con [!DNL Munchkin] versioni 152 e successive.

## Consenso accordato {#opt-in}

Gli addetti al marketing possono consentire agli utenti di dare il consenso utilizzando le funzionalità di Marketo in e-mail, moduli, pagine di destinazione e altri metodi.

## Tracciamento tramite IP anonimo {#tracking-using-an-anonymized-ip}

Gli addetti al marketing possono preservare la privacy monitorando gli utenti con un indirizzo IP anonimo. Per eseguire questa operazione, aggiungere il codice all&#39;RTP o al JavaScript [!DNL Munchkin] incorporato nel sito Web.

* Per [!DNL Munchkin], aggiungi `{"anonymizeIP",true}` alla funzione [init](https://experienceleague.adobe.com/it/docs/marketo-developer/marketo/javascriptapi/leadtracking/configuration){target="_blank"}.

* Per Web Personalization (RTP), aggiungi questo al codice JavaScript:

`anonymize IP : before calling rtp('send','view'); add rtp('set', 'settings', {'anonymizeIP' : true});`
