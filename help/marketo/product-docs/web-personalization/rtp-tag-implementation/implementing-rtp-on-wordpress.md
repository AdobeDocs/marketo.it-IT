---
unique-page-id: 4720149
description: Implementazione di RTP su Wordpress - Marketo Docs - Documentazione del prodotto
title: Implementazione di RTP su Wordpress
exl-id: f010942b-02bb-447b-a272-c4237782b2d7
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '187'
ht-degree: 0%

---

# Implementazione di RTP su Wordpress {#implementing-rtp-on-wordpress}

Per implementare il tag RTP, segui le istruzioni di installazione riportate di seguito:

1. Apri **header.php** file **Tema WordPress**.

   È possibile utilizzare un client FTP per accedere al server o modificare i file dei temi direttamente dal dashboard di WordPress. L&#39;editor di file si trova nella sezione **Aspetto** nel menu della barra laterale.

   ![](assets/image2014-11-30-15-3a35-3a30.png)

1. Nell’elenco dei file modello a destra dell’editor di testo, trova **header.php** e aprilo.

1. Vai a **Impostazioni account**.

   a) Se hai già ricevuto il tag JavaScript dal supporto - continua con il passaggio 5.

   ![](assets/image2014-11-30-15-3a19-3a21-1.png)

1. In Dominio, individua il dominio pertinente e fai clic su **Genera tag**.

   ![](assets/image2014-11-30-15-3a20-3a17-1.png)

1. Copia il tag JavaScript RTP e incollalo nei modelli del sito web.

   a) Assicurati che sia il primo script nell’intestazione della pagina, tra **`<head> </head>`** tag.

   ![](assets/image2014-11-30-15-3a36-3a31.png)

1. Fai clic su **Aggiorna file** per il file header.php .

1. Verifica che venga visualizzato su tutte le pagine, incluse le pagine di destinazione e i sottodomini.

   a) Per farlo, fai clic con il pulsante destro del mouse sulla pagina del sito web. Vai a **Visualizza origine pagina.** Cerca **RTP** per individuare il tag .
