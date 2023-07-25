---
unique-page-id: 2360189
description: Personalizzare gli URL della pagina di destinazione con un CNAME (Amministrazione) - Documentazione di Marketo - Documentazione del prodotto
title: Personalizzare gli URL della pagina di destinazione con un CNAME (amministrazione)
exl-id: a5aa1c76-15f7-4e8c-a736-77c79f65c368
feature: Administration
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 0%

---

# Personalizzare gli URL della pagina di destinazione con un CNAME  {#customize-your-landing-page-urls-with-a-cname}

Anche se Marketo ospita le pagine di destinazione, l’URL deve essere personalizzato per la tua azienda.

>[!NOTE]
>
>Nessun CNAME:
>
>https://na-sj02.marketo.com/lp/mktodemoaccount126/UnsubscribePage.html
>
>CNAME con marchio:
>
>https://go.**La tua azienda**.com/UnsuscribePage.html

>[!NOTE]
>
>**Autorizzazioni amministratore richieste**

Prepariamoci!

1. Scegli un CNAME.

   È la parte anteriore dell&#39;URL. Esempi:

   * **vai**.YourCompany.com/NameOfPage.html
   * **info**.YourCompany.com/NameOfPage.html
   * **pagine**.YourCompany.com/NameOfPage.html

   L’unica parola (più YourCompany.com) è denominata CNAME. Ne avrai bisogno in seguito, quindi prendi nota.

1. Trova la stringa del tuo account.

1. Vai a **[!UICONTROL Amministratore]** area.

   ![](assets/customize-your-landing-page-urls-with-a-cname-1.png)

1. Clic **[!UICONTROL Pagine di destinazione]**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-2.png)

1. Sotto **[!UICONTROL Pagine di destinazione]** , copia la stringa dell&#39;account dalla sezione Impostazioni.

   ![](assets/customize-your-landing-page-urls-with-a-cname-3.png)

1. Ne avrai bisogno anche in seguito, quindi prendi nota.

1. Invia una richiesta al reparto IT.

1. Chiedi al tuo staff IT di configurare il seguente CNAME (sostituisci la parola [CNAME] e [STRINGA ACCOUNT] con il testo del passaggio precedente):

   [CNAME].YourCompany.com > [STRINGA ACCOUNT].mktoweb.com

1. Completa la configurazione CNAME.

1. Una volta che il reparto di IT ha creato il CNAME, torna al **[!UICONTROL Amministratore]** area.

   ![](assets/customize-your-landing-page-urls-with-a-cname-4.png)

1. Clic **[!UICONTROL Pagine di destinazione]**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-5.png)

1. Sotto **[!UICONTROL Impostazioni]** , fare clic su **[!UICONTROL Modifica]**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-6.png)

1. Immetti il CNAME in **[!UICONTROL Nome di dominio per le pagine di destinazione]**, immetti il **[!UICONTROL Pagina di fallback]**, immetti il **[!UICONTROL Homepage]** e fai clic su **[!UICONTROL Salva]**.

   ![](assets/customize-your-landing-page-urls-with-a-cname-7.png)

Se la pagina di destinazione di Marketo non è disponibile, le persone verranno reindirizzate alla pagina di fallback.

Bel lavoro! Le pagine di destinazione ora sono contrassegnate con il dominio della tua azienda.
