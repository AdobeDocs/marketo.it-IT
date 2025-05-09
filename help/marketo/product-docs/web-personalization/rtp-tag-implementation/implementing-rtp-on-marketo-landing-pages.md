---
unique-page-id: 4720151
description: Implementazione di RTP sulle pagine di destinazione di Marketo - Documentazione di Marketo - Documentazione del prodotto
title: Implementazione di RTP sulle pagine di destinazione di Marketo
exl-id: fd19c3ad-d3f6-44a3-9f7a-d518e2d3f02a
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '195'
ht-degree: 0%

---

# Implementazione di RTP sulle pagine di destinazione di Marketo {#implementing-rtp-on-marketo-landing-pages}

Per implementare il tag RTP, seguire le istruzioni di installazione riportate di seguito:

1. Passare a **Design Studio.** Aprire l&#39;elemento da modificare. Seleziona **Azioni modello**, seleziona **Modifica bozza**.

   ![](assets/image2015-4-26-18-3a27-3a4.png)

1. Apporta le modifiche al modello nella scheda **HTML Source**.

   ![](assets/image2015-4-26-18-3a28-3a17.png)

1. Nel tuo account RTP, vai a **Impostazioni account**.

   a. Se hai già ricevuto il tag JavaScript dal Supporto tecnico - continua con il passaggio 5.

   ![](assets/image2014-11-30-15-3a19-3a21-2.png)

1. In Dominio individuare il dominio pertinente e fare clic su **Genera tag**.

   ![](assets/image2015-4-26-18-3a27-3a35.png)

   ![](assets/image2014-11-30-15-3a20-3a17-2.png)

1. Copiare il tag JavaScript RTP e incollarlo in tutti i modelli di pagina di destinazione tra i tag **`<head> </head>`**.

1. Fai clic su **Salva** e **Chiudi** la finestra.

1. Tornando a **Design Studio**, approva la pagina di destinazione da **Azioni modello**, fai clic su **Approva**.

   ![](assets/image2015-4-26-18-3a28-3a30.png)

1. Infine, per rendere effettive le modifiche apportate al modello, **devi approvare nuovamente** le pagine di destinazione che utilizzano tale modello. Puoi approvarli nuovamente tutte contemporaneamente dalla sezione Pagine di destinazione principale.

   ![](assets/image2015-4-26-18-3a28-3a49.png)

1. Verifica che venga visualizzato in tutte le pagine, incluse le pagine di destinazione e i sottodomini.

   A tale scopo, fai clic con il pulsante destro del mouse sulla pagina del sito web. Vai a **Visualizza Source pagine.** Cerca **RTP** per individuare il tag.
