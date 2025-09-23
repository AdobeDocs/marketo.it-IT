---
unique-page-id: 37355758
description: Aggiunta di membri a un programma di eventi - Documentazione di Marketo - Documentazione del prodotto
title: Aggiunta di membri a un programma evento
exl-id: 05bd4807-3ab8-452d-a389-b22477cf7445
feature: Events
source-git-commit: 09a656c3a0d0002edfa1a61b987bff4c1dff33cf
workflow-type: tm+mt
source-wordcount: '165'
ht-degree: 9%

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
