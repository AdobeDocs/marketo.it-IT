---
description: Configurazione delle visualizzazioni MSI - Documentazione di Marketo - Documentazione del prodotto
title: Configurazione delle visualizzazioni MSI
exl-id: 8a45c006-73d4-4af8-ad62-b084056d1f7d
feature: Marketo Sales Insights
source-git-commit: 431bd258f9a68bbb9df7acf043085578d3d91b1f
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 0%

---

# Configurazione delle visualizzazioni MSI {#setting-up-msi-views}

L’installazione del plug-in Sales Insight in Dynamics aggiunge automaticamente gli elementi di maggiore rilevanza e le dashboard correlate nella mappa del sito. Se per qualche motivo le dashboard non vengono aggiunte, ecco come aggiungerle manualmente.

1. In Dynamics, fai clic sull’icona a forma di ingranaggio e seleziona **Impostazioni avanzate** dal menu a discesa.

1. In alto a sinistra, fai clic su **Impostazioni**. In Personalizzazione scegliere **Personalizzazioni**.

1. Clic **Personalizzare il sistema**.

1. Nella struttura ad albero a sinistra, fai clic su **Estensioni client** e doppio clic **Mappa del sito**.

1. Fare clic sulla freccia destra per passare alla pagina successiva. Alla voce Vendite, dovresti trovare Marketo. In caso contrario, assicurati di aver importato correttamente il pacchetto.

   >[!NOTE]
   >
   >In Marketo dovresti disporre di: Elementi di maggiore rilevanza, E-mail, Attività web e Attività web anonima. Se manca qualcuno di questi dashboard, fai clic sul segno + sopra Vendite e aggiungili come sottoarea.

1. Fai clic su una dashboard per selezionarla. Nella colonna a destra, inserisci le rispettive informazioni di seguito per ciascuno di essi. Puoi ignorare tutte le categorie non elencate.

   **Elementi di maggiore rilevanza**</br>
URL: MainviewBestbets.html</br>
Icona: /WebResources/mkt_/_MainView/_imgs/icons/bestbets.svg</br>
ID: marketo_bestbets</br>
Title: Elementi di maggiore rilevanza

   **E-mail**</br>
URL: mkt_/MainViewMyEmail.html</br>
Icona: /WebResources/mkt_/_MainView/_imgs/icons/email.svg</br>
ID: marketo_myemail</br>
Titolo: E-mail

   **Attività web**</br>
URL: mkt_/MainViewWebActivity.html</br>
Icona: /WebResources/mkt_/_MainView/_imgs/icons/web_activity.svg</br>
ID: marketo_webactivity</br>
Titolo: Attività web

   **Attività Web anonima**</br>
URL: mkt_/MainViewWebActivity.html</br>
Icona: /WebResources/mkt_/_MainView/_imgs/icons/anonymous_web_activity.svg</br>
ID: marketo_anonymous_webactivity</br>
Titolo: Attività Web anonima

1. Clic **Salva** al termine.
