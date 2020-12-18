---
unique-page-id: 37355758
description: Aggiunta di membri a un programma di eventi - Documenti Marketo - Documentazione prodotto
title: Aggiunta di membri a un programma evento
translation-type: tm+mt
source-git-commit: 47b2fee7d146c3dc558d4bbb10070683f4cdfd3d
workflow-type: tm+mt
source-wordcount: '186'
ht-degree: 0%

---


# Aggiunta di membri a un programma evento {#adding-members-to-an-event-program}

Questo articolo si applica solo agli utenti che utilizzano eventi Cap o Obiettivi evento.

>[!CAUTION]
>
>L&#39;importazione di un elenco di persone direttamente in un programma dell&#39;evento impedirà il conteggio di tali record nelle registrazioni effettive nel rapporto Tracciamento obiettivo e nel rapporto Progressi cap dell&#39;evento. Segui le istruzioni riportate di seguito per assicurarti che i tuoi documenti siano conteggiati.

1. Creare e [aggiungere persone a un elenco statico](http://docs.marketo.com/x/ecKt).
1. [Creare una campagna](http://docs.marketo.com/x/M4AR) intelligente.
1. Nell&#39;elenco avanzato della Smart Campaign creata al passaggio 2, trovate e aggiungete il filtro **Member of List**.

   ![](assets/three.png)

1. Individuate e selezionate l’elenco creato al punto 1.
1. ![](assets/four.png)

1. In Flusso, trova e aggiungi il passaggio di flusso **Modifica stato programma**.
1. ![](assets/five.png)

1. Individuate e selezionate il programma dell&#39;evento.

   ![](assets/six.png)

1. Scegliete lo stato desiderato.

   ![](assets/seven.png)

1. Nella scheda Pianificazione, fare clic su **Esegui una volta**.
1. ![](assets/eight.png)

1. Selezionare **Esegui ora** e fare clic su **Esegui**.
1. ![](assets/nine.png)

1. Dopo l&#39;esecuzione della campagna intelligente, i membri vengono aggiunti al programma e vengono conteggiati nei calcoli di tracciamento degli obiettivi e di progressione dell&#39;app dell&#39;evento.

