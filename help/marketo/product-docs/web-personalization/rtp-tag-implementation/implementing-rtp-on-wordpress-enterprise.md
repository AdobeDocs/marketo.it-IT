---
unique-page-id: 4720215
description: Implementazione di RTP su Wordpress Enterprise - Documentazione di Marketo - Documentazione del prodotto
title: Implementazione di RTP su Wordpress Enterprise
exl-id: 61cfd3f8-0811-4352-9752-0081ce19257b
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '106'
ht-degree: 0%

---

# Implementazione di RTP su Wordpress Enterprise {#implementing-rtp-on-wordpress-enterprise}

Per implementare il tag RTP, seguire le istruzioni di installazione riportate di seguito:

1. Vai a **Impostazioni account**.

   a. Se hai già ricevuto il tag JavaScript dal Supporto tecnico - continua con il passaggio 3.

   ![](assets/image2014-11-30-15-3a19-3a21-3.png)

1. In Dominio, individua il dominio pertinente e fai clic su **Genera tag**.

   ![](assets/image2014-11-30-15-3a20-3a17-3.png)

1. Copia il tag JavaScript RTP.

1. Accedi al tuo account WordPress come utente amministratore

   a. Sotto **Aspetto**, vai a **JavaScript personalizzato**.
b. Incolla il tag JavaScript RTP subito dopo il codice esistente.

   ![](assets/image2014-12-3-17-3a51-3a46.png)

   >[!CAUTION]
   >
   >Quando si incolla il codice, ESCLUDI i seguenti tag:
   >
   >* `<!-- RTP tag -->`
   >* `<script type='text/javascript'>`
   >* `</script>`
   >* `<!-- End of RTP tag -->`
   >
   >Inserire SOLO lo script stesso.

1. Clic **Aggiorna**.
