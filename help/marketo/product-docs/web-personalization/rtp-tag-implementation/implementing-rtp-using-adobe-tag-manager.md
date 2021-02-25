---
unique-page-id: 4720218
description: Implementazione di RTP tramite  Adobe Tag Manager - Marketo Docs - Documentazione prodotto
title: Implementazione di RTP con  Adobe Tag Manager
translation-type: tm+mt
source-git-commit: fbaf57ec4f3532c2d71acf23171d60873b1c997c
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---


# Implementazione di RTP con  Adobe Tag Manager {#implementing-rtp-using-adobe-tag-manager}

Per implementare il tag RTP, segui le istruzioni di installazione riportate di seguito:

1. Accedi al tuo account RTP.

1. Vai a **Impostazioni account**.

   a. Se avete già ricevuto il tag JavaScript dal supporto, continuate con il passaggio 4.

   ![](assets/image2014-11-30-15-3a19-3a21-4.png)

1. In Domain (Dominio), individua il dominio appropriato e fai clic su **Generate Tag**.

   ![](assets/image2014-11-30-15-3a20-3a17-4.png)

1. Accedi al tuo account Dynamic Tag Manager ([https://dtm.adobe.com/sign_in](https://dtm.adobe.com/sign_in)).

1. Vai a **Dashboard.** Fare clic sulla proprietà Web corrispondente.

   ![](assets/image2014-12-3-17-3a58-3a17.png)

1. Vai a **Regole**, fai clic su **Crea nuova regola**.

1. Compila quanto segue

   1. Nome: **Marketo RTP**
   1. Condizioni (crollo) : Regola di attivazione in - **Parte superiore pagina**
   1. Javascript (compresso): fare clic su **Aggiungi nuovo script**

   ![](assets/image2014-12-3-17-3a59-3a40.png)

1. Chiama il nuovo tag: **Tag Marketo RTP**

1. Rimuovi il seguente codice dal tag RTP

   * `<script type='text/javascript'>`
   * `</script>`

1. Incollate il tag JavaScript RTP.

   ![](assets/image2014-12-3-18-3a3-3a45.png)

   >[!CAUTION]
   >
   >Rimuovere tutti i tag e lasciare solo lo script (no `<script type='text/javascript'>` , `</script>` )

1. Fare clic su **Salva codice** nell&#39;editor di script e su **Salva regola** nell&#39;editor di regole.

1. Nel pannello Regole, individuare la regola di caricamento della pagina Marketo RTP e nel menu a discesa **Actions** selezionare **Activate Rules** (Attiva regole).

   ![](assets/image2014-12-3-18-3a4-3a14.png)

1. **Verificate** che venga visualizzato su tutte le pagine, incluse le pagine di destinazione e i sottodomini.

   Per farlo, fate clic con il pulsante destro del mouse sulle pagine del sito Web. Vai a **Inspect Element**, fai clic su **Rete**, Cerca: **RTP**.
