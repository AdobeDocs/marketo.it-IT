---
unique-page-id: 9438139
description: Aggiunta di una persona al Inserisco nell'elenco Bloccati di - Documentazione di Marketo - Documentazione del prodotto
title: Aggiungi persona al Inserisco nell'elenco Bloccati di
exl-id: e4543bf9-11e9-42df-a31e-e2cebe24ad4a
feature: Smart Lists
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '216'
ht-degree: 0%

---

# Aggiungi persona al Inserisco nell&#39;elenco Bloccati di {#add-person-to-blocklist}

L’aggiunta di persone al tuo Elenco Bloccati di impedisce loro di ricevere la tua corrispondenza.

>[!NOTE]
>
>Marketo sta cambiando termini come Blacklist e Whitelist per Inserire nell&#39;elenco Bloccati e Inserire nell&#39;elenco Consentiti il nostro prodotto in modo da. Durante questo aggiornamento, potresti visualizzare i vecchi termini nell’interfaccia utente e nelle schermate della documentazione, nonché i nuovi termini nel testo della documentazione. Ci scusiamo per qualsiasi confusione.

1. [Crea un nuovo programma predefinito](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/create-a-program.md) e denominalo **Aggiungi al Inserisco nell&#39;elenco Bloccati di**.

1. Clic **Nuovo** e seleziona **Nuova risorsa locale**.

   ![](assets/image2015-8-14-11-3a0-3a46.png)

1. Denomina l’elenco e fai clic su **Crea**.

   ![](assets/image2015-8-14-11-3a2-3a26.png)

1. Aggiungi tutte le persone al tuo **Elenco avanzato** desideri aggiungerlo al tuo Inserisco nell&#39;elenco Bloccati di.

   >[!NOTE]
   >
   >Le persone nel tuo Inserisco nell&#39;elenco Bloccati di non riceveranno e-mail operative.

   ![](assets/three-6.png)

1. Clic **Nuovo** e seleziona **Nuova campagna avanzata**.

   ![](assets/image2015-8-14-11-3a12-3a35.png)

1. Denomina il **Nuova campagna avanzata**. Fai clic su **Crea**.

   ![](assets/image2015-8-14-11-3a13-3a36.png)

1. Trascina **Membro di elenco avanzato**.

   ![](assets/image2015-8-14-11-3a16-3a34.png)

1. Seleziona l’elenco avanzato appena creato.

   ![](assets/image2015-8-14-11-3a17-3a5.png)

1. Trascina **Modifica valore dati**.

   ![](assets/image2015-8-14-11-3a18-3a41.png)

1. Per **Flusso**, immetti **Blocca nell&#39;elenco** per **Attributo** e imposta **Nuovo valore** a **true**.

   ![](assets/image2015-8-14-11-3a21-3a1.png)

1. Il giorno **Pianificazione** , seleziona **Esegui una volta**.

   ![](assets/ten.png)

1. Seleziona **Esegui ora** e fai clic su **Esegui**.

   ![](assets/image2015-8-14-11-3a24-3a50.png)

   YAY! Queste persone non riceveranno più e-mail.

   >[!TIP]
   >
   >Creare un [attiva campagna intelligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md) utilizzo **Modifica valore dati** con **Blocca nell’elenco è true** per tutte le persone che in futuro avranno attributi che possono essere inseriti nell&#39;elenco Bloccati in modo da poter essere utilizzati in modo più efficiente.
