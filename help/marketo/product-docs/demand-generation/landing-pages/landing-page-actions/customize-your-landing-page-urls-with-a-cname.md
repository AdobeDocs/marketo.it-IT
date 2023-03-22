---
unique-page-id: 2359746
description: Personalizzare gli URL della pagina di destinazione con un CNAME - Marketo Docs - Documentazione del prodotto
title: Personalizzare gli URL della pagina di destinazione con un CNAME
exl-id: 2cd87785-61e5-46cd-b1e0-6fbc145014d4
source-git-commit: 6c1699ce986608e8b9d991f21fd649f9330e3d12
workflow-type: tm+mt
source-wordcount: '237'
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

## Trova il tuo Munchkin ID {#find-your-munchkin-id}

1. Vai a **Amministratore** area.

   ![](assets/customize-your-landing-page-urls-with-a-cname-1.png)

1. Fai clic su **Il mio account**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-2.png)

   >[!NOTE]
   >
   >**Autorizzazioni amministratore richieste**

1. Scorri verso il basso fino a &quot;Informazioni di supporto&quot; e copia il tuo Munchkin ID.

   ![](assets/customize-your-landing-page-urls-with-a-cname-3.png)

## Invia richiesta all&#39;IT {#send-request-to-it}

Chiedi al tuo personale IT di configurare il seguente CNAME: (Sostituisci la parola [CNAME] e [ID Munchkin] con il testo del passaggio precedente).

[CNAME].YourCompany.com > [ID Munchkin].mktoweb.com

## Configurazione completa CNAME {#complete-cname-setup}

1. Una volta creato il CNAME, passa alla pagina **Amministratore** area.

   ![](assets/customize-your-landing-page-urls-with-a-cname-4.png)

1. Fai clic su **Pagine di destinazione**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-5.png)

1. Sotto la **Impostazioni** sezione, fai clic su **Modifica**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-6.png)

1. Immetti il tuo CNAME in **Nome di dominio per le pagine di destinazione**, inserisci il **Pagina di fallback**, inserisci il **Homepage** e fai clic su **Salva**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-7.png)

>[!NOTE]
>
>Se la pagina di destinazione di Marketo non è disponibile, i lead di pagina vengono reindirizzati a .

Bel lavoro! Le pagine di destinazione sono ora contrassegnate con il marchio del dominio aziendale.
