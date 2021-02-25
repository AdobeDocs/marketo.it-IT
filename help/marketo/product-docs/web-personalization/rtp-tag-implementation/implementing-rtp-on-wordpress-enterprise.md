---
unique-page-id: 4720215
description: Implementazione di RTP su Wordpress Enterprise - Marketo Docs - Documentazione prodotto
title: Implementazione di RTP su Wordpress Enterprise
translation-type: tm+mt
source-git-commit: fbaf57ec4f3532c2d71acf23171d60873b1c997c
workflow-type: tm+mt
source-wordcount: '106'
ht-degree: 0%

---


# Implementazione di RTP su Wordpress Enterprise {#implementing-rtp-on-wordpress-enterprise}

Per implementare il tag RTP, segui le istruzioni di installazione riportate di seguito:

1. Vai a **Impostazioni account**.

   a. Se avete già ricevuto il tag JavaScript dal supporto, continuate con il passaggio 3.

   ![](assets/image2014-11-30-15-3a19-3a21-3.png)

1. In Domain (Dominio), individua il dominio appropriato e fai clic su **Generate Tag**.

   ![](assets/image2014-11-30-15-3a20-3a17-3.png)

1. Copiate il tag JavaScript RTP.

1. Accedi al tuo account WordPress come utente amministratore

   a. In **Aspetto**, passare a **JavaScript personalizzato**.
b. Incolla il tag Javascript RTP subito dopo il codice esistente.

   ![](assets/image2014-12-3-17-3a51-3a46.png)

   >[!CAUTION]
   >
   >Quando incollate il codice EXCLUDE, i seguenti tag:
   >
   >* `<!-- RTP tag -->`
   >* `<script type='text/javascript'>`
   >* `</script>`
   >* `<!-- End of RTP tag -->`

   >
   >Inserire lo script stesso SOLO.

1. Fare clic su **Aggiorna**.
