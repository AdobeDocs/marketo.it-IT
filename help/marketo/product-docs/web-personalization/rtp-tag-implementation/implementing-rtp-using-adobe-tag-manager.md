---
unique-page-id: 4720218
description: Implementazione di RTP tramite Adobe Tag Manager - Documentazione di Marketo - Documentazione del prodotto
title: Implementazione di RTP con Adobe Tag Manager
exl-id: 5a938d02-6b09-45d5-94b0-dbb50b5d62b6
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '211'
ht-degree: 0%

---

# Implementazione di RTP con Adobe Tag Manager {#implementing-rtp-using-adobe-tag-manager}

Per implementare il tag RTP, seguire le istruzioni di installazione riportate di seguito:

1. Accedi al tuo account RTP.

1. Vai a **Impostazioni account**.

   a. Se hai già ricevuto il tag JavaScript dal Supporto tecnico - continua con il passaggio 4.

   ![](assets/image2014-11-30-15-3a19-3a21-4.png)

1. In Dominio individuare il dominio pertinente e fare clic su **Genera tag**.

   ![](assets/image2014-11-30-15-3a20-3a17-4.png)

1. Accedi all&#39;account di Dynamic Tag Manager ([https://dtm.adobe.com/sign_in](https://dtm.adobe.com/sign_in)).

1. Passa al dashboard **.** Fare clic sulla relativa proprietà Web.

   ![](assets/image2014-12-3-17-3a58-3a17.png)

1. Vai a **Regole**, fai clic su **Crea nuova regola**.

1. Compila quanto segue

   1. Nome: **RTP Marketo**
   1. Condizioni (comprimi): regola di attivazione in - **Inizio pagina**
   1. Javascript (comprimi): fare clic su **Aggiungi nuovo script**

   ![](assets/image2014-12-3-17-3a59-3a40.png)

1. Chiama il nuovo tag: **Marketo RTP Tag**

1. Rimuovi il seguente codice dal tag RTP

   * `<script type='text/javascript'>`
   * `</script>`

1. Incolla il tag JavaScript RTP.

   ![](assets/image2014-12-3-18-3a3-3a45.png)

   >[!CAUTION]
   >
   >Assicurarsi di rimuovere tutti i tag e di lasciare solo lo script stesso (nessun `<script type='text/javascript'>` , `</script>` )

1. Fai clic su **Salva codice** nell&#39;editor di script e su **Salva regola** nell&#39;editor di regole.

1. Nel pannello Regole, individua la regola di caricamento pagina Marketo RTP e, nel menu a discesa **Azioni**, seleziona **Attiva regole**.

   ![](assets/image2014-12-3-18-3a4-3a14.png)

1. **Verificare** che venga visualizzato in tutte le pagine, inclusi i sottodomini e le pagine di destinazione.

   Per farlo, fai clic con il pulsante destro del mouse sulle pagine del tuo sito web. Vai a **Elemento Inspect**, fai clic su **Rete**, Cerca: **RTP**.
