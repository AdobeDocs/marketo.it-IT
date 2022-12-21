---
unique-page-id: 4720215
description: Implementazione di RTP su Wordpress Enterprise - Marketo Docs - Documentazione del prodotto
title: Implementazione di RTP su Wordpress Enterprise
exl-id: 61cfd3f8-0811-4352-9752-0081ce19257b
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '106'
ht-degree: 0%

---

# Implementazione di RTP su Wordpress Enterprise {#implementing-rtp-on-wordpress-enterprise}

Per implementare il tag RTP, segui le istruzioni di installazione riportate di seguito:

1. Vai a **Impostazioni account**.

   a) Se hai già ricevuto il tag JavaScript dal supporto - continua con il passaggio 3.

   ![](assets/image2014-11-30-15-3a19-3a21-3.png)

1. In Dominio, individua il dominio pertinente e fai clic su **Genera tag**.

   ![](assets/image2014-11-30-15-3a20-3a17-3.png)

1. Copia il tag JavaScript RTP.

1. Accedi al tuo account WordPress come utente amministratore

   a) Sotto **Aspetto**, vai a **JavaScript personalizzato**.
b) Incolla il tag Javascript RTP subito dopo il codice esistente.

   ![](assets/image2014-12-3-17-3a51-3a46.png)

   >[!CAUTION]
   >
   >Quando incolla il codice ESCLUDI i seguenti tag:
   >
   >* `<!-- RTP tag -->`
   >* `<script type='text/javascript'>`
   >* `</script>`
   >* `<!-- End of RTP tag -->`

   >
   >Inserire lo script stesso SOLO.

1. Fai clic su **Aggiorna**.
