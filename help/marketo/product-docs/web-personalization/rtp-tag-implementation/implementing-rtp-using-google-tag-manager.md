---
unique-page-id: 4720145
description: Implementazione di RTP tramite Google Tag Manager - Documentazione Marketo - Documentazione del prodotto
title: Implementazione di RTP con Google Tag Manager
exl-id: f7f06779-8abe-4c8c-9197-9d0c6bcfed49
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '159'
ht-degree: 0%

---

# Implementazione di RTP con Google Tag Manager {#implementing-rtp-using-google-tag-manager}

Per implementare il tag RTP, segui le istruzioni di installazione riportate di seguito.

1. Accedi al tuo account Google Tag Manager.

1. Aggiungi un nuovo tag > Configurazioni tag > Tag HTML personalizzato**.** Chiamala **RTP**.

1. Accedi al tuo account RTP**.**

1. Vai a **Impostazioni account**.

   a) Se hai già ricevuto il tag JavaScript dal supporto , continua con il passaggio 6.

   ![](assets/image2014-11-30-15-3a19-3a21.png)

1. In Dominio, individua il dominio pertinente e fai clic su **Genera tag**.

   ![](assets/image2014-11-30-15-3a20-3a17.png)

1. Copia il tag JavaScript RTP e incollalo nel nuovo **Tag HTML personalizzato** creato (passaggio 1).

1. Fai clic su **+Aggiungi regola al tag Fire**. Seleziona **Tutte le pagine**.

1. Fai clic su **Salva** e [pubblicare la nuova versione](https://support.google.com/tagmanager/answer/2699097?hl=en).

1. Verifica che venga visualizzato su tutte le pagine, incluse le pagine di destinazione e i sottodomini.

   a) Per farlo, fai clic con il pulsante destro del mouse sulla pagina del sito web. Vai a **Elemento Inspect**, Cerca **RTP** per individuare il tag .
