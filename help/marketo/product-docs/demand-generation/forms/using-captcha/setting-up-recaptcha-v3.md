---
description: Configurazione di reCAPTCHA v3 - Documentazione di Marketo - Documentazione del prodotto
title: Configurazione di reCAPTCHA v3
exl-id: 235a2688-59a8-4827-a929-a07f3ae06988
feature: Forms
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 2%

---

# Configurazione di [!UICONTROL reCAPTCHA v3] {#setting-up-recaptcha-v3}

ReCAPTCHA v3 è un’esperienza senza attriti che classifica gli invii di moduli in base a quanto siano sospetti senza l’utilizzo di testo, immagini o pulsanti. [Ulteriori informazioni](https://developers.google.com/search/blog/2018/10/introducing-recaptcha-v3-new-way-to){target="_blank"}.

## Recupera [!UICONTROL Data Center] e [!UICONTROL Munchkin ID] {#retrieve-your-data-center-and-munchkin-id}

Per il passaggio 6 della sezione Configurazione iniziale di [!UICONTROL reCAPTCHA v3] di seguito, sono necessari i [!UICONTROL Data Center] e i [!UICONTROL Munchkin ID] della sottoscrizione Marketo Engage. Ecco come trovarli.

1. In Marketo, fare clic su **[!UICONTROL Admin]**.

   ![](assets/setting-up-recaptcha-v3-1.png)

1. Fai clic su **[!UICONTROL My Account]**.

   ![](assets/setting-up-recaptcha-v3-2.png)

1. Scorri verso il basso fino a [!UICONTROL Support Information].

   ![](assets/setting-up-recaptcha-v3-3.png)

## Configurazione iniziale di [!UICONTROL reCAPTCHA v3] {#initial-recaptcha-v3-setup}

I seguenti passaggi vengono eseguiti al di fuori di Marketo.

1. Vai a [https://www.google.com/recaptcha/about/](https://www.google.com/recaptcha/about/){target="_blank"} e fai clic su v3 Admin Console.

1. Accedi/registrati con un account Google.

1. Fare clic sul pulsante [!UICONTROL Create] (+) per creare una nuova chiave.

1. Crea un’etichetta per identificare la chiave da utilizzare per Marketo Engage.

1. Scegliere il tipo **[!UICONTROL reCAPTCHA v3]**. Marketo Engage non supporta reCAPTCHA v2.

1. Aggiungi ogni dominio utilizzato dalla sottoscrizione Marketo Engage. I domini non impostati qui restituiranno errori nei moduli in cui è abilitato reCAPTCHA. Ricorda di sostituire le parole &quot;datacenter&quot; e &quot;munchkinID&quot; con i [dati nella sottoscrizione](#retrieve-your-data-center-and-munchkin-id).

   * app-datacenter.marketo.com
   * munchkinID.mktoweb.com
   * qualsiasi dominio e alias della pagina di destinazione configurato nella sottoscrizione

   >[!NOTE]
   >
   >Ad esempio, se il [!UICONTROL Data Center] dell&#39;account è &quot;sjst&quot;, il dominio da inserire nell&#39;elenco Consentiti sarà `app-sjst.marketo.com`. Se [!UICONTROL Munchkin ID] è 123-ABC-789, il dominio da inserire nell&#39;elenco Consentiti sarà `123-ABC-789.mktoweb.com`.

1. Imposta un proprietario e un indirizzo e-mail aggiuntivo a cui inviare eventuali avvisi relativi al servizio.

1. Accetta i termini di servizio reCAPTCHA.

1. Fai clic su **[!UICONTROL Submit]**.

   >[!NOTE]
   >
   >Mantieni a portata di mano la chiave del sito e la chiave segreta per la configurazione di Marketo Engage.

## Configurazione di CAPTCHA in Marketo Engage {#setting-up-captcha-in-marketo-engage}

>[!IMPORTANT]
>
>Dopo aver eseguito questi passaggi e aver [abilitato CAPTCHA nel primo Marketo form](/help/marketo/product-docs/demand-generation/forms/using-captcha/enable-captcha-in-marketo-forms.md){target="_blank"}, assicurarsi di verificare immediatamente il modulo in quanto qualsiasi configurazione errata nella configurazione di reCAPTCHA potrebbe interrompere il modulo.

1. In Marketo, fare clic su **[!UICONTROL Admin]**.

   ![](assets/setting-up-recaptcha-v3-4.png)

1. Selezionare **[!UICONTROL CAPTCHA]** nella struttura.

   ![](assets/setting-up-recaptcha-v3-5.png)

1. Fare clic su **[!UICONTROL Edit]** nelle impostazioni di [!UICONTROL CAPTCHA].

   ![](assets/setting-up-recaptcha-v3-6.png)

1. Fare clic sull&#39;elenco a discesa [!UICONTROL CAPTCHA] e scegliere [!UICONTROL reCAPTCHA v3].

   ![](assets/setting-up-recaptcha-v3-7.png)

1. Inserire **[!UICONTROL Secret Key]** e **[!UICONTROL Site Key]**. Al termine, fai clic su **[!UICONTROL Save]**.

   ![](assets/setting-up-recaptcha-v3-8.png)

>[!MORELIKETHIS]
>
>[Abilitare CAPTCHA in Marketo Forms](/help/marketo/product-docs/demand-generation/forms/using-captcha/enable-captcha-in-marketo-forms.md)
