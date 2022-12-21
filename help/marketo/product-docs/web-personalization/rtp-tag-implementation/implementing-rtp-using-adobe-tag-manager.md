---
unique-page-id: 4720218
description: Implementazione di RTP con Adobe Tag Manager - Documentazione Marketo - Documentazione del prodotto
title: Implementazione di RTP con Adobe Tag Manager
exl-id: 5a938d02-6b09-45d5-94b0-dbb50b5d62b6
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---

# Implementazione di RTP con Adobe Tag Manager {#implementing-rtp-using-adobe-tag-manager}

Per implementare il tag RTP, segui le istruzioni di installazione riportate di seguito:

1. Accedi al tuo account RTP.

1. Vai a **Impostazioni account**.

   a) Se hai già ricevuto il tag JavaScript dal supporto - continua con il passaggio 4.

   ![](assets/image2014-11-30-15-3a19-3a21-4.png)

1. In Dominio, individua il dominio pertinente e fai clic su **Genera tag**.

   ![](assets/image2014-11-30-15-3a20-3a17-4.png)

1. Accedi al tuo account Dynamic Tag Manager ([https://dtm.adobe.com/sign_in](https://dtm.adobe.com/sign_in)).

1. Vai a **Dashboard.** Fare clic sulla proprietà Web corrispondente.

   ![](assets/image2014-12-3-17-3a58-3a17.png)

1. Vai a **Regole**, fai clic su **Crea nuova regola**.

1. Compila quanto segue

   1. Nome: **Marketo RTP**
   1. Condizioni (collasso) : Regola di attivazione a - **Parte superiore pagina**
   1. Javascript (compresso): click **Aggiungi nuovo script**

   ![](assets/image2014-12-3-17-3a59-3a40.png)

1. Chiama il nuovo tag: **Tag RTP di Marketo**

1. Rimuovi il seguente codice dal tag RTP

   * `<script type='text/javascript'>`
   * `</script>`

1. Incolla il tag JavaScript RTP.

   ![](assets/image2014-12-3-18-3a3-3a45.png)

   >[!CAUTION]
   >
   >Assicurati di rimuovere tutti i tag e lasciare solo lo script stesso (no `<script type='text/javascript'>` , `</script>` )

1. Fai clic su **Salva codice** nell’editor di script e **Salva regola** nell’editor di regole.

1. Nel pannello Regole , individua la regola di caricamento della pagina RTP di Marketo e all’interno della **Azioni** selezione a discesa **Attiva regole**.

   ![](assets/image2014-12-3-18-3a4-3a14.png)

1. **Verifica** che venga visualizzato su tutte le pagine, incluse le pagine di destinazione e i sottodomini.

   Per farlo, fai clic con il pulsante destro del mouse sulle pagine del sito web. Vai a **Elemento Inspect**, fai clic su **Rete**, Cerca: **RTP**.
