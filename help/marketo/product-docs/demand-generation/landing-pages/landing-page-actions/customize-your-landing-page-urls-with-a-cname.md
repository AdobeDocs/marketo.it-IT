---
unique-page-id: 2359746
description: Personalizzare gli URL della pagina di destinazione con un CNAME - Marketo Docs - Documentazione prodotto
title: Personalizzare gli URL della pagina di destinazione con un CNAME
translation-type: tm+mt
source-git-commit: 6ae882dddda220f7067babbe5a057eec82601abf
workflow-type: tm+mt
source-wordcount: '254'
ht-degree: 0%

---


# Personalizzare gli URL della pagina di destinazione con un CNAME {#customize-your-landing-page-urls-with-a-cname}

Anche se Marketo ospita le pagine di destinazione, l’URL può essere completamente personalizzato. Che aspetto ha senza un CNAME:

`https://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html`

Il suo aspetto:

`https://go.YourCompany.com/UnsubscribePage.html`

## Scegliete un CNAME {#choose-a-cname}

Scegliete una parola da inserire all’inizio dell’URL per le pagine di destinazione. È solo una parola e dovrebbe essere relativamente breve. Esempi:

* go.YourCompany.com/NameOfPage.html
* info.YourCompany.com/NameOfPage.html
* pages.YourCompany.com/NameOfPage.html

La parola (più YourCompany.com) è denominata CNAME. Ne avrete bisogno più tardi, quindi prendetene nota.

## Trova la stringa account {#find-your-account-string}

1. Andate nell&#39;area **Admin** e fate clic su **Pagine di destinazione**.

   ![](assets/image2014-9-18-16-3a2-3a45.png)

   >[!NOTE]
   >
   >**Autorizzazioni amministratore richieste**

1. Nella scheda **Destinazione** **Pagine**, copiare l&#39;account **Account** **String** dalla sezione **Impostazioni**.

   ![](assets/image2014-9-18-16-3a44-3a12.png)

1. Avrete bisogno anche più tardi, quindi prendete nota di esso.

## Invia richiesta all&#39;IT {#send-request-to-it}

Chiedete al personale IT di configurare il seguente CNAME: (Sostituire la parola [CNAME] e [ACCOUNT STRING] con il testo del passaggio precedente.)

[CNAME].YourCompany.com >  [ACCOUNT STRING].mktoweb.com

## Impostazione CNAME completa {#complete-cname-setup}

1. Una volta che il CNAME è stato creato dal reparto IT, andate a **Admin** e fate clic su **Pagine di destinazione**.

   ![](assets/image2014-9-18-17-3a15-3a11.png)

1. Nella sezione **Impostazioni**, fare clic su **Modifica**.

   ![](assets/image2014-9-18-17-3a15-3a18.png)

1. Immettete il CNAME in **Nome di dominio per le pagine di destinazione**, immettete la pagina di fallback **File di fallback**, immettete la pagina **Homepage** e fate clic su **Salva**.

   ![](assets/image2014-9-18-17-3a15-3a25.png)

>[!NOTE]
>
>La pagina di fallback sarà il lead della pagina a cui verrà reindirizzato se la pagina di destinazione Marketo non è disponibile.

Bel lavoro! Le pagine di destinazione sono ora personalizzate con il dominio della società.
