---
unique-page-id: 37355758
description: Scopri come aggiungere membri a un programma di eventi in Marketo. Aggiungi persone al programma per la registrazione o il tracciamento della partecipazione.
title: Aggiunta di membri a un programma evento
exl-id: 05bd4807-3ab8-452d-a389-b22477cf7445
feature: Events
TQID: 'https://experienceleague.adobe.com/dazVH2bQ--OqwAYWwyT4mBM-hVd4CamYMBMGnPvqO2c'
product_v2:
  - id: b27e5950-9033-45ac-9f86-eb22e567f615
    internal-label: Marketo Engage
feature_v2:
  - id: c5620c2c-7950-5a31-936a-f3b3287f198b
    internal-label: Events
source-git-commit: f3418961b6e4611317b38dcd54a76871e9f2560d
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 8%
---
# Aggiunta di membri a un programma evento {#adding-members-to-an-event-program}

Questo articolo si applica solo agli utenti che utilizzano il limite degli eventi o gli obiettivi degli eventi.

>[!CAUTION]
>
>L’importazione di un elenco di persone direttamente in un programma di eventi impedisce che tali record vengano conteggiati nelle registrazioni effettive nel rapporto Tracciamento obiettivo e nel rapporto Progressione limite evento. Segui le istruzioni riportate di seguito per assicurarti che i tuoi dati vengano conteggiati.

1. Crea e [aggiungi persone a un elenco statico](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/create-a-static-list.md).

1. [Crea una campagna avanzata](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md).

1. Nell&#39;elenco avanzato della campagna avanzata creata nel passaggio due, trovare e aggiungere il filtro **[!UICONTROL Member of List]**.

   ![](assets/three.png)

1. Individuare e selezionare l&#39;elenco creato nel passaggio 1.

   ![](assets/four.png)

1. Nel flusso, trovare e aggiungere il passaggio di flusso **[!UICONTROL Change Program Status]**.

   ![](assets/five.png)

1. Trova e seleziona il programma dell’evento.

   ![](assets/six.png)

1. Scegli lo stato desiderato.

   ![](assets/seven.png)

1. Nella scheda [!UICONTROL Schedule], fare clic su **[!UICONTROL Run Once]**.

   ![](assets/eight.png)

1. Seleziona **[!UICONTROL Run Now]** e fai clic su **[!UICONTROL Run]**.

   ![](assets/nine.png)

1. Dopo l’esecuzione della campagna intelligente, i membri vengono aggiunti al programma e vengono conteggiati nei calcoli di Tracciamento obiettivo e Progressione limite evento.
