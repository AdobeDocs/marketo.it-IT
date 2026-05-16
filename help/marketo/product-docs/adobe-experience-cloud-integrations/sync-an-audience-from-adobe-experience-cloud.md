---
description: Scopri come sincronizzare un pubblico da Adobe Experience Cloud a Marketo Engage. Richiama i tipi di pubblico dalla Libreria tipi di pubblico nel database di Marketo per utilizzarli nelle campagne e nei programmi.
title: Sincronizzare un pubblico da Adobe Experience Cloud
exl-id: 2288ee01-2c2e-4f33-b5c9-da3a431c1816
feature: Integrations
TQID: https://experienceleague.adobe.com/XCskpUNcNae-ikOLXxREb4kePbFs9HRheIihzJqHKoU
product_v2: id: b27e5950-9033-45ac-9f86-eb22e567f615
feature_v2: id: b13bd2ad-8e65-49e5-9691-2a0d31067b35id: c5f60233-d5ea-4453-a799-0ad258b4d399id: ea90ebee-5c84-42d9-8b21-006bdabc95a3
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
source-git-commit: a526f0bf4cbdf888b1c4462ba35dd2bc92316527
workflow-type: tm+mt
source-wordcount: 280
ht-degree: 8%

---

# Sincronizzare un pubblico da Adobe Experience Cloud {#sync-an-audience-from-adobe-experience-cloud}

>[!NOTE]
>
>Una distribuzione compatibile con HIPAA di un’istanza Marketo non può utilizzare questa integrazione.

>[!PREREQUISITES]
>
>[Imposta mappatura organizzazione Adobe](/help/marketo/product-docs/adobe-experience-cloud-integrations/set-up-adobe-organization-mapping.md){target="_blank"}

## Sincronizzare un pubblico {#how-to-sync-an-audience}

1. In Il mio Marketo, fare clic sul riquadro **[!UICONTROL Database]**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-1.png)

1. Fai clic sul menu a discesa **[!UICONTROL New]** e seleziona **[!UICONTROL Sync from Experience Cloud Audience]**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-2.png)

1. Fare clic sul menu a discesa **[!UICONTROL Audience Library Folder]** e selezionare la cartella di origine desiderata.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-3.png)

1. Selezionare un **[!UICONTROL Audience Name]**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-4.png)

1. Per la destinazione, puoi selezionare un elenco esistente o digitarne il nome di uno nuovo. In questo esempio viene creato un nuovo elenco. Al termine, fai clic su **[!UICONTROL Sync]**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-5.png)

1. Fai clic su **[!UICONTROL OK]**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-6.png)

## Domande frequenti {#faq}

**Come funziona la sincronizzazione dei cookie?**

Quando la sincronizzazione dei cookie è abilitata per l’abbonamento a Marketo, munchkin.js di Marketo tenta di acquisire e memorizzare gli ECID di Adobe per l’organizzazione IMS di Adobe specificata durante la configurazione dell’integrazione e di far corrispondere questi ECID all’identificatore cookie di Marketo corrispondente. Questo consente ai profili utente anonimi di Marketo di arricchirsi con gli ECID di Adobe.

È necessario un ulteriore passaggio per associare il profilo utente anonimo a un profilo lead, identificato mediante un’e-mail in testo normale. [ è descritto esattamente come funziona](/help/marketo/product-docs/reporting/basic-reporting/report-activity/tracking-anonymous-activity-and-people.md){target="_blank"}.

**Perché la dimensione dell&#39;elenco in Marketo è diversa da quella in Adobe?**

Inoltre, una persona non eseguirà la sincronizzazione se un ID cookie ECID non può essere associato a una persona nota in Marketo.

**È una sincronizzazione occasionale?**

È sufficiente avviare la sincronizzazione una sola volta. In seguito, i record verranno sincronizzati automaticamente. La sincronizzazione iniziale può richiedere fino a 24 ore; in futuro, la sincronizzazione dei nuovi record sarà tra 2 e 3 ore.
