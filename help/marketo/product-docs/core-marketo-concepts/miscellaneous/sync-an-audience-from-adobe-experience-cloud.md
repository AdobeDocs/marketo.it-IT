---
description: Sincronizzazione di un pubblico da Adobe Experience Cloud - Documentazione Marketo - Documentazione del prodotto
title: Sincronizzazione di un pubblico da Adobe Experience Cloud
exl-id: 2288ee01-2c2e-4f33-b5c9-da3a431c1816
translation-type: tm+mt
source-git-commit: 72e1d29347bd5b77107da1e9c30169cb6490c432
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 0%

---

# Sincronizzazione di un pubblico da Adobe Experience Cloud {#sync-an-audience-from-adobe-experience-cloud}

>[!NOTE]
>
>Impossibile utilizzare questa integrazione in una distribuzione HIPAA di un&#39;istanza Marketo.

>[!PREREQUISITES]
>
>[Configurare la condivisione del pubblico di Adobe Experience Cloud](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/set-up-adobe-experience-cloud-audience-sharing.md)

## Come sincronizzare un pubblico {#how-to-sync-an-audience}

1. In My Marketo, fai clic sul riquadro **Database** .

   ![](assets/sync-an-audience-from-adobe-experience-cloud-1.png)

1. Fai clic sul menu a discesa **Nuovo** e seleziona **Sincronizza da pubblico Experience Cloud**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-2.png)

1. Fai clic sul menu a discesa **Cartella libreria Pubblico** e seleziona la cartella di origine desiderata.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-3.png)

1. Seleziona un **Nome pubblico**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-4.png)

1. Per la destinazione, è possibile selezionare un elenco esistente o digitare il nome di un nuovo elenco. In questo esempio ne stiamo creando uno nuovo. Al termine, fai clic su **Sincronizza**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-5.png)

1. Fare clic su **OK**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-6.png)

## Domande frequenti {#faq}

**Come funziona la sincronizzazione dei cookie?**

Quando la sincronizzazione dei cookie è abilitata per la tua iscrizione Marketo, Marketo’s munchkin.js tenterà di acquisire e memorizzare gli ECID di Adobe per l’organizzazione IMS di Adobe specificata durante la configurazione dell’integrazione e di far corrispondere questi ECID all’identificatore del cookie Marketo corrispondente. Questo consente ai profili utente anonimi di Marketo di arricchirsi di ECID Adobi.

È necessario un ulteriore passaggio per associare il profilo utente anonimo a un profilo lead, identificato utilizzando un messaggio e-mail di testo normale. Come funziona esattamente [è descritto qui](/help/marketo/product-docs/reporting/basic-reporting/report-activity/tracking-anonymous-activity-and-people.md).

**Perché la dimensione dell’elenco in Marketo è diversa da quella dell’Adobe?**

Inoltre, una persona non si sincronizza se non è possibile collegare un ID cookie ECID a una persona nota in Marketo.

**È una sincronizzazione una tantum?**

È sufficiente avviare la sincronizzazione una sola volta. Successivamente, i record verranno sincronizzati automaticamente. La sincronizzazione iniziale può richiedere fino a 24 ore; in futuro, i nuovi record verranno sincronizzati in 2-3 ore.
