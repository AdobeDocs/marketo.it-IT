---
unique-page-id: 4720149
description: Implementazione di RTP su Wordpress - Documentazione di Marketo - Documentazione del prodotto
title: Implementazione di RTP su Wordpress
exl-id: f010942b-02bb-447b-a272-c4237782b2d7
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '187'
ht-degree: 0%

---

# Implementazione di RTP su Wordpress {#implementing-rtp-on-wordpress}

Per implementare il tag RTP, seguire le istruzioni di installazione riportate di seguito:

1. Apri il **header.php** file del tuo **Tema WordPress**.

   Potete utilizzare un client FTP per accedere al server o modificare i file dei temi direttamente dal dashboard di WordPress. L&#39;editor di file si trova sotto **Aspetto** nel menu della barra laterale.

   ![](assets/image2014-11-30-15-3a35-3a30.png)

1. Nell&#39;elenco dei file modello a destra dell&#39;editor di testo, trovare **header.php** e aprilo.

1. Vai a **Impostazioni account**.

   a. Se hai già ricevuto il tag JavaScript dal Supporto tecnico - continua con il passaggio 5.

   ![](assets/image2014-11-30-15-3a19-3a21-1.png)

1. In Dominio, individua il dominio pertinente e fai clic su **Genera tag**.

   ![](assets/image2014-11-30-15-3a20-3a17-1.png)

1. Copia il tag JavaScript RTP e incollalo nei modelli del tuo sito web.

   a. Accertati che si tratti del primo script nell’intestazione della pagina, tra **`<head> </head>`** tag.

   ![](assets/image2014-11-30-15-3a36-3a31.png)

1. Fai clic su **Aggiorna file** per il file header.php.

1. Verifica che venga visualizzato in tutte le pagine, incluse le pagine di destinazione e i sottodomini.

   a. Per farlo, fai clic con il pulsante destro del mouse sulla pagina del sito web. Vai a **Visualizza origine pagina.** Cerca **RTP** per individuare il tag.
