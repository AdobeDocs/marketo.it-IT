---
unique-page-id: 2359746
description: Personalizzare gli URL della pagina di destinazione con un CNAME - Documentazione di Marketo - Documentazione del prodotto
title: Personalizzare gli URL della pagina di destinazione con un CNAME
exl-id: 2cd87785-61e5-46cd-b1e0-6fbc145014d4
feature: Landing Pages
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '237'
ht-degree: 0%

---

# Personalizzare gli URL della pagina di destinazione con un CNAME {#customize-your-landing-page-urls-with-a-cname}

Anche se Marketo ospita le tue pagine di destinazione, l’URL può essere completamente personalizzato. Come si presenta senza un CNAME:

`https://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html`

Il suo aspetto:

`https://go.YourCompany.com/UnsubscribePage.html`

## Scegli un CNAME {#choose-a-cname}

Scegli una parola all’inizio dell’URL per le pagine di destinazione. È solo una parola e dovrebbe essere relativamente breve. Esempi:

* go.YourCompany.com/NameOfPage.html
* info.YourCompany.com/NameOfPage.html
* pages.YourCompany.com/NameOfPage.html

L’unica parola (più YourCompany.com) è denominata CNAME. Ne avrai bisogno più tardi, quindi prendi nota.

## Ricerca dell&#39;ID Munchkin {#find-your-munchkin-id}

1. Vai a **Amministratore** area.

   ![](assets/customize-your-landing-page-urls-with-a-cname-1.png)

1. Clic **Il mio account**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-2.png)

   >[!NOTE]
   >
   >**Autorizzazioni amministratore richieste**

1. Scorri verso il basso fino a &quot;Informazioni di supporto&quot; e copia il tuo ID Munchkin.

   ![](assets/customize-your-landing-page-urls-with-a-cname-3.png)

## Invia richiesta al reparto IT {#send-request-to-it}

Chiedi al tuo personale IT di configurare il seguente CNAME: (Sostituisci la parola [CNAME] e [ID Munchkin] con il testo del passaggio precedente.)

[CNAME].YourCompany.com > [ID Munchkin].mktoweb.com

## Completare l’impostazione di CNAME {#complete-cname-setup}

1. Una volta creato il CNAME da parte del reparto IT, vai al **Amministratore** area.

   ![](assets/customize-your-landing-page-urls-with-a-cname-4.png)

1. Clic **Pagine di destinazione**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-5.png)

1. Sotto **Impostazioni** , fare clic su **Modifica**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-6.png)

1. Immetti il CNAME in **Nome di dominio per le pagine di destinazione**, immetti il **Pagina di fallback**, immetti il **Homepage** e fai clic su **Salva**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-7.png)

>[!NOTE]
>
>La pagina di fallback sarà quella a cui verranno reindirizzati i lead di pagina se la pagina di destinazione di Marketo non è disponibile.

Bel lavoro! Le pagine di destinazione ora sono contrassegnate con il dominio della tua azienda.
