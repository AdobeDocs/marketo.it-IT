---
unique-page-id: 2359746
description: Personalizzare gli URL della pagina di destinazione con un CNAME - Marketo Docs - Documentazione del prodotto
title: Personalizzare gli URL della pagina di destinazione con un CNAME
exl-id: 2cd87785-61e5-46cd-b1e0-6fbc145014d4
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 0%

---

# Personalizzare gli URL della pagina di destinazione con un CNAME {#customize-your-landing-page-urls-with-a-cname}

Anche se Marketo ospita le pagine di destinazione, l’URL può essere completamente personalizzato. Che aspetto ha senza un CNAME:

`https://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html`

Dovrebbe essere così:

`https://go.YourCompany.com/UnsubscribePage.html`

## Scegli un CNAME {#choose-a-cname}

Scegli una parola da inserire all’inizio dell’URL per le pagine di destinazione. È solo una parola e dovrebbe essere relativamente breve. Esempi:

* go.YourCompany.com/NameOfPage.html
* info.YourCompany.com/NameOfPage.html
* pages.YourCompany.com/NameOfPage.html

La parola (più YourCompany.com) è denominata CNAME. Ne avrai bisogno più tardi, quindi prendine nota.

## Trova la stringa account {#find-your-account-string}

1. Vai a **Amministratore** e fai clic su **Pagine di destinazione**.

   ![](assets/image2014-9-18-16-3a2-3a45.png)

   >[!NOTE]
   >
   >**Autorizzazioni amministratore richieste**

1. Sotto la **Atterraggio** **Pagine** , copia il **Account** **Stringa** dal **Impostazioni** sezione .

   ![](assets/image2014-9-18-16-3a44-3a12.png)

1. Avrete bisogno anche più tardi, quindi prendete una nota di esso.

## Invia richiesta all&#39;IT {#send-request-to-it}

Chiedi al tuo personale IT di configurare il seguente CNAME: (Sostituisci la parola [CNAME] e [STRINGA ACCOUNT] con il testo del passaggio precedente).

[CNAME].YourCompany.com > [STRINGA ACCOUNT].mktoweb.com

## Configurazione completa CNAME {#complete-cname-setup}

1. Una volta creato il CNAME, vai a **Amministratore** e fai clic su **Pagine di destinazione**.

   ![](assets/image2014-9-18-17-3a15-3a11.png)

1. Sotto la **Impostazioni** sezione, fai clic su **Modifica**.

   ![](assets/image2014-9-18-17-3a15-3a18.png)

1. Immetti il tuo CNAME in **Nome di dominio per le pagine di destinazione**, inserisci il **Pagina di fallback**, inserisci il **Homepage** e fai clic su **Salva**.

   ![](assets/image2014-9-18-17-3a15-3a25.png)

>[!NOTE]
>
>Se la pagina di destinazione di Marketo non è disponibile, i lead di pagina vengono reindirizzati a .

Bel lavoro! Le pagine di destinazione sono ora contrassegnate con il marchio del dominio aziendale.
