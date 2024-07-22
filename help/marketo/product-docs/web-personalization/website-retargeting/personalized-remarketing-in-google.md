---
unique-page-id: 4720810
description: Remarketing personalizzato in Google - Documentazione Marketo - Documentazione del prodotto
title: Remarketing personalizzato in Google
exl-id: cc733f43-161d-41e4-afdf-8b5217700810
feature: Web Personalization
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---

# Remarketing personalizzato in Google {#personalized-remarketing-in-google}

Il remarketing personalizzato consente di coinvolgere nuovamente gli utenti utilizzando i dati RTP e la potenza delle Google Analytics grazie alla rete di display Google.

>[!PREREQUISITES]
>
>* Completa la configurazione di [Retargeting con dati Web Personalization](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* Rivedi la documentazione di [Remarketing con Guida di Google Analytics](https://support.google.com/analytics/topic/2611283?hl=en&amp;ref_topic=3413645).

## Creazione di un pubblico per il remarketing in Google {#creating-a-remarketing-audience-in-google}

1. Accedi alle tue Google Analytics. Fai clic su **Amministratore**, **Account**, **Proprietà**. Fai clic su **Definizioni pubblico** e **Pubblico**.

   ![](assets/remarketing-ga-screenshots.jpg)

1. Fai clic su **+Nuovo pubblico**.

   ![](assets/image2015-1-15-17-3a26-3a40.png)

1. **Configurazione collegamento**: collega al tuo account Google Adwords. **Definisci pubblico**: Fai clic su **Crea nuovo**.

   ![](assets/image2015-1-15-17-3a32-3a4.png)

1. In Audience Builder, fai clic su **Sequenze** e **Trova i dati RTP** in Dimension personalizzati, variabili personalizzate, eventi.

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

**Esempio di pubblico di remarketing dai dati del pubblico segmentato RTP**

1. Fai clic su **Sequenze.**
1. Seleziona **Etichetta evento.**
1. Immetti **Nome del pubblico segmentato** (come appare in RTP).
1. Fare clic su **Applica**.

![](assets/image2015-2-10-14-3a51-3a43.png)

**Esempio di pubblico dai dati del settore RTP**

![](assets/image2015-1-15-17-3a36-3a5.png)

1. Fai clic su **Sequenze**.
1. Selezionare **RTP-Industry**.
1. Immetti **Nome del settore** (esempio: Servizi finanziari, istruzione...).
1. Fare clic su **Applica**.
1. Immetti un **Nome pubblico**. Fai clic su **Salva**.

![](assets/image2015-1-15-18-3a29-3a16.png)

## Creare una campagna di annunci di remarketing in Google Adwords {#create-a-remarketing-ad-campaign-in-google-adwords}

1. Accedi a **Google Adwords**. Fai clic su **Campagne**, seleziona **Visualizza solo rete**.

   ![](assets/image2015-1-15-18-3a31-3a58.png)

1. Immetti **Nome Campagna**, Seleziona **Tipo Remarketing.**

   ![](assets/image2015-1-15-18-3a35-3a7.png)

1. Immetti **Nome gruppo di annunci** immetti **CPC avanzato**, seleziona **Elenco remarketing**.

   ![](assets/image2015-1-15-18-3a51-3a57.png)

1. Fai clic su Salva e continua.
1. Aggiungi un annuncio di testo o immagine e avvia la campagna di remarketing.

   ![](assets/image2015-1-15-18-3a47-3a21.png)

>[!MORELIKETHIS]
>
>* [Retargeting con dati Web Personalization](/help/marketo/product-docs/web-personalization/website-retargeting/retargeting-with-web-personalization-data.md)
>* [Remarketing personalizzato in Facebook](/help/marketo/product-docs/web-personalization/website-retargeting/personalized-remarketing-in-facebook.md)
