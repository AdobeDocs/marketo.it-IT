---
description: Sincronizzare un pubblico da Adobe Experience Cloud - Documentazione Marketo - Documentazione del prodotto
title: Sincronizzare un pubblico da Adobe Experience Cloud
exl-id: 2288ee01-2c2e-4f33-b5c9-da3a431c1816
feature: Integrations
source-git-commit: 02b2e39580c5eac63de4b4b7fdaf2a835fdd4ba5
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 0%

---

# Sincronizzare un pubblico da Adobe Experience Cloud {#sync-an-audience-from-adobe-experience-cloud}

>[!NOTE]
>
>Una distribuzione compatibile con HIPAA di un’istanza Marketo non può utilizzare questa integrazione.

>[!PREREQUISITES]
>
>[Imposta mapping organizzazione Adobe](/help/marketo/product-docs/adobe-experience-cloud-integrations/set-up-adobe-organization-mapping.md){target="_blank"}

## Sincronizzare un pubblico {#how-to-sync-an-audience}

1. In Il mio Marketo, fai clic su **[!UICONTROL Database]** affiancare.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-1.png)

1. Fai clic su **[!UICONTROL Nuovo]** a discesa e selezionare **[!UICONTROL Sincronizza da pubblico Experience Cloud]**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-2.png)

1. Fai clic su **[!UICONTROL Cartella libreria Pubblico]** e selezionare la cartella di origine desiderata.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-3.png)

1. Seleziona un **[!UICONTROL Nome pubblico]**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-4.png)

1. Per la destinazione, puoi selezionare un elenco esistente o digitarne il nome di uno nuovo. In questo esempio ne stiamo creando uno nuovo. Clic **[!UICONTROL Sincronizza]** al termine.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-5.png)

1. Clic **[!UICONTROL OK]**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-6.png)

## Domande frequenti {#faq}

**Come funziona la sincronizzazione dei cookie?**

Quando la sincronizzazione dei cookie è abilitata per l’abbonamento a Marketo, munchkin.js di Marketo tenterà di acquisire e memorizzare gli ECID di Adobe per l’organizzazione IMS di Adobe specificata durante la configurazione dell’integrazione e far corrispondere questi ECID all’identificatore cookie di Marketo corrispondente. Questo consente ai profili utente anonimi di Marketo di arricchirsi di ECID Adobi.

È necessario un ulteriore passaggio per associare il profilo utente anonimo a un profilo lead, identificato utilizzando un’e-mail in testo normale. Esattamente come funziona [è descritto qui](/help/marketo/product-docs/reporting/basic-reporting/report-activity/tracking-anonymous-activity-and-people.md){target="_blank"}.

**Perché la dimensione dell’elenco in Marketo è diversa da quella in Adobe?**

Inoltre, una persona non eseguirà la sincronizzazione se non è possibile collegare un ID cookie ECID a una persona nota in Marketo.

**Questa è una sincronizzazione una tantum?**

È sufficiente avviare la sincronizzazione una sola volta. In seguito, i record verranno sincronizzati automaticamente. La sincronizzazione iniziale può richiedere fino a 24 ore; in futuro, i nuovi record verranno sincronizzati in 2-3 ore.
