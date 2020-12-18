---
unique-page-id: 4720810
description: Notizie personalizzate in Google - Marketo Docs - Documentazione prodotto
title: Osservazioni personalizzate in Google
translation-type: tm+mt
source-git-commit: e149133a5383faaef5e9c9b7775ae36e633ed7b1
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 0%

---


# Osservazioni personalizzate in Google {#personalized-remarketing-in-google}

La funzione di marcatura personalizzata consente di coinvolgere nuovamente gli utenti utilizzando i dati RTP e la potenza delle Google Analytics con la portata di Google Display Network.

>[!PREREQUISITES]
>
>* Completare la configurazione [Retargeting with Web Personalization Data](retargeting-with-web-personalization-data.md)
>* Rivedere la documentazione di [Note con Google Analytics Guida](https://support.google.com/analytics/topic/2611283?hl=en&amp;ref_topic=3413645)

>



## Creazione di un pubblico straordinario in Google {#creating-a-remarketing-audience-in-google}

1. Accedi alle tue Google Analytics. Fare clic su **Admin**, **Account**, **Property**. Fare clic su **Definizioni dell&#39;audience** e **Audiences**.

   ![](assets/remarketing-ga-screenshots.jpg)

1. Fare clic su **+Nuovo pubblico**.

   ![](assets/image2015-1-15-17-3a26-3a40.png)

1. **Configurazione** collegamento: Collegamento all&#39;account Google Adwords
1. **Definisci pubblico**: Fate clic su  **Crea nuovo**.

   ![](assets/image2015-1-15-17-3a32-3a4.png)

1. In Audience Builder, fai clic su **Sequences** e **Trova i dati RTP** in Custom Dimension, Custom Variables, Events.

>[!TIP]
>
>Come trovare i dati RTP in Analytics per creare il pubblico?
>
>Nelle Google Analytics:
>
>* Variabili personalizzate: Organizzazione, Industria
>* Categoria evento: Segmento, Insightera-CTA, RTP-Note
>* Etichetta evento: Nome segmento, Nome campagna, Nome pubblico segmentato

>
>
In Google Universal Analytics:
>
>* Dimension personalizzati: Organizzazione, Industria, Categoria (Fortune 500.1000, Global 2000), Gruppo (Enterprise, SMB), Elenco ABM (Elenco Account Denominato)
>* Categoria evento: RTP-Segment, RTP-Campaign RTP-Note
>* Etichetta evento: Nome segmento, Nome campagna, Nome pubblico segmentato

>



**Esempio di notorietà dell&#39;audience dai dati dell&#39;audience segmentata RTP**

1. Fare clic su **Sequenze.**
1. Selezionare **Etichetta evento.**
1. Immettete **Nome dell&#39;audience segmentata** (come viene visualizzato in RTP).
1. Fare clic su **Applica**.

![](assets/image2015-2-10-14-3a51-3a43.png)

**Esempio di pubblico dai dati del settore RTP**

![](assets/image2015-1-15-17-3a36-3a5.png)

1. Fare clic su **Sequenze**.
1. Selezionare** RTP-Industry**.
1. Immettere **Nome dell&#39;industria** (ad esempio Servizi finanziari, istruzione...)
1. Fare clic su **Applica**.
1. Immettete un **Nome audience**. Fare clic su **Salva**.

![](assets/image2015-1-15-18-3a29-3a16.png)

## Creazione di una campagna di annunci per commenti in Google Adwords {#create-a-remarketing-ad-campaign-in-google-adwords}

1. Accedi a **Google Adwords**. Fare clic su **Campagne**, selezionare **Visualizza solo rete**.

   ![](assets/image2015-1-15-18-3a31-3a58.png)

1. Immettere **Nome campagna**, selezionare **Tipo di commento.**

   ![](assets/image2015-1-15-18-3a35-3a7.png)

1. Immettere **Nome gruppo annunci,** immettere **CPC avanzato**, selezionare **Elenco commenti**.

   ![](assets/image2015-1-15-18-3a51-3a57.png)

1. Fate clic su Salva e continuate.
1. Aggiungi l&#39;immagine o l&#39;annuncio di testo e inizia la tua campagna di remarketing.

   ![](assets/image2015-1-15-18-3a47-3a21.png)

>[!NOTE]
>
>**Articoli correlati**
>
>* [Ritargeting con dati di personalizzazione Web](retargeting-with-web-personalization-data.md)
>* [Osservazioni personalizzate su Facebook](personalized-remarketing-in-facebook.md)

