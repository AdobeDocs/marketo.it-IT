---
unique-page-id: 4720145
description: Implementazione di RTP tramite Google Tag Manager - Documentazione di Marketo - Documentazione del prodotto
title: Implementazione di RTP tramite Google Tag Manager
exl-id: f7f06779-8abe-4c8c-9197-9d0c6bcfed49
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '159'
ht-degree: 0%

---

# Implementazione di RTP tramite Google Tag Manager {#implementing-rtp-using-google-tag-manager}

Per implementare il tag RTP, seguire le istruzioni di installazione riportate di seguito.

1. Accedi al tuo account Google Tag Manager.

1. Aggiungi un nuovo Tag > Configurazioni tag > Tag HTML personalizzato**.** chiamarlo **RTP**.

1. Accedi al tuo account RTP**.**

1. Vai a **Impostazioni account**.

   a. Se hai già ricevuto il tag JavaScript dal Supporto, continua con il passaggio 6.

   ![](assets/image2014-11-30-15-3a19-3a21.png)

1. In Dominio, individua il dominio pertinente e fai clic su **Genera tag**.

   ![](assets/image2014-11-30-15-3a20-3a17.png)

1. Copia il tag JavaScript RTP e incollalo nel nuovo **Tag HTML personalizzato** creato (passaggio 1).

1. Clic **+Aggiungi regola al tag di attivazione**. Seleziona **Tutte le pagine**.

1. Clic **Salva** e [pubblica la nuova versione](https://support.google.com/tagmanager/answer/2699097?hl=en).

1. Verifica che venga visualizzato in tutte le pagine, incluse le pagine di destinazione e i sottodomini.

   a. Per farlo, fai clic con il pulsante destro del mouse sulla pagina del tuo sito web. Vai a **Elemento Inspect**, Cerca **RTP** per individuare il tag.
