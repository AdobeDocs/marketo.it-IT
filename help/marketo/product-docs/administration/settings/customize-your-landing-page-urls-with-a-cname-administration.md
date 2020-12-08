---
unique-page-id: 2360189
description: Personalizzare gli URL delle pagine di destinazione con un CNAME (Amministrazione) - Marketo Docs - Documentazione prodotto
title: Personalizzare gli URL della pagina di destinazione con un CNAME (Amministrazione)
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---


# Personalizzare gli URL della pagina di destinazione con un CNAME (Amministrazione) {#customize-your-landing-page-urls-with-a-cname-administration}

Anche se Marketo ospita le pagine di destinazione, l’URL deve essere personalizzato per la società.

>[!NOTE]
>
>**Esempio**
>
>Nessun CNAME:
>
>http://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html
>
>CNAME con marchio:
>
>http://go.**YourCompany**.com/UnsuscribePage.html

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

Prepariamoci!

1. Scegliere un CNAME

   È la parte anteriore dell&#39;URL. Esempi:

   * **vai**.YourCompany.com/NameOfPage.html
   * **info**.YourCompany.com/NameOfPage.html
   * **pagine**.YourCompany.com/NameOfPage.html

   La parola (più YourCompany.com) è denominata CNAME. Ne avrete bisogno in un secondo momento, quindi prendetene nota.

1. Trova la stringa account
1. Andate nell&#39;area **Admin** e fate clic su Pagine **di** destinazione.

   ![](assets/image2014-9-16-13-3a9-3a44.png)

1. Nella scheda **Pagine di destinazione **, copiare la Stringa account dalla sezione Impostazioni.

   ![](assets/image2014-9-16-13-3a9-3a57.png)

1. Ne avrete bisogno anche in seguito, quindi prendete nota.
1. Invia richiesta all&#39;IT
1. Chiedete al personale IT di impostare il seguente CNAME (sostituite la parola [CNAME] e STRING [] ACCOUNT con il testo del passaggio precedente):

   [CNAME].YourCompany.com > [ACCOUNT STRING].mktoweb.com

1. Impostazione completa CNAME
1. Una volta che il CNAME è stato creato dal reparto IT, accedi ad **Admin** e fai clic su Pagine **di** destinazione.

   ![](assets/image2014-9-16-13-3a10-3a14.png)

1. Nella sezione **Impostazioni** , fate clic su **Modifica**.

   ![](assets/image2014-9-16-13-3a10-3a31.png)

1. Immettete il CNAME nel nome **di dominio per le pagine** di destinazione, immettete la pagina **di** fallback, immettete la **homepage** e fate clic su **Salva**.

   ![](assets/image2014-9-16-13-3a10-3a45.png)

   La pagina di fallback contiene il reindirizzamento delle persone se la pagina di destinazione Marketo non è disponibile.
Bel lavoro! Le pagine di destinazione sono ora personalizzate con il dominio della società.

