---
unique-page-id: 4720810
description: Remarketing personalizzato in Google - Documentazione Marketo - Documentazione del prodotto
title: Remarketing personalizzato in Google
exl-id: cc733f43-161d-41e4-afdf-8b5217700810
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---

# Remarketing personalizzato in Google {#personalized-remarketing-in-google}

Il remarketing personalizzato consente di coinvolgere nuovamente gli utenti utilizzando i dati RTP e la potenza delle Google Analytics grazie alla rete di display Google.

>[!PREREQUISITES]
>
>* Completa il [Retargeting con dati di personalizzazione web](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md) configurazione
>* Revisione [Guida al remarketing con Google Analytics](https://support.google.com/analytics/topic/2611283?hl=en&amp;ref_topic=3413645) documentazione.

## Creazione di un pubblico per il remarketing in Google {#creating-a-remarketing-audience-in-google}

1. Accedi alle tue Google Analytics. Clic **Amministratore**, **Account**, **Proprietà**. Fai clic su **Definizioni del pubblico** e **Tipi di pubblico**.

   ![](assets/remarketing-ga-screenshots.jpg)

1. Clic **+Nuovo pubblico**.

   ![](assets/image2015-1-15-17-3a26-3a40.png)

1. **Configurazione collegamento**: collega al tuo account Google Adwords. **Definisci pubblico**: fai clic **Crea nuovo**.

   ![](assets/image2015-1-15-17-3a32-3a4.png)

1. In Audience Builder, fai clic su **Sequenze** e **Trovare i dati RTP** in Dimension personalizzati, Variabili personalizzate, Eventi.

>[!TIP]
>
>Come trovare i dati RTP in Analytics per creare il tuo pubblico?
>
>Nelle Google Analytics:
>
>* Variabili personalizzate: Organizzazione, Settore
>* Categoria evento: segmento, Insightera-CTA, RTP-remarketing
>* Etichetta evento: Nome segmento, Nome campagna, Nome pubblico segmentato
>
>In Google Universal Analytics:
>
>* Dimension personalizzati: Organizzazione, Settore, Categoria (Fortune 500,1000, Global 2000), Gruppo (Enterprise, SMB), Elenco ABM (Named Account List)
>* Categoria evento: RTP-Segment, RTP-Campaign RTP-Remarketing
>* Etichetta evento: Nome segmento, Nome campagna, Nome pubblico segmentato

**Esempio di pubblico di remarketing da dati di pubblico segmentato RTP**

1. Clic **Sequenze.**
1. Seleziona **Etichetta evento.**
1. Invio **Nome del pubblico segmentato** (come appare nella RTP).
1. Clic **Applica**.

![](assets/image2015-2-10-14-3a51-3a43.png)

**Esempio di pubblico da dati del settore RTP**

![](assets/image2015-1-15-17-3a36-3a5.png)

1. Clic **Sequenze**.
1. Seleziona **RTP-Industry**.
1. Invio **Nome dell’industria** (es. Servizi finanziari, istruzione...).
1. Clic **Applica**.
1. Immetti un **Nome pubblico**. Clic **Salva**.

![](assets/image2015-1-15-18-3a29-3a16.png)

## Creare una campagna di annunci di remarketing in Google Adwords {#create-a-remarketing-ad-campaign-in-google-adwords}

1. Accedi a **Google Adwords**. Fai clic su **Campagne**, seleziona **Visualizza solo rete**.

   ![](assets/image2015-1-15-18-3a31-3a58.png)

1. Invio **Nome campagna**, Seleziona **Digitare Remarketing.**

   ![](assets/image2015-1-15-18-3a35-3a7.png)

1. Invio **Nome del gruppo di annunci,** Invio **CPC avanzato**, Seleziona **Elenco remarketing**.

   ![](assets/image2015-1-15-18-3a51-3a57.png)

1. Fai clic su Salva e continua.
1. Aggiungi un annuncio di testo o immagine e avvia la campagna di remarketing.

   ![](assets/image2015-1-15-18-3a47-3a21.png)

>[!MORELIKETHIS]
>
>* [Retargeting con dati di personalizzazione web](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* [Remarketing personalizzato in Facebook](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md)
