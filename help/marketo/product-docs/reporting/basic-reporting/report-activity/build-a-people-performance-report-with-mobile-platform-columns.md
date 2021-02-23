---
unique-page-id: 2951220
description: Creare un rapporto sulle prestazioni delle persone con colonne della piattaforma mobile - Documenti Marketo - Documentazione del prodotto
title: Creare un rapporto sulle prestazioni delle persone con le colonne della piattaforma mobile
translation-type: tm+mt
source-git-commit: 03ee7b69f691efce12825aa708c81dffa23cecd9
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 0%

---


# Creare un report sulle prestazioni delle persone con le colonne della piattaforma mobile {#build-a-people-performance-report-with-mobile-platform-columns}

Per creare un rapporto sulle prestazioni delle persone con le colonne della piattaforma mobile (iOS/Android), effettuate le seguenti operazioni.

## Creazione di elenchi smart per dispositivi mobili {#create-mobile-smart-lists}

1. Andate a **Marketing Activities**.

   ![](assets/ma.png)

1. Scegliete un programma.

   ![](assets/two-1.png)

1. In **Nuova**, selezionare **Nuova risorsa locale**.

   ![](assets/three-1.png)

1. Fare clic su **Smart List**.

   ![](assets/four-1.png)

1. Digitare un nome e fare clic su **Crea**.

   ![](assets/five-1.png)

1. Individuate e trascinate il filtro E-mail aperta nel quadro.

   ![](assets/six-1.png)

1. Impostate E-mail su **è qualsiasi**.

   ![](assets/seven.png)

1. Fare clic su **Aggiungi vincolo** e selezionare **Piattaforma**.

   ![](assets/eight.png)

   >[!TIP]
   >
   >In questo esempio è stato utilizzato il filtro E-mail aperta. Potete anche utilizzare il filtro E-mail con clic, in quanto contiene il vincolo Piattaforma.

1. Impostate Piattaforma su **iOS**.

   ![](assets/nine.png)

   >[!NOTE]
   >
   >Almeno una persona deve aver aperto una delle e-mail su un dispositivo iOS per consentirne la ricerca automatica da parte di Marketo. Se non viene visualizzato, potete digitarlo manualmente e salvarlo.

   Ora create un secondo elenco avanzato per la piattaforma &quot;Android&quot;. Una volta fatto, passate alla sezione successiva.

## Creare un report sulle prestazioni delle persone {#create-a-people-performance-report}

1. In Attività di marketing, selezionate il programma che contiene gli elenchi smart **iOS** e **Android**.

   ![](assets/ten.png)

1. In **Nuova**, selezionare **Nuova risorsa locale**.

   ![](assets/eleven.png)

1. Fare clic su **Report**.

   ![](assets/twelve.png)

1. Impostate Tipo su **Prestazioni persone**.

   ![](assets/thirteen.png)

1. Fare clic su **Crea**.

   ![](assets/fourteen.png)

   Stai andando alla grande! Passiamo ora alla sezione successiva.

## Aggiungi elenchi smart mobili come colonne {#add-mobile-smart-lists-as-columns}

1. Nel rapporto appena creato, fare clic su **Setup**, quindi trascinare **Colonne personalizzate** nell&#39;area di lavoro.

   ![](assets/fifteen.png)

   >[!NOTE]
   >
   >Per impostazione predefinita, il rapporto Prestazioni persone sta esaminando gli ultimi 7 giorni. Potete modificare il periodo di tempo facendo doppio clic su di esso.

1. Trovate e selezionate gli elenchi smart creati in precedenza e fate clic su **Applica**.

   ![](assets/sixteen.png)

1. Fare clic su **Report** per eseguire il rapporto e visualizzare i dati.

   ![](assets/seventeen.png)

   Abbastanza figo, giusto? Ben fatto!
