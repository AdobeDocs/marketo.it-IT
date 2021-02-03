---
unique-page-id: 37355758
description: Aggiunta di membri a un programma di eventi - Documenti Marketo - Documentazione prodotto
title: Aggiunta di membri a un programma evento
translation-type: tm+mt
source-git-commit: ed83438ae5660d172e845f25c4d72d599574bd91
workflow-type: tm+mt
source-wordcount: '177'
ht-degree: 0%

---


# Aggiunta di membri a un programma evento {#adding-members-to-an-event-program}

Questo articolo si applica solo agli utenti che utilizzano eventi Cap o Obiettivi evento.

>[!CAUTION]
>
>L&#39;importazione di un elenco di persone direttamente in un programma dell&#39;evento impedirà il conteggio di tali record nelle registrazioni effettive nel rapporto Tracciamento obiettivo e nel rapporto Progressi cap dell&#39;evento. Segui le istruzioni riportate di seguito per assicurarti che i tuoi documenti siano conteggiati.

1. Creare e [aggiungere persone a un elenco statico](/help/marketo/product-docs/core-marketo-concepts/smart-lists-and-static-lists/static-lists/create-a-static-list.md).

1. [Creare una campagna](/help/marketo/product-docs/core-marketo-concepts/smart-campaigns/creating-a-smart-campaign/create-a-new-smart-campaign.md) intelligente.

1. Nell&#39;elenco avanzato della Smart Campaign creata al passaggio 2, trovate e aggiungete il filtro **Member of List**.

   ![](assets/three.png)

1. Individuate e selezionate l’elenco creato al punto 1.

   ![](assets/four.png)

1. In Flusso, trova e aggiungi il passaggio di flusso **Modifica stato programma**.

   ![](assets/five.png)

1. Individuate e selezionate il programma dell&#39;evento.

   ![](assets/six.png)

1. Scegliete lo stato desiderato.

   ![](assets/seven.png)

1. Nella scheda Pianificazione, fare clic su **Esegui una volta**.

   ![](assets/eight.png)

1. Selezionare **Esegui ora** e fare clic su **Esegui**.

   ![](assets/nine.png)

1. Dopo l&#39;esecuzione della campagna intelligente, i membri vengono aggiunti al programma e vengono conteggiati nei calcoli di tracciamento degli obiettivi e di progressione dell&#39;app dell&#39;evento.
