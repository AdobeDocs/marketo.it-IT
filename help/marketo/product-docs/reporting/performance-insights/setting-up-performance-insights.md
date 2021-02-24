---
unique-page-id: 12981145
description: Impostazione di approfondimenti sulle prestazioni - Documenti Marketo - Documentazione del prodotto
title: Impostazione di approfondimenti sulle prestazioni
translation-type: tm+mt
source-git-commit: cb7df3dd38275837f8ab05ce846c2c68ab78462f
workflow-type: tm+mt
source-wordcount: '307'
ht-degree: 0%

---


# Impostazione di approfondimenti sulle prestazioni {#setting-up-performance-insights}

Seguite i passaggi riportati di seguito per impostare MPI.

## Impostazione opportunità {#opportunity-setup}

1. Fare clic su **Admin**.

   ![](assets/admin.png)

1. Fare clic su **Analisi del ciclo economico**.

   ![](assets/two-2.png)

   >[!NOTE]
   >
   >Se non si dispone di RCA, è necessario selezionare **Analisi programma** per il passaggio 2.

1. In Attribuzione, fare clic su **Modifica**.

   ![](assets/three-1.png)

1. Vengono visualizzate le impostazioni di attribuzione.

   ![](assets/four-2.png)

   Se Attribuzione è esplicita, accertatevi che il ruolo di contatto opportunità sia stato popolato (tramite l&#39;endpoint Ruolo opportunità o tramite l&#39;integrazione CRM).

   Se Attribuzione è implicita, accertatevi che il campo società sul lead/contatto sia lo stesso del Nome account dell&#39;opportunità.

   >[!NOTE]
   >
   >Verifica che tutti i campi delle opportunità siano compilati:
   >
   >* Importo opportunità
   >* È chiusa
   >* È stato vinto
   >* Data creazione (questa impostazione potrebbe non essere impostata nel caso in cui lo si tratti)
   >* Data di chiusura (potrebbe non essere impostato nel caso in cui lo si tratti)
   >* Tipo opportunità


## Impostazione programma {#program-setup}

Aggiornare i costi del programma per almeno 12 mesi. Puoi farlo manualmente o utilizzando l&#39;API del programma. In questo esempio lo facciamo manualmente.

1. Fate clic su **Attività marketing**.

   ![](assets/ma.png)

1. Trova e seleziona il programma.

   ![](assets/select-program.png)

1. Fare clic sulla scheda **Setup**.

   ![](assets/setup-tab.png)

1. Trascinare **Costo periodo** nell&#39;area di lavoro.

   ![](assets/period-cost.png)

1. Impostare il mese del programma almeno 12 mesi fa e fare clic su **Ok**.

   ![](assets/set-period.png)

1. Impostate il costo del periodo e fate clic su **Salva**.

   ![](assets/set-cost.png)

Quindi, controlla il comportamento di analisi per indicare se un particolare canale deve essere incluso nell&#39;analisi. Impostate il comportamento di Analytics (Normale, Inclusivo, Operativo).

1. Fare clic su **Admin**.

   ![](assets/admin.png)

1. Fare clic su **Tag**.

   ![](assets/tags.png)

1. Fare clic su **+** per espandere l&#39;elenco Canale.

   ![](assets/channel.png)

1. Fate doppio clic sul canale desiderato.

   ![](assets/channel-click.png)

1. Fai clic sul menu a discesa **Comportamento analisi** e seleziona il comportamento desiderato.

   ![](assets/edit-channel.png)

1. Impostate i criteri di successo.

   ![](assets/success.png)

1. Fare clic su **Salva**.

   ![](assets/save.png)

## Collegare il programma alla persona {#tie-the-program-to-the-person}

1. Accertati che il programma di acquisizione e la data di acquisizione siano stati impostati per ogni persona presente nel tuo database al fine di poter utilizzare la funzione First Touch Attribution.
1. Assicurati che i tuoi programmi stiano impostando gli stati di successo per le persone.

>[!NOTE]
>
>Le modifiche apportate non sono istantanee. Prima dell&#39;entrata in vigore delle modifiche è necessario un periodo overnight.
