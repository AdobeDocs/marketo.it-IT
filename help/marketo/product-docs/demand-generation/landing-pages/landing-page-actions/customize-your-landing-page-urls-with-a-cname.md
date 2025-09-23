---
unique-page-id: 2359746
description: Personalizzare gli URL della pagina di destinazione con un CNAME - Documentazione di Marketo - Documentazione del prodotto
title: Personalizzare gli URL della pagina di destinazione con un CNAME
exl-id: 2cd87785-61e5-46cd-b1e0-6fbc145014d4
feature: Landing Pages
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '228'
ht-degree: 7%

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

## Trova il tuo Munchkin ID {#find-your-munchkin-id}

1. Vai all&#39;area **Amministratore**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-1.png)

1. Fai clic su **Il mio account**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-2.png)

   >[!NOTE]
   >
   >**Autorizzazioni amministratore richieste**

1. Scorri verso il basso fino a &quot;Informazioni di supporto&quot; e copia il tuo Munchkin ID.

   ![](assets/customize-your-landing-page-urls-with-a-cname-3.png)

## Invia richiesta al reparto IT {#send-request-to-it}

Chiedi al tuo personale IT di configurare il seguente CNAME: (sostituisci la parola [CNAME] e [Munchkin ID] con il testo del passaggio precedente).

[CNAME].YourCompany.com > [Munchkin ID].mktoweb.com

## Completare l’impostazione di CNAME {#complete-cname-setup}

1. Una volta creato il CNAME da parte del reparto IT, vai all&#39;area **Amministratore**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-4.png)

1. Fai clic su **Pagine di destinazione**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-5.png)

1. Nella sezione **Impostazioni**, fai clic su **Modifica**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-6.png)

1. Immetti il tuo CNAME in **[!UICONTROL Domain name for Landing Pages]**, immetti il tuo **[!UICONTROL Fallback page]**, immetti il tuo **[!UICONTROL Homepage]** e fai clic su **[!UICONTROL Save]**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-7.png)

>[!NOTE]
>
>La pagina di fallback sarà quella a cui verranno reindirizzati i lead di pagina se la pagina di destinazione di Marketo non è disponibile.

Bel lavoro! Le pagine di destinazione ora sono contrassegnate con il dominio della tua azienda.
