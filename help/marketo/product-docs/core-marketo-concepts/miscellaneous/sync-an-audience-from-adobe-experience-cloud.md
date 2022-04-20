---
description: Sincronizzazione di un pubblico da Adobe Experience Cloud - Documentazione Marketo - Documentazione del prodotto
title: Sincronizzazione di un pubblico da Adobe Experience Cloud
exl-id: 2288ee01-2c2e-4f33-b5c9-da3a431c1816
source-git-commit: 86451f1027e74479a415a4c6654a2625275d4112
workflow-type: tm+mt
source-wordcount: '272'
ht-degree: 0%

---

# Sincronizzazione di un pubblico da Adobe Experience Cloud {#sync-an-audience-from-adobe-experience-cloud}

>[!NOTE]
>
>Impossibile utilizzare questa integrazione in una distribuzione HIPAA di un&#39;istanza Marketo.

>[!PREREQUISITES]
>
>[Impostazione della mappatura dell&#39;organizzazione Adobe](/help/marketo/product-docs/core-marketo-concepts/miscellaneous/set-up-adobe-organization-mapping.md)

## Come sincronizzare un pubblico {#how-to-sync-an-audience}

1. In My Marketo, fai clic sul pulsante **Database** piastrelle.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-1.png)

1. Fai clic sul pulsante **Nuovo** a discesa e seleziona **Sincronizzazione da pubblico Experience Cloud**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-2.png)

1. Fai clic sul pulsante **Cartella Libreria Pubblico** e seleziona la cartella di origine desiderata.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-3.png)

1. Seleziona un **Nome del pubblico**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-4.png)

1. Per la destinazione, è possibile selezionare un elenco esistente o digitare il nome di un nuovo elenco. In questo esempio ne stiamo creando uno nuovo. Fai clic su **Sincronizzazione** al termine.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-5.png)

1. Fai clic su **OK**.

   ![](assets/sync-an-audience-from-adobe-experience-cloud-6.png)

## Domande frequenti {#faq}

**Come funziona la sincronizzazione dei cookie?**

Quando la sincronizzazione dei cookie è abilitata per la tua iscrizione Marketo, Marketo’s munchkin.js tenterà di acquisire e memorizzare gli ECID Adobi per l’organizzazione Adobe IMS specificata durante la configurazione dell’integrazione e di far corrispondere questi ECID all’identificatore cookie Marketo corrispondente. Questo consente ai profili utente anonimi di Marketo di arricchirsi di ECID Adobi.

È necessario un ulteriore passaggio per associare il profilo utente anonimo a un profilo lead, identificato utilizzando un messaggio e-mail di testo normale. Esattamente come funziona [è descritto qui](/help/marketo/product-docs/reporting/basic-reporting/report-activity/tracking-anonymous-activity-and-people.md).

**Perché la dimensione dell’elenco in Marketo è diversa da quella dell’Adobe?**

Inoltre, una persona non si sincronizza se non è possibile collegare un ID cookie ECID a una persona nota in Marketo.

**È una sincronizzazione una tantum?**

È sufficiente avviare la sincronizzazione una sola volta. Successivamente, i record verranno sincronizzati automaticamente. La sincronizzazione iniziale può richiedere fino a 24 ore; in futuro, i nuovi record verranno sincronizzati in 2-3 ore.
