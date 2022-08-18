---
description: Configurazione di reCAPTCHA v3 - Marketo Docs - Documentazione del prodotto
title: Configurazione reCAPTCHA v3
hide: true
hidefromtoc: true
exl-id: 235a2688-59a8-4827-a929-a07f3ae06988
source-git-commit: ccc62b22f260293ac193ce03a31e4f03aba34768
workflow-type: tm+mt
source-wordcount: '204'
ht-degree: 0%

---

# Configurazione reCAPTCHA v3 {#setting-up-recaptcha-v3}

Testo introduttivo

## Configurazione iniziale di reCAPTCHA v3 {#initial-recaptcha-v3-setup}

Testo: Descrizione v3 : i seguenti passaggi vengono eseguiti al di fuori del Marketo Engage.

1. Vai a [https://www.google.com/recaptcha/about/](https://www.google.com/recaptcha/about/){target=&quot;_blank&quot;} e fai clic sull&#39;Admin Console v3.

1. Accedi/registrati con un account Google.

1. Fai clic sul pulsante Crea (+) per creare una nuova chiave.

1. Crea un’etichetta per identificare la chiave da utilizzare come Marketo Engage.

1. Scegli tipo **reCAPTCHA v3**. Al momento il Marketo Engage non supporta reCAPTCHA v2.

1. Aggiungi ogni dominio utilizzato dalla sottoscrizione del Marketo Engage. I domini non impostati qui restituiranno errori nei moduli in cui è abilitato reCAPTCHA.

   * 123-ABC-456.mktoweb.com
   * app-pod.marketo.com
   * qualsiasi dominio e alias della pagina di destinazione configurato nella sottoscrizione

1. Imposta un proprietario e un indirizzo e-mail aggiuntivo che deve ricevere eventuali avvisi sul servizio.

1. Accettare i termini di servizio reCAPTCHA.

1. Fai clic su **Invia**.

>[!NOTE]
>
>Mantieni la chiave del sito e la chiave segreta a portata di mano per la configurazione del Marketo Engage.

## Impostazione del CAPTCHA nel Marketo Engage {#setting-up-captcha-in-marketo-engage}

1. In Marketo, fai clic su **Amministratore**.

   ![](assets/setting-up-recaptcha-v3-1.png)

1. Seleziona **CAPTCHA** nell&#39;albero.

   ![](assets/setting-up-recaptcha-v3-2.png)

1. Fai clic su **Modifica** sulle impostazioni CAPTCHA.

   ![](assets/setting-up-recaptcha-v3-3.png)

1. Fai clic sull’elenco a discesa CAPTCHA e scegli reCAPTCHA v3.

   ![](assets/setting-up-recaptcha-v3-4.png)

1. Inserire la chiave segreta e la chiave del sito. Fai clic su **Salva** al termine.

   ![](assets/setting-up-recaptcha-v3-5.png)
