---
unique-page-id: 9438139
description: Aggiunta di una persona al Inserisco nell'elenco Bloccati di - Documentazione di Marketo - Documentazione del prodotto
title: Aggiungi persona al Inserisco nell'elenco Bloccati di
exl-id: e4543bf9-11e9-42df-a31e-e2cebe24ad4a
feature: Smart Lists
source-git-commit: cc87ecb8d3245734ec0ce984eeccf742833a85d2
workflow-type: tm+mt
source-wordcount: '184'
ht-degree: 1%

---

# Aggiungi persona al Inserisco nell&#39;elenco Bloccati di {#add-person-to-blocklist}

L’aggiunta di persone al tuo Elenco Bloccati di impedisce loro di ricevere la tua corrispondenza.

1. [Crea un nuovo programma predefinito](/help/marketo/product-docs/core-marketo-concepts/programs/creating-programs/create-a-program.md) e denominalo **Aggiungi al Inserisco nell&#39;elenco Bloccati di**.

1. Clic **Nuovo** e seleziona **Nuova risorsa locale**.

   ![](assets/add-person-to-blocklist-1.png)

1. Seleziona **Elenco avanzato**.

   ![](assets/add-person-to-blocklist-2.png)

1. Denomina l’elenco e fai clic su **Crea**.

   ![](assets/add-person-to-blocklist-3.png)

1. Aggiungi tutte le persone al tuo **Elenco avanzato** desideri aggiungerlo al tuo Inserisco nell&#39;elenco Bloccati di.

   ![](assets/add-person-to-blocklist-4.png)

   >[!NOTE]
   >
   >Le persone nel tuo Inserisco nell&#39;elenco Bloccati di non riceveranno e-mail operative.

1. Torna al tuo programma.

   ![](assets/add-person-to-blocklist-5.png)

1. Clic **Nuovo** e seleziona **Nuova campagna avanzata**.

   ![](assets/add-person-to-blocklist-6.png)

1. Denomina il **Nuova campagna avanzata**. Fai clic su **Crea**.

   ![](assets/add-person-to-blocklist-7.png)

1. Trascina **Membro di elenco avanzato**.

   ![](assets/add-person-to-blocklist-8.png)

1. Seleziona l’elenco avanzato appena creato.

   ![](assets/add-person-to-blocklist-9.png)

1. Fai clic su **Flusso** scheda. Trascina la **Modifica valore dati** Azione di flusso.

   ![](assets/add-person-to-blocklist-10.png)

1. In **Attributo** selezione a discesa **Blocca nell&#39;elenco** e imposta **Nuovo valore** a **true**.

   ![](assets/add-person-to-blocklist-11.png)

1. Fai clic su **Pianificazione** e seleziona **Esegui una volta**.

   ![](assets/add-person-to-blocklist-12.png)

1. Seleziona **Esegui ora** e fai clic su **Esegui**.

   ![](assets/add-person-to-blocklist-13.png)

1. Clic **Esegui** di nuovo.

   ![](assets/add-person-to-blocklist-14.png)

Queste persone non riceveranno più e-mail.

>[!TIP]
>
>Creare un [attiva campagna intelligente](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md) utilizzo **Modifica valore dati** con **Blocca nell’elenco è true** per tutte le persone che in futuro avranno attributi che possono essere inseriti nell&#39;elenco Bloccati in modo da poter essere utilizzati in modo più efficiente.
